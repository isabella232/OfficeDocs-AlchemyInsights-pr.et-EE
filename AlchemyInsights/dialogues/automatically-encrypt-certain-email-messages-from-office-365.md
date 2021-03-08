---
title: Teatud meilisõnumite automaatne krüptimine Office 365 kaudu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524908"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="51bc7-102">Teatud meilisõnumite automaatne krüptimine Office 365 kaudu</span><span class="sxs-lookup"><span data-stu-id="51bc7-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="51bc7-103">Valige [Exchange ' i administreerimiskeskuses](https://outlook.office365.com/ecp/)suvand **mail Flow > reeglid**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="51bc7-104">Klõpsake ikooni **Uus (+)** ja seejärel käsku **Rakenda Office 365 Sõnumite krüptimine ja õiguste kaitse sõnumitele**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="51bc7-105">Sisestage väljale **nimi** reegli nimi (nt *kõigi sõnumite krüptimine*).</span><span class="sxs-lookup"><span data-stu-id="51bc7-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="51bc7-106">Jaotises **Rakenda see reegel, kui** klõpsate nuppu **[Rakenda kõigile sõnumitele]**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="51bc7-107">Klõpsake välja " **tee järgmine** " kõrval nuppu **Vali see**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="51bc7-108">Valige rippmenüüs **RMS** -i Mall käsk **Krüpti** ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="51bc7-109">(Kui seda suvandit ei kuvata, tähendab see seda, et teie leping ei sisalda automaatset krüptimist.</span><span class="sxs-lookup"><span data-stu-id="51bc7-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="51bc7-110">Kuid saate selle lisada!)</span><span class="sxs-lookup"><span data-stu-id="51bc7-110">But you can add it!)</span></span>
7. <span data-ttu-id="51bc7-111">Märkige ruut kontrolli **seda reeglit raskusastme tasemega** ja seejärel valige soovitud tase.</span><span class="sxs-lookup"><span data-stu-id="51bc7-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="51bc7-112">Kui teie ettevõttel on lepingulised kohustused kõigi krüptitud meilisõnumite saatmiseks, soovitame määrata taseme **kõrgeks**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="51bc7-113">Klõpsake jaotises **Valige selle reegli jaoks mudel** nuppu **Jõusta**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="51bc7-114">Valige mis tahes valikuline valik (loendist valikuliste valikute seast, mida saate selles punktis teha, millest paljusid saab lisada lihtsuse vaikesätetega).</span><span class="sxs-lookup"><span data-stu-id="51bc7-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="51bc7-115">Klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="51bc7-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="51bc7-116">Saate alati tagasi tulla ja seda reeglit hiljem redigeerida.</span><span class="sxs-lookup"><span data-stu-id="51bc7-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="51bc7-117">Lisateavet krüptimise reeglite loomise kohta leiate teemast meilisõnumite [krüptimine meilisõnumite krüptimiseks Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="51bc7-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>
