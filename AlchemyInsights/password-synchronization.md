---
title: Parooli sünkroonimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481445"
---
# <a name="password-synchronization"></a><span data-ttu-id="53d34-102">Parooli sünkroonimine</span><span class="sxs-lookup"><span data-stu-id="53d34-102">Password synchronization</span></span>

<span data-ttu-id="53d34-103">**Parooli Hash sünkroonimine ei tööta üldse**</span><span class="sxs-lookup"><span data-stu-id="53d34-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="53d34-104">Mõned levinud probleemid klientidega, kui parooli Hash sünkroonimine ei tööta, on järgmised.</span><span class="sxs-lookup"><span data-stu-id="53d34-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="53d34-105">Azure AD ' is kasutatava Active Directory kontoga suhtlemiseks kohapealse Active Directory abil pole antud **tiražeerimise kataloogi muudatusi** ja **tiražeerimise register muudab kõik** juurdepääsuõigused, mida on vaja parooli sünkroonimiseks – peate selle parandama, andes need juurdepääsuõigused Active Directory kontole.</span><span class="sxs-lookup"><span data-stu-id="53d34-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="53d34-106">Parooli Hash sünkroonimine on keelatud pärast seda, kui administraator muutis kasutaja Sign-In meetod **parooli sünkroonimise** teise variandi (nt **Föderatsioon AD FS** Azure AD Connecti viisardiga) – saate selle parandada, kui lubate Azure AD Connecti viisardis **parooli Hash sünkroonimise** funktsiooni.</span><span class="sxs-lookup"><span data-stu-id="53d34-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="53d34-107">Ühenduvuse probleem kohapealne Active Directoryga.</span><span class="sxs-lookup"><span data-stu-id="53d34-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="53d34-108">Näiteks ei pääse mõned domeenikontrollerid Azure AD Connecti kaudu juurde või tulemüürid [on blokeeritud](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) , peate selle parandama, tagades, et Azure AD Connecti serveri ja kohapealse Active Directory vaheline Ühenduvus töötab õigesti.</span><span class="sxs-lookup"><span data-stu-id="53d34-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="53d34-109">Azure AD Connect server on praegu lavastuse režiimis, mille tulemusena server ei saa parooli hashes-probleemi tõrkeotsinguks, järgige jaotises kirjeldatud juhiseid, mida on kirjeldatud jaotises [tõrkeotsing parooliga sünkroonimisel AZURE ad Connecti sünkroonimine – paroole ei sünkroonita](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="53d34-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="53d34-110">**Parooli Hash sünkroonimine ei tööta mõne kasutaja jaoks**</span><span class="sxs-lookup"><span data-stu-id="53d34-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="53d34-111">Kui märkate, et parooli Hash ei sünkroonita kasutaja jaoks, kasutage probleemi uurimiseks ja lahendamiseks Azure AD ' i ülesande **tõrkeotsingut** .</span><span class="sxs-lookup"><span data-stu-id="53d34-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="53d34-112">Tehke järgmised toimingud.</span><span class="sxs-lookup"><span data-stu-id="53d34-112">Perform the following tasks:</span></span>

    <span data-ttu-id="53d34-113">loomine.</span><span class="sxs-lookup"><span data-stu-id="53d34-113">a.</span></span> [<span data-ttu-id="53d34-114">Viisardis tõrkeotsingu ülesande käivitamine</span><span class="sxs-lookup"><span data-stu-id="53d34-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="53d34-115">b.</span><span class="sxs-lookup"><span data-stu-id="53d34-115">b.</span></span> [<span data-ttu-id="53d34-116">Tõrkeotsingu cmdlet-käsu kasutamine konkreetsel otstarbel parooli räsi sünkroonimise probleemi uurimiseks</span><span class="sxs-lookup"><span data-stu-id="53d34-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="53d34-117">Kohapealne Active Directory User Object on lubatud **kasutaja peab parooli muutma järgmisel sisselogimise** suvandil.</span><span class="sxs-lookup"><span data-stu-id="53d34-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="53d34-118">Kui see suvand on lubatud, määratakse kasutajale ajutine parool ja teil palutakse muuta järgmise sisselogimise parooli.</span><span class="sxs-lookup"><span data-stu-id="53d34-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="53d34-119">Azure AD Connecti ei sünkroonita Azure AD ajutised paroolid.</span><span class="sxs-lookup"><span data-stu-id="53d34-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="53d34-120">Ülaltoodud probleemi lahendamiseks tehke ühte järgmistest toimingutest.</span><span class="sxs-lookup"><span data-stu-id="53d34-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="53d34-121">Paluge kasutajal sisse logida asutusesisesesse rakendusse (nt Windowsi töölauale) ja muuta parooli.</span><span class="sxs-lookup"><span data-stu-id="53d34-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="53d34-122">Uus parool sünkroonitakse Azure AD-ga.</span><span class="sxs-lookup"><span data-stu-id="53d34-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="53d34-123">Kui administraator on kasutaja parooli värskendanud, siis peab kasutaja parooli **muutma järgmisel sisselogimisel parooli vahetama** ja kasutajaga uue parooli ühiskasutusse andma.</span><span class="sxs-lookup"><span data-stu-id="53d34-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="53d34-124">Kohapealne Active Directory kasutaja objekt pole objekti sünkroonimiseks või parooli sünkroonimiseks **õigesti konfigureeritud** .</span><span class="sxs-lookup"><span data-stu-id="53d34-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="53d34-125">Selle probleemi tõrkeotsingu sooritamiseks järgige juhiseid, mis on kirjeldatud jaotises [tõrkeotsing parooli räsi sünkroonimisel AZURE ad Connecti sünkroonimine](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="53d34-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







