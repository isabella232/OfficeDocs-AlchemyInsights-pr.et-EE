---
title: Kustutatud sündmuste auditi logide lugemine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429526"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="bd31e-102">Kustutatud sündmuste auditi logide lugemine</span><span class="sxs-lookup"><span data-stu-id="bd31e-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="bd31e-103">Selleks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="bd31e-103">Here's how to do this:</span></span>

1. <span data-ttu-id="bd31e-104">Avage [Office 365 turbe & täitmise keskus](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="bd31e-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="bd31e-105">Valige **Otsingu**  >  [**auditilogi otsing**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="bd31e-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="bd31e-106">Kui kuvatakse teade selle kohta, et peate funktsiooni lülitama, jätkake ja lülitage see kohe välja.</span><span class="sxs-lookup"><span data-stu-id="bd31e-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="bd31e-107">Kui funktsioon pole sisse lülitatud, ei saa otsingutulemused eelmistest kuupäevadest andmeid tõmmata.</span><span class="sxs-lookup"><span data-stu-id="bd31e-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="bd31e-108">Valige **Tegevused** ja seejärel otsige **Exchange ' i postkasti tegevused**.</span><span class="sxs-lookup"><span data-stu-id="bd31e-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="bd31e-109">Valige kustutatud **sõnumite** kaustast Kustutatud üksused ja **teisaldatud sõnumid kausta Kustutatud** suvandid.</span><span class="sxs-lookup"><span data-stu-id="bd31e-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="bd31e-110">Kui olete lõpetanud, klõpsake paani **Tegevused** minimeerimiseks väljaspool paani.</span><span class="sxs-lookup"><span data-stu-id="bd31e-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="bd31e-111">Määrake kuupäevavahemik ja seejärel valige väljal **Kasutajad** selle kasutaja kasutajanimi, keda soovite uurida.</span><span class="sxs-lookup"><span data-stu-id="bd31e-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="bd31e-112">Korraga saab valida ka mitu kasutajat.</span><span class="sxs-lookup"><span data-stu-id="bd31e-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="bd31e-113">Valige **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="bd31e-113">Select **Search**.</span></span> <span data-ttu-id="bd31e-114">Tegevused kuvatakse jaotises **tulemid**.</span><span class="sxs-lookup"><span data-stu-id="bd31e-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="bd31e-115">Üksikasjade kuvamiseks valige tegevus ja seejärel valige **rohkem teavet**.</span><span class="sxs-lookup"><span data-stu-id="bd31e-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="bd31e-116">Lisateavet kustutatud üksuse kohta (nt teema teemarida ja üksuse asukoht kustutatud kujul) kuvatakse väljal **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="bd31e-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="bd31e-117">Kustutatud üksusi ei saa auditi Logi funktsiooni abil taastada.</span><span class="sxs-lookup"><span data-stu-id="bd31e-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="bd31e-118">Kustutatud üksuste taastamiseks lugege teemat [Kustutatud üksuste või meilide taastamine Outlook Web Appis](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="bd31e-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="bd31e-119">Lisateavet leiate teemast [Office 365 auditilogi otsimine levinud stsenaariumide tõrkeotsinguks](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="bd31e-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
