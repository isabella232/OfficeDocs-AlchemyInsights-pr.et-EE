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
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538737"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="6b773-102">Järelevalve juurdepääsu Exchange</span><span class="sxs-lookup"><span data-stu-id="6b773-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="6b773-103">Saavad juurdepääsu kasutajad saavad selle ettevõtte juurdepääsu nõuetele ei vasta.</span><span class="sxs-lookup"><span data-stu-id="6b773-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6b773-104">Probleemi lahendamiseks soovitame ühte või mitut järgmistest lahendustest:</span><span class="sxs-lookup"><span data-stu-id="6b773-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="6b773-105">Kui seade on eeldada, et olla kaasatud, nõustada ettevõtte portaali rakendust ja veenduge, et see on ettevõtte portaali kasutaja.</span><span class="sxs-lookup"><span data-stu-id="6b773-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6b773-106">Kui seda pole, peaks kasutaja seadet registreerida.</span><span class="sxs-lookup"><span data-stu-id="6b773-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="6b773-107">Minge Azure'i portaal **Intune \> seade vastavust**.</span><span class="sxs-lookup"><span data-stu-id="6b773-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6b773-108">**Kuvari** all klõpsake **seadme vastavust**.</span><span class="sxs-lookup"><span data-stu-id="6b773-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="6b773-109">Saate vaadata oma seadme vastavuse aruandes veendumaks, et kasutaja seade on märgitud vastavuses.</span><span class="sxs-lookup"><span data-stu-id="6b773-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="6b773-110">Minge Azure'i portaal **Intune \> seade vastavust**.</span><span class="sxs-lookup"><span data-stu-id="6b773-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="6b773-111">Klõpsake jaotises **Halda**ja **poliitika**.</span><span class="sxs-lookup"><span data-stu-id="6b773-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="6b773-112">Täitmise poliitika loendis kontrollida, et profiil on oma kasutaja seadmele määratud.</span><span class="sxs-lookup"><span data-stu-id="6b773-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6b773-113">Kui ühtegi profiili on määratud, siis Intune ei saa kinnitada seadme vastavust oleku.</span><span class="sxs-lookup"><span data-stu-id="6b773-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="6b773-114">Muuta kasutaja juurdepääsu määramine.</span><span class="sxs-lookup"><span data-stu-id="6b773-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="6b773-115">Minge Azure'i portaal **Intune \> juurdepääsu \> poliitika**</span><span class="sxs-lookup"><span data-stu-id="6b773-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="6b773-116">Valige loendist reeglid</span><span class="sxs-lookup"><span data-stu-id="6b773-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="6b773-117">Klõpsake suvandit **kasutajad ja rühmad**</span><span class="sxs-lookup"><span data-stu-id="6b773-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="6b773-118">Keegi poliitika suunata need lisada **kaasamisloendis** .</span><span class="sxs-lookup"><span data-stu-id="6b773-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="6b773-119">Tagamaks, et isik on välja jäetud poliitikast, lisada need **välistada** nimekirja.</span><span class="sxs-lookup"><span data-stu-id="6b773-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="6b773-120">Loe edasi: [Monitor tingimusjuurdepääsuseadmete kuidas](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="6b773-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

