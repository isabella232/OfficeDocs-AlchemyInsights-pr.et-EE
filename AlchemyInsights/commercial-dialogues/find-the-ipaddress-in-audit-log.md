---
title: IP-aadressi otsimine auditi logist
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481720"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="f9f2f-102">IP-aadressi otsimine auditi logist</span><span class="sxs-lookup"><span data-stu-id="f9f2f-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="f9f2f-103">Kasutaja või administraatori teostatud tegevus vastab IP-aadressile, mis on kuvatud auditi logides.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="f9f2f-104">Kliendiinfo on ka logitud.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-104">The client information is also logged.</span></span> <span data-ttu-id="f9f2f-105">IP-aadressi tuvastamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="f9f2f-106">Avage [Office 365 turbe & täitmise keskus](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="f9f2f-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f9f2f-107">Valige **Otsingu**  >  **[auditilogi otsing](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f9f2f-108">Kui kuvatakse teade selle kohta, et teil on vaja auditit lülitada, jätkake ja lülitage see kohe välja.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="f9f2f-109">Kui see funktsioon pole lubatud, siis ei saa otsingutulemused eelmistest kuupäevadest andmeid tõmmata.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f9f2f-110">Kui olete huvitatud konkreetsest tegevusest, valige see loendist **Tegevused** ; Vastasel juhul tagastatakse valitud kasutajale vaikimisi kõik tegevused.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="f9f2f-111">Pange tähele, et teatud tegevused ei pruugi olla menüüs **Tegevused** valiku jaoks saadaval. need auditi üksused tagastatakse siis, kui valitud on **kõigi tegevuste tulemid** (vaikesäte).</span><span class="sxs-lookup"><span data-stu-id="f9f2f-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="f9f2f-112">Määrake kuupäevavahemik ja valige väljal **Kasutajad** selle kasutaja kasutajanimi, keda soovite uurida.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="f9f2f-113">Valige **Otsi**.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-113">Select **Search**.</span></span> <span data-ttu-id="f9f2f-114">Tegevused kuvatakse jaotises **tulemid**.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-114">The activities appear under **Results**.</span></span> <span data-ttu-id="f9f2f-115">Iga tegevuse IP-aadressi saab vaadata.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="f9f2f-116">Üksikasjade kuvamiseks valige tegevus ja seejärel valige **rohkem teavet**.</span><span class="sxs-lookup"><span data-stu-id="f9f2f-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="f9f2f-117">Lisateavet leiate teemast [Office 365 auditilogi otsimine levinud stsenaariumide tõrkeotsinguks](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="f9f2f-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>