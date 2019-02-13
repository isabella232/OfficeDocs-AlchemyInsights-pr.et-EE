---
title: Järelevalve juurdepääsu
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902339"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="56a4b-102">Järelevalve juurdepääsu</span><span class="sxs-lookup"><span data-stu-id="56a4b-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="56a4b-p101">Saavad juurdepääsu kasutajad saavad selle ettevõtte juurdepääsu nõuetele ei vasta. Probleemi lahendamiseks soovitame ühte või mitut järgmistest lahendustest:</span><span class="sxs-lookup"><span data-stu-id="56a4b-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="56a4b-p102">Kui seade on eeldada, et olla kaasatud, nõustada ettevõtte portaali rakendust ja veenduge, et see on ettevõtte portaali kasutaja. Kui seda pole, peaks kasutaja seadet registreerida.</span><span class="sxs-lookup"><span data-stu-id="56a4b-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="56a4b-p103">Minge Azure'i portaal **Intune \> seade vastavust**. **Kuvari** all klõpsake **seadme vastavust**. Saate vaadata oma seadme vastavuse aruandes veendumaks, et kasutaja seade on märgitud vastavuses.</span><span class="sxs-lookup"><span data-stu-id="56a4b-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="56a4b-p104">Minge Azure'i portaal **Intune \> seade vastavust**. Klõpsake jaotises **Halda**ja **poliitika**. Täitmise poliitika loendis kontrollida, et profiil on oma kasutaja seadmele määratud. Kui ühtegi profiili on määratud, siis Intune ei saa kinnitada seadme vastavust oleku.</span><span class="sxs-lookup"><span data-stu-id="56a4b-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="56a4b-114">Muuta kasutaja juurdepääsu määramine.</span><span class="sxs-lookup"><span data-stu-id="56a4b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="56a4b-115">Minge Azure'i portaal **Intune \> juurdepääsu \> poliitika**</span><span class="sxs-lookup"><span data-stu-id="56a4b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="56a4b-116">Valige loendist reeglid</span><span class="sxs-lookup"><span data-stu-id="56a4b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="56a4b-117">Klõpsake suvandit **kasutajad ja rühmad**</span><span class="sxs-lookup"><span data-stu-id="56a4b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="56a4b-p105">Keegi poliitika suunata need lisada **kaasamisloendis** . Tagamaks, et isik on välja jäetud poliitikast, lisada need **välistada** nimekirja.</span><span class="sxs-lookup"><span data-stu-id="56a4b-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="56a4b-120">Loe edasi: [Monitor tingimusjuurdepääsuseadmete kuidas](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="56a4b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

