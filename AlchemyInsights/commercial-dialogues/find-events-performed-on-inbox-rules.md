---
title: Sisendkausta reeglitega tehtud sündmuste otsimine
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481717"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="814a3-102">Sisendkausta reeglitega tehtud sündmuste otsimine</span><span class="sxs-lookup"><span data-stu-id="814a3-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="814a3-103">Kui sisendkausta reeglid on loodud, muudetud või kustutatud, salvestatakse sündmused auditi logisse.</span><span class="sxs-lookup"><span data-stu-id="814a3-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="814a3-104">Nende läbivaatamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="814a3-104">Here's how to review them:</span></span>

1. <span data-ttu-id="814a3-105">Avage [Office 365 turbe & täitmise keskus](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="814a3-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="814a3-106">Valige otsingu > auditilogi otsing.</span><span class="sxs-lookup"><span data-stu-id="814a3-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="814a3-107">Kui kuvatakse teade selle kohta, et teil on vaja auditit lülitada, jätkake ja lülitage see kohe välja.</span><span class="sxs-lookup"><span data-stu-id="814a3-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="814a3-108">Kui see funktsioon pole sisse lülitatud, ei saa otsingutulemused eelmistest kuupäevadest andmeid tõmmata.</span><span class="sxs-lookup"><span data-stu-id="814a3-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="814a3-109">Valige väli tegevused ja leidke Exchange ' i postkasti toimingud ning seejärel valige New-InboxRule Outlook Web Appi kaudu sisendkausta reegli loomine.</span><span class="sxs-lookup"><span data-stu-id="814a3-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="814a3-110">Kui olete lõpetanud, klõpsake paani tegevused minimeerimiseks väljaspool paani.</span><span class="sxs-lookup"><span data-stu-id="814a3-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="814a3-111">Määrake kuupäevavahemik ja seejärel valige väljal kasutajad selle kasutaja kasutajanimi, keda soovite uurida.</span><span class="sxs-lookup"><span data-stu-id="814a3-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="814a3-112">Korraga saab valida ka mitu kasutajat.</span><span class="sxs-lookup"><span data-stu-id="814a3-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="814a3-113">Valige Otsi.</span><span class="sxs-lookup"><span data-stu-id="814a3-113">Select Search.</span></span> <span data-ttu-id="814a3-114">Tegevused kuvatakse jaotises tulemid.</span><span class="sxs-lookup"><span data-stu-id="814a3-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="814a3-115">Üksikasjade kuvamiseks valige tegevus ja seejärel valige rohkem teavet.</span><span class="sxs-lookup"><span data-stu-id="814a3-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="814a3-116">Jaotises parameetrid saate vaadata reegli nime, seatud tingimusi ja toiminguid, mida reegel võtab.</span><span class="sxs-lookup"><span data-stu-id="814a3-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="814a3-117">Lisateavet leiate teemast Office 365 auditilogi otsimine levinud stsenaariumide tõrkeotsinguks.</span><span class="sxs-lookup"><span data-stu-id="814a3-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>