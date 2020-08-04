---
title: Kliendi autentimise serdi juurutamise tõrkeotsing
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555002"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="0611c-102">Kliendi autentimise serdi juurutamise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="0611c-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="0611c-103">Intune ' i NDES/SCEP ja PKCS/PFX-i kliendi sertide profiile kasutatakse tavaliselt koos muude profiilidega (nt WiFi, VPN ja meiliaadress), et kasutajad saaksid autentida ettevõtte ressursse.</span><span class="sxs-lookup"><span data-stu-id="0611c-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="0611c-104">Kui need profiili tüübid on lingitud kliendi serdi profiiliga, sõltub selle profiili edukas rakendamine.</span><span class="sxs-lookup"><span data-stu-id="0611c-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="0611c-105">Kliendi serdi profiili algse infrastruktuuri häälestus ja seotud konfiguratsioon nõuavad sageli tõrkeotsingut.</span><span class="sxs-lookup"><span data-stu-id="0611c-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="0611c-106">Üksikasjalikud juhised NDES konnektori edukaks häälestamiseks ja tõrkeotsingu juhised serdi juurutusega seotud probleemide isoleerimiseks leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="0611c-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="0611c-107">Konfigureeri infrastruktuur, et toetada SCEP Intune ' i abil</span><span class="sxs-lookup"><span data-stu-id="0611c-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="0611c-108">Microsoft Intune ' i SCEP serdi profiilide tõrkeotsingu ülevaade</span><span class="sxs-lookup"><span data-stu-id="0611c-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="0611c-109">Kasutage konfiguratsiooni kinnitamiseks viidatud PowerShelli skripte.</span><span class="sxs-lookup"><span data-stu-id="0611c-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="0611c-110">Lisateavet leiate artiklist [Intune ' i serdi konnektori kinnitamise skriptid](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="0611c-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="0611c-111">**Muud levinud probleemid**</span><span class="sxs-lookup"><span data-stu-id="0611c-111">**Other common issues**</span></span>

<span data-ttu-id="0611c-112">**Kui proovin installida Intune ' i serdi konnektori NDES konnektori serverisse, kuvatakse teade "serdi taotluses olevat parooli ei saa kontrollida. Võimalik, et seda on juba kasutatud. Hankige selle päringuga esitamiseks uus parool. "**</span><span class="sxs-lookup"><span data-stu-id="0611c-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="0611c-113">See sõnum tähendab, et peate käivitama serdi konnektori installi administraatorina.</span><span class="sxs-lookup"><span data-stu-id="0611c-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="0611c-114">Mõnes keskkonnas peavad Intune ' i serdiga serverid kasutama Intune ' iga ühenduse loomiseks puhverserverit ja seega peab serdi konnektor kasutama puhverserverit.</span><span class="sxs-lookup"><span data-stu-id="0611c-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="0611c-115">Mõnel juhul ignoreerib NDES konnektor konfigureeritud puhverserveri sätteid ja võib olla vajalik puhverserveri sätete konfigureerimine LocalSystem turbe kontekstis.</span><span class="sxs-lookup"><span data-stu-id="0611c-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="0611c-116">Lahenduseks on Internet Exploreri käivitamine SÜSTEEMIna ja puhverserveri konfigureerimine IE-s.</span><span class="sxs-lookup"><span data-stu-id="0611c-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="0611c-117">Pärast Intune Connector Service ' i taaskäivitamist loob NDES konnektor Intune ' i.</span><span class="sxs-lookup"><span data-stu-id="0611c-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="0611c-118">**NDES ei saa kasutaja seadmeid enam SCEP sertidest.**</span><span class="sxs-lookup"><span data-stu-id="0611c-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="0611c-119">On võimalik, et NDES serverile väljastatud kliendi autentimine, mis on määratud NDES konnektori installimisel, on aegunud või on puudu.</span><span class="sxs-lookup"><span data-stu-id="0611c-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="0611c-120">Lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="0611c-120">To resolve:</span></span> 
 
1. <span data-ttu-id="0611c-121">Desinstallige NDES konnektor.</span><span class="sxs-lookup"><span data-stu-id="0611c-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="0611c-122">Kasutage järgmisi andmeid uue kliendi autentimise või serveri autentimise serdi taotlemiseks.</span><span class="sxs-lookup"><span data-stu-id="0611c-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="0611c-123">Teema nimi: CN = väline FQDN</span><span class="sxs-lookup"><span data-stu-id="0611c-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="0611c-124">Teema alternatiivne nimi (mõlemad on nõutavad): DNS = väline FQDN, DNS = sisemine FQDN</span><span class="sxs-lookup"><span data-stu-id="0611c-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="0611c-125">Installige NDES konnektor uuesti uue serdiga.</span><span class="sxs-lookup"><span data-stu-id="0611c-125">Reinstall the NDES connector with the new certificate.</span></span>