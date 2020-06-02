---
title: IP-aadressi ja kliendi tuvastamine auditiloogides
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508912"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="4f27e-102">IP-aadressi ja kliendi tuvastamine auditiloogides</span><span class="sxs-lookup"><span data-stu-id="4f27e-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="4f27e-103">Auditilogi kuvatakse IP-aadress, mis vastab tegevusele Microsoft 365 kasutaja või administraator.</span><span class="sxs-lookup"><span data-stu-id="4f27e-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="4f27e-104">Samuti logitakse klienditeave.</span><span class="sxs-lookup"><span data-stu-id="4f27e-104">The client information is also logged.</span></span> <span data-ttu-id="4f27e-105">Siin on juhised sellise teabe tuvastamiseks</span><span class="sxs-lookup"><span data-stu-id="4f27e-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="4f27e-106">Logige sisse [Microsoft 365 Security & vastavuse Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="4f27e-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="4f27e-107">**otsingulehele otsingu**  >  **auditilogi** .</span><span class="sxs-lookup"><span data-stu-id="4f27e-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="4f27e-108">Kui olete huvitatud konkreetsest tegevusest, valige see **tegevuste** loendist.</span><span class="sxs-lookup"><span data-stu-id="4f27e-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="4f27e-109">Kui ei, siis tagastatakse kõik tegevused valitud kasutajale (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="4f27e-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="4f27e-110">**Märkus**: teatud tegevused ei pruugi olla saadaval menüüs **Tegevused** ; kuid need auditiüksused tagastatakse, kui on valitud **kõigi tegevuste Kuva tulemid** (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="4f27e-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="4f27e-111">Määrake kasutajanimi väljal **Kasutajad** , valige tegevuse jaoks sobiv kuupäevavahemik ja klõpsake suvandit **Otsing**.</span><span class="sxs-lookup"><span data-stu-id="4f27e-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="4f27e-112">Tulemustes näete tulemuste paanil selle tegevuse IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="4f27e-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="4f27e-113">Valige auditiloend üksikasjaliku teabe kuvamiseks **üksikasjade** hüpik (nt. Klient, kasutaja, kes tegi toimingu vms).</span><span class="sxs-lookup"><span data-stu-id="4f27e-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="4f27e-114">Lisateabe saamiseks vaadake [kahjustatud kontole juurdepääsuks kasutatava arvuti IP-aadressi leidmist](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="4f27e-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
