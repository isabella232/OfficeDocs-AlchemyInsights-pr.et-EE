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
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539025"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="e8272-102">IP-aadress ja kliendi auditilogi</span><span class="sxs-lookup"><span data-stu-id="e8272-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="e8272-103">Office 365 kasutaja või administraator tegevus vastab IP-aadress kuvatakse auditilogide.</span><span class="sxs-lookup"><span data-stu-id="e8272-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="e8272-104">Kliendi andmed ka logitud.</span><span class="sxs-lookup"><span data-stu-id="e8272-104">The client information is also logged.</span></span> <span data-ttu-id="e8272-105">Siin on sammud teha kindlaks sellise teabe</span><span class="sxs-lookup"><span data-stu-id="e8272-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="e8272-106">Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e8272-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e8272-107">Mine **Otsi** > **auditi logifaili** otsingulehte.</span><span class="sxs-lookup"><span data-stu-id="e8272-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="e8272-108">Kui olete huvitatud konkreetse töö, valige see **tegevus** .</span><span class="sxs-lookup"><span data-stu-id="e8272-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="e8272-109">Kui ei, siis kõik tegevused tuleb tagasi valitud kasutaja (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="e8272-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="e8272-110">**Märkus**: teatud tegevused ei pruugi **tegevuste** menüü; Aga need auditi üksused tagasi kui **Näita tulemust kõik tegevused** on valitud (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="e8272-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="e8272-111">Määrake kasutajanimi väljale **Kasutajad** valida tegevuseks sobiv kuupäevavahemik ja klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="e8272-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="e8272-112">Tulemused, näete IP-aadressi, mille puhul tulemuste paanil.</span><span class="sxs-lookup"><span data-stu-id="e8272-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="e8272-113">Valige auditikirje üksikasjaliku teabe **üksikasjad** hüpik (nt klient, kasutaja, et läbi tegevuse, jne.).</span><span class="sxs-lookup"><span data-stu-id="e8272-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="e8272-114">Lisateabe saamiseks vt [ohustatud konto juurdepääsuks arvuti IP-aadressi leidmine](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="e8272-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
