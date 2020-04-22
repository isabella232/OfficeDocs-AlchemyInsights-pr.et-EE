---
title: Tingimusjuurdepääsu jälgimine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713714"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="b1e8a-102">Exchange ' i tingimusjuurdepääsu jälgimine</span><span class="sxs-lookup"><span data-stu-id="b1e8a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="b1e8a-103">Tingimusjuurdepääsu sihtkasutajad saavad meilimeili, kui need ei vasta teie organisatsiooni juurdepääsunõuetele.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b1e8a-104">Probleemi lahendamiseks soovitame ühte või mitut järgmistest lahendustest:</span><span class="sxs-lookup"><span data-stu-id="b1e8a-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="b1e8a-105">Kui eeldatakse, et seade on registreeritud, soovitame kasutajal minna ettevõtteportaali rakendusse ja veenduda, et see kuvatakse ettevõtteportaalis.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b1e8a-106">Kui ei ole, kasutaja peaks registreeruda seade.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="b1e8a-107">Azure ' i portaal minna **Intune \> seadme nõuetele**.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b1e8a-108">Klõpsake **Monitor** jaotises monitor **seadme vastavus**.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="b1e8a-109">Vaadake seadme vastavusaruannet veendumaks, et kasutaja seade on märgitud vastavaks.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="b1e8a-110">Azure ' i portaal minna **Intune \> seadme nõuetele**.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="b1e8a-111">Klõpsake jaotises **Halda** **poliitikad**.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="b1e8a-112">Vastavuse poliitika loendis veenduge, et profiil on määratud teie kasutaja seadmesse.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b1e8a-113">Kui ühtegi profiili pole määratud, ei saa Intune kinnitada seadme vastavusolekut.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="b1e8a-114">Redigeerige kasutaja tingimusjuurdepääsu määramist.</span><span class="sxs-lookup"><span data-stu-id="b1e8a-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="b1e8a-115">Azure ' i portaal minna **Intune \> tingimusjuurdepääsu \> poliitikad**</span><span class="sxs-lookup"><span data-stu-id="b1e8a-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="b1e8a-116">Valige loendist soovitud poliitika</span><span class="sxs-lookup"><span data-stu-id="b1e8a-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="b1e8a-117">Klõpsake valikul **kasutajad ja rühmad**</span><span class="sxs-lookup"><span data-stu-id="b1e8a-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="b1e8a-118">Teatud poliitika kellelegi sihtimiseks lisage need **kaasamisloendisse** .</span><span class="sxs-lookup"><span data-stu-id="b1e8a-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="b1e8a-119">Et tagada, et inimene on poliitikast välja jäetud, lisage need **välisnimekirja** .</span><span class="sxs-lookup"><span data-stu-id="b1e8a-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="b1e8a-120">Loe lähemalt: [Kuidas jälgida tingimusjuurdepääsu seadmed](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="b1e8a-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

