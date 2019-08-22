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
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539160"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="c1225-102">Sisendkausta reegli tegevuse auditilogid tuvastada</span><span class="sxs-lookup"><span data-stu-id="c1225-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="c1225-103">Office 365 turvalisuse & vastavuse Center auditi logifaili Otsi saate vaadata sisendkausta reegel sündmused (luua, muuta ja kustutada sisendkausta reeglid).</span><span class="sxs-lookup"><span data-stu-id="c1225-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="c1225-104">Logige sisse [Office 365 & vastavuse Turvakeskus](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c1225-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c1225-105">Mine **Otsi** > **auditi logifaili** otsingulehte.</span><span class="sxs-lookup"><span data-stu-id="c1225-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c1225-106">Valige kuupäevavahemik väljadele **Alguskuupäev** ja **lõppkuupäev** .</span><span class="sxs-lookup"><span data-stu-id="c1225-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="c1225-107">Kontrollige jaotises **Exchange'i postkasti tegevust**, **tegevuse** väärtuseks on **New-InboxRule loomine/muutmine/luba/Keela reegel**.</span><span class="sxs-lookup"><span data-stu-id="c1225-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="c1225-108">Klõpsake nuppu **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="c1225-108">Click **Search**.</span></span>

<span data-ttu-id="c1225-109">Tulemused, valige audit kirje.</span><span class="sxs-lookup"><span data-stu-id="c1225-109">In the results, select an audit record.</span></span> <span data-ttu-id="c1225-110">Hüpik üksikasjad nuppu **Lisateave**.</span><span class="sxs-lookup"><span data-stu-id="c1225-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c1225-111">Sisendkausta reegli sätete kohta teabe kuvatakse väljal **Parameetrid** .</span><span class="sxs-lookup"><span data-stu-id="c1225-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="c1225-112">Lisateabe saamiseks vt [Determining kui sisendkausta reegel loonud kasutaja](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="c1225-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
