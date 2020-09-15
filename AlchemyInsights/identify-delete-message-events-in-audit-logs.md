---
title: Tuvasta sõnumi sündmuste kustutamine auditi logides
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696509"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="f800f-102">Kustutatud meilisõnumite auditi logid</span><span class="sxs-lookup"><span data-stu-id="f800f-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="f800f-103">Alates jaanuarist 2019 on Microsoft vaikimisi Postkasti auditilogi sisse lülitanud.</span><span class="sxs-lookup"><span data-stu-id="f800f-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="f800f-104">Vastasel juhul peate kindla kasutaja jaoks sõnumite kustutamise üle vaatamiseks käsitsi lubama toimingute kustutamise.</span><span class="sxs-lookup"><span data-stu-id="f800f-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="f800f-105">Kui postkasti auditi logimine on teie asutuse või konkreetse kasutaja jaoks juba lubatud, järgige alltoodud juhiseid.</span><span class="sxs-lookup"><span data-stu-id="f800f-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="f800f-106">Logige sisse [Microsoft 365 turbe & nõuetele vastavuse keskuses](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="f800f-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="f800f-107">Klõpsake nuppu **Otsing ja juurdlus** ning valige **auditilogi otsing**.</span><span class="sxs-lookup"><span data-stu-id="f800f-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="f800f-108">Valige väljadel **Alguskuupäev** ja **lõppkuupäev** kuupäevavahemik.</span><span class="sxs-lookup"><span data-stu-id="f800f-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="f800f-109">Määrake kasutaja kasutajanimi, mida soovite uurida (üksuste kustutanud kasutaja).</span><span class="sxs-lookup"><span data-stu-id="f800f-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="f800f-110">Valige väljal **Tegevused** **kaust** kustutatud ja **teisaldatud sõnumid kausta Kustutatud üksused**.</span><span class="sxs-lookup"><span data-stu-id="f800f-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="f800f-111">Klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="f800f-111">Click **Search**.</span></span>

<span data-ttu-id="f800f-112">Valige tulemites auditi kirje.</span><span class="sxs-lookup"><span data-stu-id="f800f-112">In the results, select an audit record.</span></span> <span data-ttu-id="f800f-113">Klõpsake hüpik üksikasjad nuppu **veel teavet**.</span><span class="sxs-lookup"><span data-stu-id="f800f-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f800f-114">Väljal **AffectedItems** kuvatakse Lisateave kustutatud üksuse kohta (nt üksuse teemarida ja üksuse asukoht, kui see kustutati).</span><span class="sxs-lookup"><span data-stu-id="f800f-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="f800f-115">Atribuut **ClientInfoString** kuvatakse siis, kui kustutatud on Outlookis, Outlooki veebirakenduses (varem Outlook Web App) või mis tahes muus seadmes.</span><span class="sxs-lookup"><span data-stu-id="f800f-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="f800f-116">Lisateavet leiate teemast [postkasti jaoks meili edasisaatmise häälestamine](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="f800f-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="f800f-117">**Märkus**: kustutatud üksusi ei saa auditi Logi funktsiooni abil taastada.</span><span class="sxs-lookup"><span data-stu-id="f800f-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="f800f-118">Outlooki veebirakenduses kustutatud sõnumite toomise kohta leiate teavet teemast [Kustutatud üksuste taastamine Outlook Web Appis](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="f800f-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
