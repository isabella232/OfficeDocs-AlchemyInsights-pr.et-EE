---
title: Väliste kasutajate lisamine levirühma
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737869"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="d74b2-102">Väliste kasutajate lisamine levirühma</span><span class="sxs-lookup"><span data-stu-id="d74b2-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="d74b2-103">Välise kontakti lisamine levirühma (DG) on kaheastmeline protsess:</span><span class="sxs-lookup"><span data-stu-id="d74b2-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="d74b2-104">Looge väline kasutaja e-posti Kontakt:</span><span class="sxs-lookup"><span data-stu-id="d74b2-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="d74b2-105">Minge administreerimiskeskuses **kasutajate** > [kontaktide](https://admin.microsoft.com/adminportal/home#/Contact) lehele.</span><span class="sxs-lookup"><span data-stu-id="d74b2-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="d74b2-106">Valige **Lisa kontakt**.</span><span class="sxs-lookup"><span data-stu-id="d74b2-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="d74b2-107">Tippige kontakti teave ja valige käsk **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="d74b2-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="d74b2-108">Lisage e-posti kontakt oma peadirektoraadile:</span><span class="sxs-lookup"><span data-stu-id="d74b2-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="d74b2-109">Minge administreerimiskeskuses lehele **rühmade** > [grupid](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="d74b2-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="d74b2-110">Leidke peadirektoraat, kuhu soovite välise kasutaja lisada, ja valige see redigeerimisdialoogi avamiseks.</span><span class="sxs-lookup"><span data-stu-id="d74b2-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="d74b2-111">Vahekaardil **liikmed** valige **Kuva kõik ja Halda liikmeid**.</span><span class="sxs-lookup"><span data-stu-id="d74b2-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="d74b2-112">Valige **Lisa liikmeid**.</span><span class="sxs-lookup"><span data-stu-id="d74b2-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="d74b2-113">Valige eelmises etapis loodud e-posti kontakt ja seejärel valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="d74b2-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="d74b2-114">Kui pärast nende juhiste järgimist ei saa teie välised kasutajad saata e-kirju peadirektoraadile või ei saa sellest e-kirju, võib peadirektoraat olla märgistatud ainult sisemiste kasutajate meilide lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="d74b2-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="d74b2-115">Saate seda konfiguratsiooni kontrollida ja parandada juhiste järgi [siin](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="d74b2-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="d74b2-116">**Märkus:** Need juhised ei kehti, kui teie rühma tüüp on "Office 365 rühma" asemel "levirühm."</span><span class="sxs-lookup"><span data-stu-id="d74b2-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="d74b2-117">Kui see on nii, saate lisada välise kasutaja otse rühma Outlook.</span><span class="sxs-lookup"><span data-stu-id="d74b2-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="d74b2-118">Üksikasjalik teave Office 365 gruppide kohta, samuti juhised väliste külaliste lisamiseks leiate [sellest artiklist](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="d74b2-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  