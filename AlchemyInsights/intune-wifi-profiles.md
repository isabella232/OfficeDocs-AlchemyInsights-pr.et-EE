---
title: Wi-Fi-profiilide Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555005"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="6253a-102">Wi-Fi-profiilide Intune</span><span class="sxs-lookup"><span data-stu-id="6253a-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="6253a-103">MDM-i klientide Wi-Fi-ühenduvuse edukas rakendamine sõltub õigesti juurutatud profiilist, mis vastab ettevõtte Wi-Fi infrastruktuuri nõuetele.</span><span class="sxs-lookup"><span data-stu-id="6253a-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="6253a-104">Uuritud klientarvutite vastavate sätete läbivaatamiseks lugege järgmisi teemasid.</span><span class="sxs-lookup"><span data-stu-id="6253a-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="6253a-105">Wi-Fi-sätete lisamine Androidi kasutavatele seadmetele Microsoft Intune ' is</span><span class="sxs-lookup"><span data-stu-id="6253a-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="6253a-106">Wi-Fi-sätete lisamine Android Enterprise ' i jaoks mõeldud ja täielikult hallatavatele seadmetele Microsoft Intune ' is</span><span class="sxs-lookup"><span data-stu-id="6253a-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="6253a-107">Wi-Fi-sätete lisamine iOS-i ja iPadOS seadmete jaoks Microsoft Intune ' is</span><span class="sxs-lookup"><span data-stu-id="6253a-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="6253a-108">Wi-Fi-sätete lisamine Windows 10 ja uuemate seadmete jaoks Intune ' is</span><span class="sxs-lookup"><span data-stu-id="6253a-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="6253a-109">Windowsi seadmetes Wi-Fi-sätete importimine Intune ' is</span><span class="sxs-lookup"><span data-stu-id="6253a-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="6253a-110">**Levinud probleemid**</span><span class="sxs-lookup"><span data-stu-id="6253a-110">**Common Issues**</span></span>

<span data-ttu-id="6253a-111">**Juurutan Wi-Fi-profiili, mis sõltub Wi-Fi-profiilis määratud kasutatavast serdist. Konfiguratsiooni profiilid kuvatakse siiski tõrke olek.**</span><span class="sxs-lookup"><span data-stu-id="6253a-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="6253a-112">Kontrollige, kas teie seade sai serdi kätte.</span><span class="sxs-lookup"><span data-stu-id="6253a-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="6253a-113">Tehke Intune ' is valik **kõik seadmed** ja valige seade > **seadme konfiguratsioon**.</span><span class="sxs-lookup"><span data-stu-id="6253a-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="6253a-114">Kontrollige, kas kõik oodatud profiilid on loendis ja edukas olekus.</span><span class="sxs-lookup"><span data-stu-id="6253a-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="6253a-115">Kui teie sertide tarneahelas on vaheserdid, siis veenduge, et Androidi profiilis oleks need juurutatud Androidi seadmetes.</span><span class="sxs-lookup"><span data-stu-id="6253a-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="6253a-116">Serdi oleku kontrollimiseks valige **seadme konfiguratsiooni**  >  **profiilid**  >  **Android Kesktase ca**  >  **Atribuudid**  >  **usaldusväärsed serdid**.</span><span class="sxs-lookup"><span data-stu-id="6253a-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="6253a-117">Kui kuvatakse endiselt tõrked, vaadake jaotist protseduurid ja tõrkeotsing.</span><span class="sxs-lookup"><span data-stu-id="6253a-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="6253a-118">Lisateavet leiate teemast [Microsoft Intune ' i SCEP serdi profiilide tõrkeotsingu ülevaade](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="6253a-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="6253a-119">**Juurutasin seadmes Wi-Fi-profiili. Intune näitab, et see oli edukas, kuid seade ei Ühenda Wi-Fi-võrguga.**</span><span class="sxs-lookup"><span data-stu-id="6253a-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="6253a-120">Edukas olek tähendab seda, et Intune on profiili edukalt juurutanud konfigureeritud kujul.</span><span class="sxs-lookup"><span data-stu-id="6253a-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="6253a-121">Kuid need konfiguratsioonid ei pruugi teie võrgu ja/või autentimise nõuetele vastavaks osutuda.</span><span class="sxs-lookup"><span data-stu-id="6253a-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="6253a-122">Proovitud ühenduse kohta leiate lisateavet teemast logid sisse infrastruktuuri ja autentimise teenuses (Wi-Fi-pääsupunkti kontrolleri ja NPS/RADIUS serveri kaudu).</span><span class="sxs-lookup"><span data-stu-id="6253a-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="6253a-123">Logide kogumiseks ja läbivaatamiseks peate võib-olla töötama võrgu infrastruktuuri meeskonnaga või muu tootja WiFi-tarnijaga.</span><span class="sxs-lookup"><span data-stu-id="6253a-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>