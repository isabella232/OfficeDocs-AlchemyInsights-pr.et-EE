---
title: Office 365 meilisõnumite automaatne krüptimine teatud domeenidele saadetavate meilisõnumite jaoks
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524872"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="8e9de-102">Office 365 meilisõnumite automaatne krüptimine teatud domeenidele saadetavate meilisõnumite jaoks</span><span class="sxs-lookup"><span data-stu-id="8e9de-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="8e9de-103">Valige [Exchange ' i administreerimiskeskuses](https://outlook.office365.com/ecp/)suvand **mail Flow > reeglid**.</span><span class="sxs-lookup"><span data-stu-id="8e9de-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="8e9de-104">Klõpsake ikooni **Uus (+)** ja seejärel käsku **Rakenda Office 365 Sõnumite krüptimine ja õiguste kaitse sõnumitele**.</span><span class="sxs-lookup"><span data-stu-id="8e9de-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="8e9de-105">Sisestage väljale **nimi** reegli nimi (nt *contoso.com saadetud sõnumite krüptimine*).</span><span class="sxs-lookup"><span data-stu-id="8e9de-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="8e9de-106">**Kui olete selle reegli rakendanud**, valige **adressaadi > Domeen**.</span><span class="sxs-lookup"><span data-stu-id="8e9de-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="8e9de-107">Sisestage domeeni nimi (nt **contoso.com**).</span><span class="sxs-lookup"><span data-stu-id="8e9de-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="8e9de-108">Klõpsake ikooni **Add (+) (+)** ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="8e9de-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="8e9de-109">Klõpsake välja " **tee järgmine** " kõrval nuppu **Vali see**.</span><span class="sxs-lookup"><span data-stu-id="8e9de-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="8e9de-110">Valige rippmenüüs **RMS** -i Mall käsk **Krüpti** ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="8e9de-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="8e9de-111">(Kui seda suvandit ei kuvata, tähendab see seda, et teie leping ei sisalda automaatset krüptimist.</span><span class="sxs-lookup"><span data-stu-id="8e9de-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="8e9de-112">Kuid saate selle lisada!)</span><span class="sxs-lookup"><span data-stu-id="8e9de-112">But you can add it!)</span></span>
9. <span data-ttu-id="8e9de-113">Valige mis tahes valikuline valik (loendist valikuliste valikute seast, mida saate selles punktis teha, millest paljusid saab lisada lihtsuse vaikesätetega).</span><span class="sxs-lookup"><span data-stu-id="8e9de-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="8e9de-114">Klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="8e9de-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8e9de-115">Saate alati tagasi tulla ja seda reeglit hiljem redigeerida.</span><span class="sxs-lookup"><span data-stu-id="8e9de-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="8e9de-116">Lisateavet krüptimise reeglite loomise kohta leiate teemast meilisõnumite [krüptimine meilisõnumite krüptimiseks Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="8e9de-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>