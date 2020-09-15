---
title: Väliste kasutajate lisamine levirühma
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663509"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="2831d-102">Väliste kasutajate lisamine levirühma</span><span class="sxs-lookup"><span data-stu-id="2831d-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="2831d-103">Välise kontakti lisamine levirühma (DG) on kaheastmeline protsess.</span><span class="sxs-lookup"><span data-stu-id="2831d-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="2831d-104">Välise kasutaja jaoks e-posti kontakti loomine.</span><span class="sxs-lookup"><span data-stu-id="2831d-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="2831d-105">Avage halduskeskus lehel **kasutajate**  >  [Kontaktid](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="2831d-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="2831d-106">Valige **Lisa kontakt**.</span><span class="sxs-lookup"><span data-stu-id="2831d-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="2831d-107">Tippige kontakti teave ja klõpsake nuppu **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="2831d-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="2831d-108">Lisa e-posti kontakt oma PEADIREKTORAADIle:</span><span class="sxs-lookup"><span data-stu-id="2831d-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="2831d-109">Avage halduskeskus lehel **rühmade**  >  [rühmad](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="2831d-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="2831d-110">Otsige üles peadirektoraat, kuhu soovite välise kasutaja lisada, ja valige see, et avada dialoogiboks redigeerimine.</span><span class="sxs-lookup"><span data-stu-id="2831d-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="2831d-111">Valige menüü **liikmed** käsk **Kuva kõik ja Halda liikmeid**.</span><span class="sxs-lookup"><span data-stu-id="2831d-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="2831d-112">Valige **Lisa liikmeid**.</span><span class="sxs-lookup"><span data-stu-id="2831d-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="2831d-113">Valige eelmises juhises loodud meilisõnum ja seejärel valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="2831d-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="2831d-114">Kui teie väliskasutajad ei saa pärast järgmisi toiminguid saata meile PEADIREKTORAADIle meilisõnumeid või ei saa sellelt meilisõnumeid vastu võtta, võib see olla see, et peadirektoraat on tähistatud ainult sisemiste kasutajate meilisõnumeid.</span><span class="sxs-lookup"><span data-stu-id="2831d-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="2831d-115">Saate kontrollida seda konfiguratsiooni ja parandada selle juhiseid järgides [siin](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="2831d-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="2831d-116">**Märkus:** Neid juhiseid ei rakendata, kui teie rühma tüüp on "levirühma" asemel "Microsoft 365 Group".</span><span class="sxs-lookup"><span data-stu-id="2831d-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="2831d-117">Kui see on nii, saate välise kasutaja lisada otse rühmale Outlookist.</span><span class="sxs-lookup"><span data-stu-id="2831d-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="2831d-118">[Sellest artiklist](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)leiate üksikasjalikku teavet Microsoft 365 rühmade kohta ning väliskülaliste lisamise juhiseid.</span><span class="sxs-lookup"><span data-stu-id="2831d-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  