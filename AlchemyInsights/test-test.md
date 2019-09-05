---
title: SharePoint Online ' i Terminikauplus puuduvad terminid
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762053"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="5e266-102">BitLockeri krüptimise lubamine Intune ' iga</span><span class="sxs-lookup"><span data-stu-id="5e266-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="5e266-103">Intune lõpp-punkti kaitse poliitika saab konfigureerida Boitlocker krüpteerimise sätted Windowsi seadmete nagu kirjeldatud: Windows10 (ja uuem) sätteid, et kaitsta seadmeid, kasutades Intune</span><span class="sxs-lookup"><span data-stu-id="5e266-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="5e266-104">Peaksite teadma, et paljud uuemad seadmed, mis töötavad Windows 10 toetavad automaatset BitLockeri krüptimist, mis käivitatakse ilma MDM-poliitika rakendamist.</span><span class="sxs-lookup"><span data-stu-id="5e266-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="5e266-105">See võib mõjutada poliitika rakendamist, kui vaikimisi sätted on konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="5e266-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="5e266-106">Üksikasjalikumat infot leiate KKK-st.</span><span class="sxs-lookup"><span data-stu-id="5e266-106">See FAQ for more detail.</span></span>


<span data-ttu-id="5e266-107">KKK  Q: millised Windowsi tugiteenuste seadme krüptimine lõpp-punkti kaitse poliitika abil?</span><span class="sxs-lookup"><span data-stu-id="5e266-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="5e266-108"> A. Intune lõpp-punkti kaitse poliitika sätted rakendatakse BitLockeri CSP abil.</span><span class="sxs-lookup"><span data-stu-id="5e266-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="5e266-109">Kõik väljaanded ega järkude Windows ei toeta BitLockeri CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="5e266-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="5e266-110">Sel ajal Windowsi väljaanded: Enterprise; Haridus, mobiil, mobiilne ettevõtlus ja professionaalne (alates järk 1809) toetatakse.</span><span class="sxs-lookup"><span data-stu-id="5e266-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="5e266-111">Q: kui seade on juba krüpteeritud BitLocker kasutades OPERATSIOONISÜSTEEMI vaikesätteid krüptimismeetod ja šifri tugevus (XTS-AES-128) kohaldab poliitika erinevate sätetega automaatselt käivitab uuesti krüpteerimine draivi uute sätetega?</span><span class="sxs-lookup"><span data-stu-id="5e266-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="5e266-112">A: ei.</span><span class="sxs-lookup"><span data-stu-id="5e266-112">A: No.</span></span> <span data-ttu-id="5e266-113">Uue šifri sätete rakendamiseks tuleb draiv esmalt dekrüptida.</span><span class="sxs-lookup"><span data-stu-id="5e266-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="5e266-114">Märkus seadmete registreerunud autopiloot automaatne krüptimine, mis ilmneb OOBE ajal ei käivitata enne Intune poliitika hinnatakse, mis võimaldab poliitika põhinev sätted kasutatakse asemel OS vaikesätted</span><span class="sxs-lookup"><span data-stu-id="5e266-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="5e266-115">Q kui seade on krüptitud tõttu rakenduse Intune poliitika on dekrüptida, kui see poliitika eemaldatakse?</span><span class="sxs-lookup"><span data-stu-id="5e266-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="5e266-116">A. krüptimisega seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimine.</span><span class="sxs-lookup"><span data-stu-id="5e266-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="5e266-117">Q: Miks Intune vastavuse poliitika näitab, et minu seade ei ole "BitLocker lubatud", kuid see on?</span><span class="sxs-lookup"><span data-stu-id="5e266-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="5e266-118">A: "BitLockeri lubatud" säte Intune vastavuse poliitika kasutab Windows seadme tervise kinnitus (DHA) klient.</span><span class="sxs-lookup"><span data-stu-id="5e266-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="5e266-119">See klient mõõdab ainult seadme oleku boot ajal.</span><span class="sxs-lookup"><span data-stu-id="5e266-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="5e266-120">Nii et kui seadet pole taaskäivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeenus BitLockeri aktiivsest seadmest.</span><span class="sxs-lookup"><span data-stu-id="5e266-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>