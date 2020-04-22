---
title: Tuvastada sisendkausta reegli tegevuse auditilogi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716420"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2824f-102">Tuvastada sisendkausta reegli tegevuse auditilogi</span><span class="sxs-lookup"><span data-stu-id="2824f-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2824f-103">Auditilogi otsingut saate kasutada Microsoft 365 Security & vastavuse keskus sisendkausta reegli sündmuste kuvamiseks (loomine, muutmine ja kustutamine sisendkausta reeglid).</span><span class="sxs-lookup"><span data-stu-id="2824f-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2824f-104">Logige sisse [Microsoft 365 Security & vastavuse Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="2824f-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2824f-105">**otsingulehele otsingu** > **auditilogi** .</span><span class="sxs-lookup"><span data-stu-id="2824f-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="2824f-106">Saate **valida kuupäevavahemiku alguskuupäeva ja** **lõppkuupäeva** väljadel.</span><span class="sxs-lookup"><span data-stu-id="2824f-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2824f-107">**Exchange ' i postkasti tegevuste**, veenduge, et välja **Tegevused** väärtuseks on seatud **Uus InboxRule luua/muuta/lubada/keelata sisendkausta reegel**.</span><span class="sxs-lookup"><span data-stu-id="2824f-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2824f-108">Klõpsake suvandit **Otsing**.</span><span class="sxs-lookup"><span data-stu-id="2824f-108">Click **Search**.</span></span>

<span data-ttu-id="2824f-109">Valige tulemustel auditikirje.</span><span class="sxs-lookup"><span data-stu-id="2824f-109">In the results, select an audit record.</span></span> <span data-ttu-id="2824f-110">Üksikasjade hüpik, klõpsake **rohkem teavet**.</span><span class="sxs-lookup"><span data-stu-id="2824f-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2824f-111">Teave sisendkausta reegli sätete kohta kuvatakse väljal **Parameetrid** .</span><span class="sxs-lookup"><span data-stu-id="2824f-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2824f-112">Lisateabe saamiseks vaadake määratlemine, [kui kasutaja lõi sisendkausta reegel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="2824f-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
