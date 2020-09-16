---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731235"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="53a5e-102">BitLockeri krüptimise lubamine Intune ' i abil</span><span class="sxs-lookup"><span data-stu-id="53a5e-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="53a5e-103">Intune Endpoint Protection Policy saab kasutada BitLockeri krüptimise sätete konfigureerimiseks Windowsi seadmetes.</span><span class="sxs-lookup"><span data-stu-id="53a5e-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="53a5e-104">Lisateavet leiate artiklist [Windows 10 (ja hilisemad) sätted, et kaitsta seadmeid Intune ' i abil](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="53a5e-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="53a5e-105">Peaksite teadma, et paljud uuemad seadmed, kus töötab Windows 10, toetavad automaatset BitLockeri krüptimist, mis käivitatakse MDM-poliitikat rakendamata.</span><span class="sxs-lookup"><span data-stu-id="53a5e-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="53a5e-106">See võib mõjutada poliitika rakendamist, kui vaikesätted pole konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="53a5e-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="53a5e-107">Üksikasjalikumat teavet leiate järgmisest KKK-s.</span><span class="sxs-lookup"><span data-stu-id="53a5e-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="53a5e-108">Lisateavet BitLockeri probleemide tõrkeotsingu kohta leiate teemast [BitLockeri poliitikate tõrkeotsing Microsoft Intune ' is](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="53a5e-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="53a5e-109">**KKK**</span><span class="sxs-lookup"><span data-stu-id="53a5e-109">**FAQ**</span></span>

 <span data-ttu-id="53a5e-110">K: millised Windows ' i versioonid toetavad seadme krüptimist lõpp-punkti kaitse poliitika abil?</span><span class="sxs-lookup"><span data-stu-id="53a5e-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="53a5e-111">V: Intune ' i lõpp-punkti kaitsepoliitika sätted rakendatakse [BITLOCKERI CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)-i kaudu.</span><span class="sxs-lookup"><span data-stu-id="53a5e-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="53a5e-112">BitLockeri CSP ei toeta kõiki Windowsi väljaandeid ega väljaandeid.</span><span class="sxs-lookup"><span data-stu-id="53a5e-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="53a5e-113">Praegu toetatakse järgmisi Windowsi väljaandeid: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (järk 1809 ja uuem versioon).</span><span class="sxs-lookup"><span data-stu-id="53a5e-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="53a5e-114">K. Kui seade on BitLocker-iga juba krüptitud, kasutades krüptimise meetodi ja šifri tugevuse (XTS-AES-128) jaoks mõeldud OS-i vaikesätteid, siis käivitab uue sättega automaatselt draivi uuesti krüptimine.</span><span class="sxs-lookup"><span data-stu-id="53a5e-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="53a5e-115">Vastus. Ei.</span><span class="sxs-lookup"><span data-stu-id="53a5e-115">A: No.</span></span> <span data-ttu-id="53a5e-116">Uue šifri sätete rakendamiseks peab draiv esmalt dekrüptima.</span><span class="sxs-lookup"><span data-stu-id="53a5e-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="53a5e-117">**Märkus:** Kui seadmeid registreeritakse autopiloodiga, siis OOBE ajal ilmnev automaatne krüptimine ei käivitu enne, kui poliitika on hinnanud, mis võimaldab OPERATSIOONISÜSTEEMI vaikesätete asemel kasutada poliitikal põhinevaid sätteid.</span><span class="sxs-lookup"><span data-stu-id="53a5e-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="53a5e-118">K. Kui seade krüptitakse Intune ' i poliitika rakendamise tõttu, dekrüptitakse see poliitika eemaldamise korral?</span><span class="sxs-lookup"><span data-stu-id="53a5e-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="53a5e-119">V: krüptimisega seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimist.</span><span class="sxs-lookup"><span data-stu-id="53a5e-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="53a5e-120">K: Miks Intune ' i nõuetele vastavuse poliitika näitab, et minu seadmel pole BitLockerit lubatud, isegi kui see on nii?</span><span class="sxs-lookup"><span data-stu-id="53a5e-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="53a5e-121">V: Intune ' i nõuetele vastavuse poliitikas säte "BitLocker enabled" kasutab Windowsi seadme terviseohutuse kinnitust (DHA) klienti.</span><span class="sxs-lookup"><span data-stu-id="53a5e-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="53a5e-122">See klient mõõdab ainult seadme olekut alglaadimise ajal.</span><span class="sxs-lookup"><span data-stu-id="53a5e-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="53a5e-123">Nii et kui seadet pole uuesti käivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeeninduse teenusest BitLocker aktiivsena.</span><span class="sxs-lookup"><span data-stu-id="53a5e-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 