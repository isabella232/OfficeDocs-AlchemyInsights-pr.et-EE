---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908706"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="56c02-102">BitLockeri krüptimise lubamine Intune ' iga</span><span class="sxs-lookup"><span data-stu-id="56c02-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="56c02-103">Intune lõpp-punkti kaitse poliitika saab kasutada BitLockeri Krüptimissätete konfigureerimiseks Windowsi seadmetele.</span><span class="sxs-lookup"><span data-stu-id="56c02-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="56c02-104">Lisateabe saamiseks vaadake [Windows 10 (ja uuemate versioonide) sätteid, et kaitsta seadmeid Intune ' i abil](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="56c02-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="56c02-105">Peaksite teadma, et paljud uuemad seadmed, mis töötavad Windows 10 toetavad automaatset BitLockeri krüptimist, mis käivitatakse ilma MDM-poliitika rakenduseta.</span><span class="sxs-lookup"><span data-stu-id="56c02-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="56c02-106">See võib mõjutada poliitika rakendamist, kui vaikesätted on konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="56c02-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="56c02-107">Üksikasjalikumat Lisateavet leiate järgmistest KKK-st.</span><span class="sxs-lookup"><span data-stu-id="56c02-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="56c02-108">BitLockeri probleemide tõrkeotsingu kohta teabe saamiseks vaadake [Microsofti Intune BitLockeri poliitikate tõrkeotsing](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="56c02-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="56c02-109">**Kkk**</span><span class="sxs-lookup"><span data-stu-id="56c02-109">**FAQ**</span></span>

 <span data-ttu-id="56c02-110">Q: mis väljaanded Windowsi tugiteenuste seadme krüptimine lõpp-punkti kaitse poliitika abil?</span><span class="sxs-lookup"><span data-stu-id="56c02-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="56c02-111">A. Intune lõpp-punkti kaitse poliitika sätted rakendatakse [BitLockeri CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)abil.</span><span class="sxs-lookup"><span data-stu-id="56c02-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="56c02-112">Kõik väljaanded või Windowsi järgud toetavad BitLockeri CSP.</span><span class="sxs-lookup"><span data-stu-id="56c02-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="56c02-113">Sel ajal toetatakse järgmisi Windowsi väljaandeid: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (järk 1809 ja uuem).</span><span class="sxs-lookup"><span data-stu-id="56c02-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="56c02-114">Q: kui seade on juba krüpteeritud BitLocker kasutades OPERATSIOONISÜSTEEMI vaikesätteid krüpteerimismeetod ja šifri tugevus (XTS-AES-128), rakendades poliitika erinevate sätetega automaatselt käivitab uuesti krüpteerimine draivi uute sätetega?</span><span class="sxs-lookup"><span data-stu-id="56c02-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="56c02-115">A: ei.</span><span class="sxs-lookup"><span data-stu-id="56c02-115">A: No.</span></span> <span data-ttu-id="56c02-116">Uue šifri sätete rakendamiseks peab draiv esmalt dekrüpteeritud.</span><span class="sxs-lookup"><span data-stu-id="56c02-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="56c02-117">**Märkus:** Autodele, mis on kaasatud autopiloot, automaatne krüptimine, mis ilmneb OOBE ajal ei käivitata enne Intune poliitika on hinnatud, mis võimaldab poliitikapõhise sätted kasutatakse asemel OS vaikesätted.</span><span class="sxs-lookup"><span data-stu-id="56c02-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="56c02-118">Q: kui seade on krüpteeritud tõttu rakenduse Intune poliitika, kas see dekrüpteeritakse, kui see poliitika eemaldatakse?</span><span class="sxs-lookup"><span data-stu-id="56c02-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="56c02-119">A. krüptimisega seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimine.</span><span class="sxs-lookup"><span data-stu-id="56c02-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="56c02-120">Q: Miks Intune vastavuse poliitika näitab, et minu seadmel pole BitLockeri lubatud, kuigi see on?</span><span class="sxs-lookup"><span data-stu-id="56c02-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="56c02-121">A: "BitLocker lubatud" säte Intune vastavuse poliitika kasutab Windows seadme tervise kinnitus (DHA) klient.</span><span class="sxs-lookup"><span data-stu-id="56c02-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="56c02-122">See klient mõõdab ainult seadme oleku boot ajal.</span><span class="sxs-lookup"><span data-stu-id="56c02-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="56c02-123">Nii et kui seadet pole taaskäivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeenindus BitLockeri aktiivsena.</span><span class="sxs-lookup"><span data-stu-id="56c02-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 