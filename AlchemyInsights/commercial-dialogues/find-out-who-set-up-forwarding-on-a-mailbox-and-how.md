---
title: Vaadake, kes häälestas postkastis edasisaatmise ja kuidas
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481573"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="ae8cc-102">Vaadake, kes häälestas postkastis edasisaatmise ja kuidas</span><span class="sxs-lookup"><span data-stu-id="ae8cc-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="ae8cc-103">Kui postkastis on määratud väline edasisaatmine, auditeeritakse tegevust Set-Mailbox cmdlet-käsu osana.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="ae8cc-104">Auditilogi tegevuse leidmiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="ae8cc-105">Avage [Office 365 turbe & täitmise keskus](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="ae8cc-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ae8cc-106">Valige **Otsingu** >  **auditilogi otsing**.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ae8cc-107">Kui kuvatakse teade selle kohta, et teil on vaja auditit lülitada, jätkake ja lülitage see kohe välja.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ae8cc-108">Kui see funktsioon pole sisse lülitatud, ei saa otsingutulemused eelmistest kuupäevadest andmeid tõmmata.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ae8cc-109">Veenduge, et välja **Tegevused** väärtuseks on seatud **kõigi tegevuste tulemid** (vaikeväärtus).</span><span class="sxs-lookup"><span data-stu-id="ae8cc-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="ae8cc-110">Määrake kuupäevavahemik.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-110">Specify the date range.</span></span> <span data-ttu-id="ae8cc-111">Te ei pea kasutajanime määrama.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="ae8cc-112">Valige **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-112">Select **Search**.</span></span> <span data-ttu-id="ae8cc-113">Tegevused kuvatakse jaotises **tulemid**.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="ae8cc-114">Valige **Filtreeri tulemid** ja seejärel sisestage väljale **tegevuse** filter väärtus **Set-postkast** .</span><span class="sxs-lookup"><span data-stu-id="ae8cc-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="ae8cc-115">See funktsioon annab tulemuseks kõik **postkasti** toimingud.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="ae8cc-116">Üksikasjade kuvamiseks valige tegevus ja seejärel valige **rohkem teavet**.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="ae8cc-117">Jaotises **Parameetrid** saate vaadata postkastis määratud edasisaatmise meiliaadressi.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="ae8cc-118">**Kasutajanimi** tähistab kasutajat, kes häälestas postkastis välise edasisaatmise.</span><span class="sxs-lookup"><span data-stu-id="ae8cc-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="ae8cc-119">Lisateavet leiate teemast [Office 365 auditilogi otsimine levinud stsenaariumide tõrkeotsinguks](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="ae8cc-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>