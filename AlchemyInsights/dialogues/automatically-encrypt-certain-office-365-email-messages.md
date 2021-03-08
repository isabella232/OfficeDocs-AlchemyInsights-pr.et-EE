---
title: Teatud Office ' i 365 meilisõnumite automaatne krüptimine
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524896"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="ecfdb-102">Teatud Office ' i 365 meilisõnumite automaatne krüptimine</span><span class="sxs-lookup"><span data-stu-id="ecfdb-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="ecfdb-103">Saate automaatselt krüptida sõnumeid, mida kasutajad saavad teatud välistele inimestele või organisatsioonidele saata.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="ecfdb-104">Selleks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="ecfdb-105">Valige [Exchange ' i administreerimiskeskuses](https://outlook.office365.com/ecp/)suvand **mail Flow > reeglid**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="ecfdb-106">Klõpsake ikooni **Uus (+)** ja seejärel käsku **Rakenda Office 365 Sõnumite krüptimine ja õiguste kaitse sõnumitele**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="ecfdb-107">Sisestage väljale **nimi** reegli nimi (nt *DrToniRamos@gmail.com saadetud sõnumite krüptimine*).</span><span class="sxs-lookup"><span data-stu-id="ecfdb-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="ecfdb-108">Jaotises **Rakenda see reegel, kui** valite **adressaadi > on see inimene**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="ecfdb-109">Valige aknas **liikmete valimine** selle inimese nimi, kellele soovite krüptimise reegli rakendada, ja klõpsake siis nuppu **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="ecfdb-110">Kui olete kasutajate lisamise lõpetanud, klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="ecfdb-111">Klõpsake välja " **tee järgmine** " kõrval nuppu **Vali see**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="ecfdb-112">Valige rippmenüüs **RMS** -i Mall käsk **Krüpti** ja seejärel klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="ecfdb-113">(Kui seda suvandit ei kuvata, tähendab see seda, et teie leping ei sisalda automaatset krüptimist.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="ecfdb-114">Kuid saate selle lisada!)</span><span class="sxs-lookup"><span data-stu-id="ecfdb-114">But you can add it!)</span></span>
9. <span data-ttu-id="ecfdb-115">Valige mis tahes valikuline valik (loendist valikuliste valikute seast, mida saate selles punktis teha, millest paljusid saab lisada lihtsuse vaikesätetega).</span><span class="sxs-lookup"><span data-stu-id="ecfdb-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="ecfdb-116">Klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ecfdb-117">Saate alati tagasi tulla ja seda reeglit hiljem redigeerida.</span><span class="sxs-lookup"><span data-stu-id="ecfdb-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="ecfdb-118">Lisateavet krüptimise reeglite loomise kohta leiate teemast meilisõnumite [krüptimine Office 365 meilisõnumite krüptimiseks](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="ecfdb-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

