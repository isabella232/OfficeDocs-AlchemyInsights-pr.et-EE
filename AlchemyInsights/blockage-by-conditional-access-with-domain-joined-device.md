---
title: Ma saan blokeeritud domeeniga liitunud seadmega tingimisi juurdepääsu tõttu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035723"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="3fc23-102">Ma saan blokeeritud domeeniga liitunud seadmega tingimisi juurdepääsu tõttu</span><span class="sxs-lookup"><span data-stu-id="3fc23-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="3fc23-103">**Väga Soovitatavad tööriistad**</span><span class="sxs-lookup"><span data-stu-id="3fc23-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="3fc23-104">[Seadme registreerimise tõrkeotsija tööriist](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – tööriist, mis aitab tõrkeotsingul kõige levinumaid seadme registreerimise probleeme.</span><span class="sxs-lookup"><span data-stu-id="3fc23-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="3fc23-105">[Seadme registreerimise ühenduvuse skriptimine](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skript, mis aitab tagada, et seade pääseb juurde seadme registreerimise lõpp-punktidele süsteemi konto all.</span><span class="sxs-lookup"><span data-stu-id="3fc23-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="3fc23-106">[AZURE ad Device cleanup script](https://github.com/mzmaili/AzureADDeviceCleanup) – skript, mis võimaldab teil otsida ja hallata aegunud seadmeid teie keskkonnas.</span><span class="sxs-lookup"><span data-stu-id="3fc23-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="3fc23-107">Siin on mõned levinumad põhjused, miks tingimusjuurdepääsu võib nurjuda, kui seade on domeeniga liitunud (hübriid-Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3fc23-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="3fc23-108">**Seadmes pole AZURE ad PRT** -d, peate veenduma, et seadmel on Azure AD esmase värskendamise luba (PRT).</span><span class="sxs-lookup"><span data-stu-id="3fc23-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="3fc23-109">Lisateavet PRT kohta leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="3fc23-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="3fc23-110">Kui soovite kontrollida, kas teil on Azure AD PRT, saate käivitada `dsregcmd/status` seadmes käsu ja kontrollida, kas "AzureAdPrt" võrdub "Jah".</span><span class="sxs-lookup"><span data-stu-id="3fc23-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="3fc23-111">Kui "AzureAdPrt" on "ei", siis kontrollige järgmist.</span><span class="sxs-lookup"><span data-stu-id="3fc23-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="3fc23-112">**Kas teil on väline keskkond AD FS-iga ja see pole kasutajate koduvõrgust** juurdepääsetav: sel juhul veenduge, et teie "usernamemixed" lõpp-punktid on Suhtevõrgu kaudu juurdepääsetavad.</span><span class="sxs-lookup"><span data-stu-id="3fc23-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="3fc23-113">Kui teie AD FS on VPN-i taga, veenduge, et kasutajad ühenduvad VPN-iga ja logige seadmesse uuesti sisse.</span><span class="sxs-lookup"><span data-stu-id="3fc23-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="3fc23-114">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="3fc23-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="3fc23-115">**Kas seadme TPM on vigane ja seetõttu ei saa seadet autentida**: märkige ruut "TPM. msc", et näha, kas TPM-i olek on "valmis".</span><span class="sxs-lookup"><span data-stu-id="3fc23-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="3fc23-116">Kui ei, siis käivitage `dsregcmd/leave` ja laske seadmel uuesti AZURE ad-ga liituda.</span><span class="sxs-lookup"><span data-stu-id="3fc23-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="3fc23-117">Seejärel proovi uuesti.</span><span class="sxs-lookup"><span data-stu-id="3fc23-117">Then, try again.</span></span> <span data-ttu-id="3fc23-118">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="3fc23-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="3fc23-119">**Kasutate kolmanda osapoole identiteedi pakkujat, mis ei toeta WS-Trust protokolli**.</span><span class="sxs-lookup"><span data-stu-id="3fc23-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="3fc23-120">Nagu on kirjeldatud meie dokumentides, ei saa hübriid-Azure AD-liitunud seadmed sel juhul töötada.</span><span class="sxs-lookup"><span data-stu-id="3fc23-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="3fc23-121">Palun tööta oma identiteedi pakkujaga toe saamiseks.</span><span class="sxs-lookup"><span data-stu-id="3fc23-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="3fc23-122">**Kasutajad kasutavad Chrome ' i brauserit, ilma et Windows 10 kontod** või **Office ' i laiendus Chrome ei kasuta automaatselt PRT-ga liitunud või hübriid-AAD-ga ühendatud seadmetes PRT**. see viib tõrkele mis tahes seadmel põhinevate tingimusjuurdepääsu poliitikate korral, kus kuvatakse tõrketeade "registreerimata seade".</span><span class="sxs-lookup"><span data-stu-id="3fc23-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="3fc23-123">Chrome ' i brauseri õigeks kasutamiseks peate installima "Windows 10 Accounts" või "Office ' i laienduse kasutajate Chrome ' i brauseris" SCCM või Intune ' i kaudu.</span><span class="sxs-lookup"><span data-stu-id="3fc23-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="3fc23-124">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="3fc23-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="3fc23-125">Kui laiendust ei saa eemalt tõugata, Teavitage kasutajaid käsitsi installimisest mõnele ülaltoodud laiendist, et pääseda juurde rakendustele, mis jäävad Device-põhise tingimusjuurdepääsu juurde.</span><span class="sxs-lookup"><span data-stu-id="3fc23-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="3fc23-126">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="3fc23-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="3fc23-127">**Seade oli õigesti hübriid AZURE ad liitunud, kuid see on tahtmatult kustutatud või keelatud, kas AZURE ad Connecti või Azure ' i portaalis muudatuste sünkroonimise tõttu**: kui see on nii, siis seadme objekti ei tuvastata enam täielikult ühendatud seadmena, kuigi "AzureAdJoined" ja "PRT" olek kuvatakse seadmes kehtivana.</span><span class="sxs-lookup"><span data-stu-id="3fc23-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="3fc23-128">Selle probleemi lahendamiseks käivitage `dsregcmd/leave` mõjutatud seadmetes ja lubage uuesti AZURE ad.</span><span class="sxs-lookup"><span data-stu-id="3fc23-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="3fc23-129">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="3fc23-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="3fc23-130">Kui teie seadmed on opsüsteemis Windows 10, 1809 Update, VPN-i/pilve puhverserveriga ja vaadake probleeme "AzureAdPrt" olekuga või mis tahes rakenduse SSO probleemiga (Outlook ei Ühenda postkastiga, isegi kui teil oli PRT), veenduge, et teil on see paik [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) või aprilli koondvärskenduses [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , et vältida PRT rikete tegemist.</span><span class="sxs-lookup"><span data-stu-id="3fc23-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















