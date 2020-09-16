---
title: SharePoint Online ' i Termini salvest puuduvad terminid
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750447"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="8c19e-102">BitLockeri krüptimise lubamine Intune ' i abil</span><span class="sxs-lookup"><span data-stu-id="8c19e-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="8c19e-103">Intune Endpoint Protection Policy saab kasutada Windowsi seadmete Boitlocker konfigureerimiseks, nagu on kirjeldatud jaotises: Windows10 (ja uuemad) sätted, et kaitsta seadmeid Intune ' i abil</span><span class="sxs-lookup"><span data-stu-id="8c19e-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="8c19e-104">Peaksite teadma, et paljud uuemad seadmed, kus töötab Windows 10, toetavad automaatset BitLockeri krüptimist, mis käivitatakse MDM-poliitikat rakendamata.</span><span class="sxs-lookup"><span data-stu-id="8c19e-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="8c19e-105">See võib mõjutada poliitika rakendamist, kui vaikesätted pole konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="8c19e-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="8c19e-106">Üksikasjalikumat teavet leiate teemast KKK.</span><span class="sxs-lookup"><span data-stu-id="8c19e-106">See FAQ for more detail.</span></span>


<span data-ttu-id="8c19e-107">KKK   k: millised Windowsis olevad väljaanded toetavad seadme krüptimist lõpp-punkti kaitse poliitika abil?</span><span class="sxs-lookup"><span data-stu-id="8c19e-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="8c19e-108"> V: Intune ' i lõpp-punkti kaitsepoliitika sätted rakendatakse BitLockeri CSP-i kaudu.</span><span class="sxs-lookup"><span data-stu-id="8c19e-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="8c19e-109">BitLockeri CSP ei toeta kõiki väljaandeid ega Windowsi väljaandeid. 
     </span><span class="sxs-lookup"><span data-stu-id="8c19e-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="8c19e-110">Praegu on Windowsi versioonid: Enterprise; Toetatakse haridust, mobiili, mobiilset ettevõtlust ja Professionalit (alates järgust 1809).</span><span class="sxs-lookup"><span data-stu-id="8c19e-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="8c19e-111">K. Kui seade on BitLocker-iga juba krüptitud, kasutades krüptimise meetodi ja šifri tugevuse (XTS-AES-128) sätteid, mis käivitab automaatselt draivi uuesti krüpteerimise uute sätetega.</span><span class="sxs-lookup"><span data-stu-id="8c19e-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="8c19e-112">Vastus. Ei.</span><span class="sxs-lookup"><span data-stu-id="8c19e-112">A: No.</span></span> <span data-ttu-id="8c19e-113">Uute šifri sätete rakendamiseks peab draiv esmalt dekrüptima.</span><span class="sxs-lookup"><span data-stu-id="8c19e-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="8c19e-114">Märkus seadmete registreerimisel autopiloot on automaatne krüptimine, mis ilmneb OOBE ajal ei käivitu kuni Intune poliitika hinnatakse, mis võimaldab poliitikal põhinevad sätted, mida kasutatakse OS-i vaikesätete asemel</span><span class="sxs-lookup"><span data-stu-id="8c19e-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="8c19e-115">K kui seade krüptitakse Intune ' i poliitika rakendamise tõttu, dekrüptitakse see poliitika eemaldamise korral?</span><span class="sxs-lookup"><span data-stu-id="8c19e-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="8c19e-116">A: krüptimise seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimist.</span><span class="sxs-lookup"><span data-stu-id="8c19e-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="8c19e-117">K: Miks Intune ' i nõuetele vastavuse poliitika näitab, et minu seadmel pole "BitLocker enabled", kuid see on?</span><span class="sxs-lookup"><span data-stu-id="8c19e-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="8c19e-118">V: "BitLockeri lubatud" säte Intune ' i nõuetele vastavuse poliitikas kasutab Windowsi seadme terviseohutuse kinnitust (DHA) klienti.</span><span class="sxs-lookup"><span data-stu-id="8c19e-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="8c19e-119">See klient mõõdab ainult seadme olekut alglaadimise ajal.</span><span class="sxs-lookup"><span data-stu-id="8c19e-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="8c19e-120">Nii et kui seadet pole uuesti käivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeeninduse teenusest BitLocker aktiivsena.</span><span class="sxs-lookup"><span data-stu-id="8c19e-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>