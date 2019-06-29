---
title: IP-aadress ja kliendi auditilogi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382949"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="073b2-102">IP-aadress ja kliendi auditilogi</span><span class="sxs-lookup"><span data-stu-id="073b2-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="073b2-103">Auditilogide näidatakse IP-aadress, mis vastab kasutaja või administraator tegevus.</span><span class="sxs-lookup"><span data-stu-id="073b2-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="073b2-104">Kliendi andmed ka logitud.</span><span class="sxs-lookup"><span data-stu-id="073b2-104">The client information is also logged.</span></span> <span data-ttu-id="073b2-105">Siin on sammud teha kindlaks sellise teabe</span><span class="sxs-lookup"><span data-stu-id="073b2-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="073b2-106">Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="073b2-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="073b2-107">Valige **Auditi logifaili Otsi**nuppu **Otsi ja uurimine** .</span><span class="sxs-lookup"><span data-stu-id="073b2-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="073b2-108">Kui olete huvitatud konkreetse töö, valige see **tegevus** .</span><span class="sxs-lookup"><span data-stu-id="073b2-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="073b2-109">Kui ei, siis kõik tegevused tuleb tagasi valitud kasutaja (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="073b2-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="073b2-110">**Märkus**: teatud tegevused ei pruugi **tegevuste** menüü; Aga need auditi üksused tagasi kui **Näita tulemust kõik tegevused** on valitud (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="073b2-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="073b2-111">Määrake kasutajanimi väljale **Kasutajad** valida tegevuseks sobiv kuupäevavahemik ja klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="073b2-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="073b2-112">Tulemused, näete IP-aadressi, mille puhul tulemuste paanil.</span><span class="sxs-lookup"><span data-stu-id="073b2-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="073b2-113">Valige auditikirje üksikasjaliku teabe **üksikasjad** hüpik (nt klient, kasutaja, et läbi tegevuse, jne.).</span><span class="sxs-lookup"><span data-stu-id="073b2-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="073b2-114">Lisateabe saamiseks vt [ohustatud konto juurdepääsuks arvuti IP-aadressi leidmine](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="073b2-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
