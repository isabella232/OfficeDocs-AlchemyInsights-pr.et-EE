---
title: IP-aadressi ja kliendi tuvastamine auditi logides
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668306"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="a9080-102">IP-aadressi ja kliendi tuvastamine auditi logides</span><span class="sxs-lookup"><span data-stu-id="a9080-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="a9080-103">Auditi logides kuvatakse Microsoft 365 kasutaja või administraatori tegevusele vastav IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="a9080-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="a9080-104">Kliendiinfo on ka logitud.</span><span class="sxs-lookup"><span data-stu-id="a9080-104">The client information is also logged.</span></span> <span data-ttu-id="a9080-105">Selle teabe tuvastamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="a9080-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="a9080-106">Logige sisse [Microsoft 365 turbe & nõuetele vastavuse keskuses](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a9080-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="a9080-107">Avage leht **Otsingu**  >  **auditilogi otsing** .</span><span class="sxs-lookup"><span data-stu-id="a9080-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="a9080-108">Kui olete huvitatud konkreetsest tegevusest, valige see **tegevuste** loendist.</span><span class="sxs-lookup"><span data-stu-id="a9080-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="a9080-109">Kui ei, siis tagastatakse kõik tegevused valitud kasutaja jaoks (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="a9080-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="a9080-110">**Märkus**: teatud tegevused ei pruugi olla saadaval menüüs **Tegevused** ; need auditi üksused tagastatakse siis, kui valitud on **kõigi tegevuste tulemid** (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="a9080-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="a9080-111">Määrake väljal **Kasutajad** kasutajanimi, valige tegevuse jaoks sobiv kuupäevavahemik ja klõpsake siis nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="a9080-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="a9080-112">Tulemites näete paanil tulemid selle tegevuse IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="a9080-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="a9080-113">Valige auditi kirje, et **näha üksikasjalikku teavet hüpik (** nt klient, toimingu sooritanud kasutaja jne).</span><span class="sxs-lookup"><span data-stu-id="a9080-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="a9080-114">Lisateavet leiate teemast [ohustatud kontole juurdepääsemiseks kasutatava arvuti IP-aadressi leidmine](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="a9080-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
