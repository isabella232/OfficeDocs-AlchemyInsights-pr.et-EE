---
title: Tingimusliku juurdepääsu jälgimine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702899"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a305e-102">Exchange ' i tingimisi juurdepääsu jälgimine</span><span class="sxs-lookup"><span data-stu-id="a305e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a305e-103">Juurdepääsuõigusega kasutajatele antakse teatise meilisõnum, kui need ei vasta teie asutuse juurdepääsu nõuetele.</span><span class="sxs-lookup"><span data-stu-id="a305e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a305e-104">Lahendamiseks soovitame teha ühte või mitut järgmistest lahendustest.</span><span class="sxs-lookup"><span data-stu-id="a305e-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a305e-105">Kui eeldatakse, et seade on registreeritud, Soovitage kasutajal minna ettevõtte portaali rakendusse ja veenduge, et see kuvatakse ettevõtte portaalis.</span><span class="sxs-lookup"><span data-stu-id="a305e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a305e-106">Kui seda ei juhtu, peaks kasutaja seadme registreerima.</span><span class="sxs-lookup"><span data-stu-id="a305e-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a305e-107">Avage Azure ' i portaalis \*\* \> seadme nõuetele vastavuse häälestamine\*\*.</span><span class="sxs-lookup"><span data-stu-id="a305e-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a305e-108">Klõpsake jaotises **kuvar** nuppu **seadme nõuetele vastavus**.</span><span class="sxs-lookup"><span data-stu-id="a305e-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="a305e-109">Vaadake seadme nõuetele vastavuse aruandeid, et veenduda, kas kasutaja seade on märgitud nõuetele vastavaks.</span><span class="sxs-lookup"><span data-stu-id="a305e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a305e-110">Avage Azure ' i portaalis \*\* \> seadme nõuetele vastavuse häälestamine\*\*.</span><span class="sxs-lookup"><span data-stu-id="a305e-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a305e-111">Klõpsake jaotises **haldamine**nuppu **poliitikad**.</span><span class="sxs-lookup"><span data-stu-id="a305e-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="a305e-112">Veenduge, et nõuetele vastavuse poliitikate loendis oleks teie kasutaja seadmele määratud profiil.</span><span class="sxs-lookup"><span data-stu-id="a305e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a305e-113">Kui profiili pole määratud, ei saa Intune kinnitada seadme nõuetele vastavuse olekut.</span><span class="sxs-lookup"><span data-stu-id="a305e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a305e-114">Kasutaja tingimusliku juurdepääsu määramise redigeerimine.</span><span class="sxs-lookup"><span data-stu-id="a305e-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a305e-115">Azure ' i portaalis Avage \*\* \> tingimusjuurdepääsu \> poliitikate häälestamine\*\*</span><span class="sxs-lookup"><span data-stu-id="a305e-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a305e-116">Loendist poliitika valimine</span><span class="sxs-lookup"><span data-stu-id="a305e-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a305e-117">Valige **kasutajad ja rühmad**</span><span class="sxs-lookup"><span data-stu-id="a305e-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a305e-118">Kellegile teatud poliitika suunamiseks lisage need loendisse **kaasa** .</span><span class="sxs-lookup"><span data-stu-id="a305e-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="a305e-119">Kui soovite tagada, et isik on poliitikast välja jäetud, lisage need loendisse **välista** .</span><span class="sxs-lookup"><span data-stu-id="a305e-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a305e-120">Lisateavet leiate [teemast tingimusliku juurdepääsu seadmete jälgimine](https://docs.microsoft.com/intune/conditional-access-exchange-monitor) .</span><span class="sxs-lookup"><span data-stu-id="a305e-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

