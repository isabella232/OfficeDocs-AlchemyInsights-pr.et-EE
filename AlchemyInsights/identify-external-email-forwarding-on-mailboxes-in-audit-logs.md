---
title: Väliste meilisõnumite edasisaatmise tuvastamine auditi logide postkastides
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696293"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="aaaf8-102">Tuvastamine, kui väline meilisõnumite edasisaatmine on konfigureeritud postkastides</span><span class="sxs-lookup"><span data-stu-id="aaaf8-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="aaaf8-103">Kui Microsoft 365 kasutaja konfigureerib välise meili edasisaatmise postkastis, auditeeritakse tegevust cmdlet **-käsu Set-Mailbox** osana.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="aaaf8-104">Auditilogi abil saate vaadata tegevust turbe & vastavuskontrolli keskuses.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="aaaf8-105">Logige sisse [Microsoft 365 turbe & nõuetele vastavuse keskuses](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="aaaf8-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="aaaf8-106">Avage leht **Otsingu**  >  **auditilogi otsing** .</span><span class="sxs-lookup"><span data-stu-id="aaaf8-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="aaaf8-107">Valige väljadel **Alguskuupäev** ja **lõppkuupäev** kuupäevavahemik.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="aaaf8-108">Te ei pea kasutajanime määrama.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-108">You don't need to specify a username.</span></span> <span data-ttu-id="aaaf8-109">Veenduge, et väli **Tegevused** oleks seatud **kõigi tegevuste tulemite kuvamiseks**.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="aaaf8-110">Klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-110">Click **Search**.</span></span>

<span data-ttu-id="aaaf8-111">Klõpsake tulemites nuppu **Filtreeri tulemid** ja tippige väljale tegevuse filter **väärtus Set-postkast** .</span><span class="sxs-lookup"><span data-stu-id="aaaf8-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="aaaf8-112">Valige tulemites auditi kirje.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-112">Select an audit record in the results.</span></span> <span data-ttu-id="aaaf8-113">Klõpsake hüpik **üksikasjad** nuppu **veel teavet**.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="aaaf8-114">Peate iga auditi kirje üksikasju uurima, et teha kindlaks, kas tegevus on seotud meilisõnumite edasisaatmisega.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="aaaf8-115">**ObjectId**: muudetud postkasti pseudonüümi väärtus.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="aaaf8-116">**Parameetrid**: _ForwardingSmtpAddress_ tähistab TARGETi meiliaadressi.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="aaaf8-117">**Kasutajanimi**: kasutaja, kes konfigureeris meilisõnumite edasisaatmise väljal **ObjectId** postkastis.</span><span class="sxs-lookup"><span data-stu-id="aaaf8-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="aaaf8-118">Lisateavet leiate teemast [postkasti jaoks meili edasisaatmise häälestamine](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="aaaf8-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
