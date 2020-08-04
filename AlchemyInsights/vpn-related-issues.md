---
title: VPN-iga seotud probleemid
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554970"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="cd3ff-102">VPN-iga seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="cd3ff-102">VPN related issues</span></span>

<span data-ttu-id="cd3ff-103">Virtuaalse privaatvõrgu ühenduvuse edukas rakendamine MDM-klientidele sõltub juurutatud profiilist, mis vastab õigesti VPN-i infrastruktuuri nõuetele.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="cd3ff-104">Teie uurimisel kasutatavate klientarvutite jaoks sobivate sätete leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="cd3ff-105">Windows 10 ja Windowsi holograafiline seadme sätted Intune ' i abil VPN-ühenduste lisamiseks</span><span class="sxs-lookup"><span data-stu-id="cd3ff-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="cd3ff-106">VPN-i sätete lisamine iOS-i ja iPadOS seadmetes Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cd3ff-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="cd3ff-107">Androidi seadme sätted VPN-i konfigureerimiseks Intune-is</span><span class="sxs-lookup"><span data-stu-id="cd3ff-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="cd3ff-108">VPN-i sätete lisamine opsüsteemis Microsoft Intune (macOS) seadmetes</span><span class="sxs-lookup"><span data-stu-id="cd3ff-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="cd3ff-109">Kui teie VPN-i profiil kasutab serdil põhinevat autentimist, veenduge, et VPN-profiiliga lingitud serdi ja kliendi autentimise serdi profiilid on edukalt juurutatud.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="cd3ff-110">**Levinud probleemid**</span><span class="sxs-lookup"><span data-stu-id="cd3ff-110">**Common Issues**</span></span>

<span data-ttu-id="cd3ff-111">**Juurutasin seadmesse VPN-I profiili. Intune näitab, et see oli edukas, kuid seade ei ühendu VPN-iga.**</span><span class="sxs-lookup"><span data-stu-id="cd3ff-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="cd3ff-112">Edukas olek tähendab seda, et Intune on profiili edukalt juurutanud konfigureeritud kujul.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="cd3ff-113">Kuid need konfiguratsioonid ei pruugi teie võrgu ja/või autentimise nõuetele vastavaks osutuda.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="cd3ff-114">Logige sisse infrastruktuuri ja autentimise teenuse (VPN server ja NPS/RADIUS serveri) kohta lisateabe saamiseks proovitud ühendust.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="cd3ff-115">Logide kogumiseks ja läbivaatamiseks peate võib-olla töötama võrgu infrastruktuuri meeskonnaga või kolmanda osapoole VPN-i tarnijaga.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="cd3ff-116">**Kui Konfigureerin kohandatud VPN-I iOS-I jaoks, pole rakenduse VPN-i funktsioon saadaval.**</span><span class="sxs-lookup"><span data-stu-id="cd3ff-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="cd3ff-117">Rakenduse VPN iOS-i seadmetes Intune ' is on praegu saadaval kindlas teenusepakkujate ja partnerite loendis, kes peavad enne rakenduse VPN-i konfigureerimist täitma ka serdi eeltingimused.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="cd3ff-118">Lisateavet leiate teemast [rakenduse virtuaalse privaatvõrgu (VPN) häälestamine iOS-i/iPadOS seadmete jaoks Intune ' is](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="cd3ff-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="cd3ff-119">Lisateavet kõigi VPN-ühenduse tüüpide kohta Intune ' is leiate artiklist VPN- [profiilide loomine Intune ' i VPN-serveritega ühenduse](https://docs.microsoft.com/intune/vpn-settings-configure)loomiseks.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="cd3ff-120">**iOS on-demand VPN ei käivitu, kui konfigureeritud domeen on juurdepääsetav**</span><span class="sxs-lookup"><span data-stu-id="cd3ff-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="cd3ff-121">Automaatse VPN-i sätete testimiseks seadke järgmised väärtused.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="cd3ff-122">Soovin teha järgmist. **hinnake iga ühenduste katset**</span><span class="sxs-lookup"><span data-stu-id="cd3ff-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="cd3ff-123">Valige, kas soovite ühenduse luua: **vajadusel ühenduse loomine**</span><span class="sxs-lookup"><span data-stu-id="cd3ff-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="cd3ff-124">Kui kasutajad pääsevad juurde järgmistele domeenidele: **Target** *Domain Name*</span><span class="sxs-lookup"><span data-stu-id="cd3ff-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="cd3ff-125">Kui ülaltoodud konfiguratsioon pole edukas, lisage järgmine element.</span><span class="sxs-lookup"><span data-stu-id="cd3ff-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="cd3ff-126">Kui see URL pole kättesaadav, võtke ühendust VPN-iga: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="cd3ff-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>