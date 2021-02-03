---
title: Parooli tagasikirjutamise lubamine Azure AD Connectis
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093351"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="2d5d4-102">Parooli tagasikirjutamise lubamine Azure AD Connectis</span><span class="sxs-lookup"><span data-stu-id="2d5d4-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="2d5d4-103">Selleks et lubada iseteeninduslikku paroolilähtestuse tagasikirjutamist, peate esmalt Azure AD Connectis lubama tagasikirjutamise võimaluse.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="2d5d4-104">Tehke Azure AD Connecti serveri kaudu järgmised toimingud.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="2d5d4-105">Logige sisse Azure AD Connecti serverisse ja käivitage **Azure AD Connecti** konfigureerimisviisard.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="2d5d4-106">Klõpsake lehel **Tere tulemast** nuppu **Konfigureeri**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="2d5d4-107">Lehel **Lisaülesanded** valige **Kohanda sünkroonimissuvandeid** ja seejärel klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="2d5d4-108">Lehel **Loo ühendus Azure AD-ga** sisestage oma Azure’i rentniku üldadministraatori identimisteave ja seejärel klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="2d5d4-109">Filtreerimislehtedel **Ühenda kataloogid** ja **Domeen/OÜ** klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="2d5d4-110">Lehel **Valikulised funktsioonid** märkige valiku **Parooli tagasikirjutamine** kõrval olev kastike ja klõpsake nuppu **Edasi**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="2d5d4-111">Lehel **Konfigureerimiseks valmis** klõpsake nuppu **Konfigureeri** ja oodake, kuni protsess lõpeb.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="2d5d4-112">Kui näete, et konfigureerimine on lõppenud, klõpsake nuppu **Välju**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="2d5d4-113">Kui parooli tagasikirjutamine on Azure AD Connectis lubatud, konfigureerige Azure AD SSPR-i tagasikirjutamine.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="2d5d4-114">SSPR-is parooli tagasikirjutamise lubamiseks tehke järgmised toimingud.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="2d5d4-115">Logige üldadministraatori kontot kasutades sisse Microsoft Azure’i portaali.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="2d5d4-116">Otsige üles **Azure Active Directory** ja valige see, klõpsake valikut **Paroolilähtestus** ning seejärel valikut **Kohapealne integreerimine**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="2d5d4-117">Määrake küsimuse **Soovite paroole tagasi kirjutada oma kohapealsesse kataloogi?** vastuseks **Jah**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="2d5d4-118">Määrake küsimuse **Lubate kasutajatel kontosid lukust avada ilma oma parooli lähtestamata?** vastuseks **Jah**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="2d5d4-119">Kui olete valmis, klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-119">When ready, click **Save**.</span></span>

<span data-ttu-id="2d5d4-120">Lisateavet leiate artiklist [Kuidas lubada Azure Active Directoryil iseteeninduslikku paroolilähtestuse tagasikirjutamist kohapealsesse keskkonda](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="2d5d4-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="2d5d4-121">Kui administraator lähtestab Azure’i portaalis kasutaja parooli ja see on väliskasutaja või parool räsisünkroonitud, kirjutatakse parool tagasi kohapealsesse keskkonda.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="2d5d4-122">See funktsioon nõuab Azure’i Premium-litsentsi (P1 või P2) ja hetkel pole see Office’i haldusportaalis toetatud.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
