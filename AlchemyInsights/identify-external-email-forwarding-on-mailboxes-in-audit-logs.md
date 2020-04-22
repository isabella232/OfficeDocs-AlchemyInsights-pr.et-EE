---
title: Tuvastada väline e-posti suunamine postkastid auditilogi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716456"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c34b8-102">Tuvastada, kui väline e-posti suunamine on konfigureeritud postkastid</span><span class="sxs-lookup"><span data-stu-id="c34b8-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c34b8-103">Kui Microsoft 365 kasutaja konfigureerib välise e-posti suunamine postkasti, tegevust auditeeritakse osana **Set-Mailbox cmdlet-** käsu.</span><span class="sxs-lookup"><span data-stu-id="c34b8-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c34b8-104">Tegevust saate vaadata auditilogi otsingu abil turbe-& Vastavuskeskuses.</span><span class="sxs-lookup"><span data-stu-id="c34b8-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c34b8-105">Logige sisse [Microsoft 365 Security & vastavuse Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c34b8-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c34b8-106">**otsingulehele otsingu** > **auditilogi** .</span><span class="sxs-lookup"><span data-stu-id="c34b8-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c34b8-107">Saate **valida kuupäevavahemiku alguskuupäeva ja** **lõppkuupäeva** väljadel.</span><span class="sxs-lookup"><span data-stu-id="c34b8-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c34b8-108">Kasutajanime ei ole vaja määrata.</span><span class="sxs-lookup"><span data-stu-id="c34b8-108">You don't need to specify a username.</span></span> <span data-ttu-id="c34b8-109">Veenduge, et välja **Tegevused** väärtuseks kuvatakse **kõigi tegevuste tulemused**.</span><span class="sxs-lookup"><span data-stu-id="c34b8-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c34b8-110">Klõpsake suvandit **Otsing**.</span><span class="sxs-lookup"><span data-stu-id="c34b8-110">Click **Search**.</span></span>

<span data-ttu-id="c34b8-111">Tulemuste, klõpsake **filtri tulemused** ja tippige **määratud postkast** tegevuse filter kasti.</span><span class="sxs-lookup"><span data-stu-id="c34b8-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c34b8-112">Valige tulemite auditilogi.</span><span class="sxs-lookup"><span data-stu-id="c34b8-112">Select an audit record in the results.</span></span> <span data-ttu-id="c34b8-113">**Üksikasjade** hüpik, klõpsake **rohkem teavet**.</span><span class="sxs-lookup"><span data-stu-id="c34b8-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c34b8-114">Peate vaatama iga auditi kirje üksikasjad, et teha kindlaks, kas tegevus on seotud e-posti suunamine.</span><span class="sxs-lookup"><span data-stu-id="c34b8-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c34b8-115">**ObjectId**: muudetud postkasti alias väärtus.</span><span class="sxs-lookup"><span data-stu-id="c34b8-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c34b8-116">**Parameetrid**: _forwardingsmtpaddress_ näitab Target e-posti aadress.</span><span class="sxs-lookup"><span data-stu-id="c34b8-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c34b8-117">**Userid**: kasutaja, kes on konfigureeritud e-posti suunamine postkasti **ObjectId** välja.</span><span class="sxs-lookup"><span data-stu-id="c34b8-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c34b8-118">Lisateabe saamiseks vaadake määrates, [kes seadistada e-posti suunamine postkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c34b8-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
