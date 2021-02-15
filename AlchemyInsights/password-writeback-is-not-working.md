---
title: Parooli tagasikirjutusega ei tööta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243363"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="56b45-102">Parooli tagasikirjutusega ei tööta</span><span class="sxs-lookup"><span data-stu-id="56b45-102">Password Writeback is not working</span></span>

<span data-ttu-id="56b45-103">**Mul on probleeme parooli tagasikirjutusega konfigureerimisega**</span><span class="sxs-lookup"><span data-stu-id="56b45-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="56b45-104">Salasõna tagasikirjutusega on esmaklassiline funktsioon.</span><span class="sxs-lookup"><span data-stu-id="56b45-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="56b45-105">Veenduge, et mõistate litsentsimise nõudeid.</span><span class="sxs-lookup"><span data-stu-id="56b45-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="56b45-106">Teie ettevõttes peab olema vähemalt ühe litsentsiga määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="56b45-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="56b45-107">**Ainult pilveteenuse kasutajad** – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid</span><span class="sxs-lookup"><span data-stu-id="56b45-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="56b45-108">**Pilv ja/või kohapealsed kasutajad** – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="56b45-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="56b45-109">Lisateavet litsentsimise nõuete kohta leiate teemast [AZURE ad iseteeninduse parooli lähtestamise litsentsimise nõuded](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="56b45-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="56b45-110">Teil on vähemalt ühe administraatori konto ning ühe vastava litsentsiga kasutajakonto.</span><span class="sxs-lookup"><span data-stu-id="56b45-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="56b45-111">Peate ühendama Azure AD Connecti esmase domeenikontrolleri Emulaatoriga tagasikirjutusega töötamiseks.</span><span class="sxs-lookup"><span data-stu-id="56b45-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="56b45-112">Saate konfigureerida Azure AD Connecti kasutama esmast domeenikontrollerit, paremklõpsates Active Directory sünkroonimise konnektori **atribuute** ja valides seejärel käsu **Konfigureeri kausta partitsioonid**.</span><span class="sxs-lookup"><span data-stu-id="56b45-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="56b45-113">Sealt otsige üles jaotis **domeenikontrolleri ühenduste sätted** ja märkige ruut nimega **ainult eelistatud domeenikontrollerid**.</span><span class="sxs-lookup"><span data-stu-id="56b45-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="56b45-114">Kui eelistatud DC pole PDC-emulaator, jääb Azure AD Connecti jaoks endiselt välja PDC parooli tagasikirjutusega.</span><span class="sxs-lookup"><span data-stu-id="56b45-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="56b45-115">Parooli lähtestamine on teie rentniku jaoks konfigureeritud ja lubatud.</span><span class="sxs-lookup"><span data-stu-id="56b45-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="56b45-116">Lisateavet leiate teemast [kasutajatele Azure ' i reklaami paroolide lähtestamise lubamine](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="56b45-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="56b45-117">Veenduge, et administraatorikonto, mida kasutatakse parooli tagasikirjutusega lubamiseks, on pilveteenuse administraatorikonto (loodud Azure AD-s, mis pole kohapealne AD)</span><span class="sxs-lookup"><span data-stu-id="56b45-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="56b45-118">Teil on ühe või mitme metsaga AD kohapealne juurutus, kus töötab Windows Server 2008 R2, Windows Server 2012 või Windows Server 2012 R2 uusimate hoolduspaketid installitud</span><span class="sxs-lookup"><span data-stu-id="56b45-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="56b45-119">Teil on installitud Azure AD Connecti tööriist ja olete valmis oma reklaami keskkonna sünkroonimiseks pilve.</span><span class="sxs-lookup"><span data-stu-id="56b45-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="56b45-120">Enne parooli tagasikirjutusega katsetamist veenduge, et täidate Azure AD Connecti kaudu nii AD kui ka Azure AD-st täieliku importimise ja täieliku sünkroonimise.</span><span class="sxs-lookup"><span data-stu-id="56b45-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="56b45-121">Lisateavet leiate artiklist [AZURE ad Connecti täielik sünkroonimine ja täielik importimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="56b45-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="56b45-122">**Mul on probleem parooliga tagasikirjutusega ühenduvusega**</span><span class="sxs-lookup"><span data-stu-id="56b45-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="56b45-123">[AZURE ad Connecti](https://www.microsoft.com/download/details.aspx?id=47594) uusima versiooni allalaadimine ja lubamine</span><span class="sxs-lookup"><span data-stu-id="56b45-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="56b45-124">Tulemüüri konfigureerimine: Azure AD Connecti tööriist (1.1.443 ja ülal) vajab **VÄLJAMINEVA https** -i juurdepääsu:</span><span class="sxs-lookup"><span data-stu-id="56b45-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="56b45-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="56b45-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="56b45-126">ServiceBus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="56b45-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="56b45-127">Lubada, et idle ühendused püsivad vähemalt 2-3 minutit.</span><span class="sxs-lookup"><span data-stu-id="56b45-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="56b45-128">**Mul on endiselt probleeme parooliga tagasikirjutusega**</span><span class="sxs-lookup"><span data-stu-id="56b45-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="56b45-129">Kui teil on endiselt probleeme, proovige keelata ja uuesti lubada parooli tagasikirjutusega teenus Azure AD Connecti tööriistas</span><span class="sxs-lookup"><span data-stu-id="56b45-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="56b45-130">Lisateavet leiate teemast [parooli tagasikirjutusega keelamine ja uuesti lubamine](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="56b45-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
