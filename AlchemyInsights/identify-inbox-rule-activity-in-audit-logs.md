---
title: Sisendkausta reegli tegevuse auditilogid tuvastada
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383021"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="21dd3-102">Sisendkausta reegli tegevuse auditilogid tuvastada</span><span class="sxs-lookup"><span data-stu-id="21dd3-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="21dd3-103">Saate auditi Logi otsing turvalisuse & vastavuse Center sisendkausta reegel sündmuste (luua, muuta ja kustutada sisendkaustareeglid) vaatamiseks.</span><span class="sxs-lookup"><span data-stu-id="21dd3-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="21dd3-104">Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="21dd3-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="21dd3-105">Valige **Auditi logifaili Otsi**nuppu **Otsi ja uurimine** .</span><span class="sxs-lookup"><span data-stu-id="21dd3-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="21dd3-106">Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** .</span><span class="sxs-lookup"><span data-stu-id="21dd3-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="21dd3-107">Kontrollige jaotises **Exchange'i postkasti tegevust**, **tegevuse** väärtuseks on **New-InboxRule loomine/muutmine/luba/Keela reegel**.</span><span class="sxs-lookup"><span data-stu-id="21dd3-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="21dd3-108">Klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="21dd3-108">Click **Search**.</span></span>

<span data-ttu-id="21dd3-109">Tulemused, valige audit kirje.</span><span class="sxs-lookup"><span data-stu-id="21dd3-109">In the results, select an audit record.</span></span> <span data-ttu-id="21dd3-110">Hüpik üksikasjad nuppu **Lisateave**.</span><span class="sxs-lookup"><span data-stu-id="21dd3-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="21dd3-111">Sisendkausta reegli sätete kohta teabe kuvatakse väljal **Parameetrid** .</span><span class="sxs-lookup"><span data-stu-id="21dd3-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="21dd3-112">Lisateabe saamiseks vt [Determining kui sisendkausta reegel loonud kasutaja](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="21dd3-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
