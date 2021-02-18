---
title: Kas teie kasutajad on saanud ründesisuga meilisõnumeid?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291788"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="caf5d-102">Kas teie kasutajad on saanud ründesisuga meilisõnumeid?</span><span class="sxs-lookup"><span data-stu-id="caf5d-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="caf5d-103">Ründemeilidest saate nüüd Microsoftile teada anda [turbe- ja vastavuskeskuse edastuste lehel](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="caf5d-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="caf5d-104">[Administraatori edastuste](https://sip.protection.office.com/reportsubmission) lehe kaudu edastatud sõnumeid kontrollitakse ja **üksikasjade** hüpikus kuvatakse järgmine teave:</span><span class="sxs-lookup"><span data-stu-id="caf5d-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="caf5d-105">kas saatja meiliaadressi autentimisel ilmnes kohaletoimetamise ajal probleeme;</span><span class="sxs-lookup"><span data-stu-id="caf5d-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="caf5d-106">kas leidub poliitikatabamusi, mis oleksid võinud sõnumiga seotud otsust mingil viisil mõjutada või selle alistada;</span><span class="sxs-lookup"><span data-stu-id="caf5d-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="caf5d-107">praegused ohutustamise tulemused, et saaksite vaadata, kas sõnumis sisaldunud URL-id või failid olid ründesisuga või mitte;</span><span class="sxs-lookup"><span data-stu-id="caf5d-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="caf5d-108">hindajate tagasiside.</span><span class="sxs-lookup"><span data-stu-id="caf5d-108">Feedback from graders</span></span>

<span data-ttu-id="caf5d-109">Alistuse leidmise korral peaks uus kontroll lõpule jõudma mõne minutiga.</span><span class="sxs-lookup"><span data-stu-id="caf5d-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="caf5d-110">Kui probleem polnud seotud meiliaadressi autentimisega või kui kohaletoimetamist ei mõjutanud poliitikast tulenev alistamine, võib hindajate tagasiside saamiseks kuluda kuni üks päev.</span><span class="sxs-lookup"><span data-stu-id="caf5d-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="caf5d-111">Kui te pole sõnumi, URL-i või faili osas tehtud lõpliku otsusega (blokeerida või mitte blokeerida) nõus, esitage sõnum ühe päeva möödumisel uuesti kontrollimiseks.</span><span class="sxs-lookup"><span data-stu-id="caf5d-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="caf5d-112">Suure tõenäosusega toob sõnumi uuesti esitamine kaasa otsuse muutumise.</span><span class="sxs-lookup"><span data-stu-id="caf5d-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="caf5d-113">Seni saate ründesisuga meilisõnumid kasutajate postkastidest eemaldada [selle artikli](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) juhiste järgi.</span><span class="sxs-lookup"><span data-stu-id="caf5d-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="caf5d-114">Kliendid, kellel on Microsoft Defender for Office 365, saavad:</span><span class="sxs-lookup"><span data-stu-id="caf5d-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="caf5d-115">kasutada [ohu-uurijat kahtlaste meilisõnumite leidmiseks ja kustutamiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered);</span><span class="sxs-lookup"><span data-stu-id="caf5d-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="caf5d-116">kasutada [ohutute linkide funktsiooni juurdepääsu blokeerimiseks](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) ründesisule viivale URL-ile;</span><span class="sxs-lookup"><span data-stu-id="caf5d-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="caf5d-117">jälgida kasutajaid, kes on ründesisule viivaid URL-e klõpsanud ja neile liikunud: [Andmepüügi-URL-ide ja klõpsude otsuseandmete vaatamine](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace);</span><span class="sxs-lookup"><span data-stu-id="caf5d-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="caf5d-118">käsitsi [käivitada automaatuurimise](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).</span><span class="sxs-lookup"><span data-stu-id="caf5d-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="caf5d-119">Samuti saate end ründesisuga failide ja URL-ide eest kaitsta artikli [Kaitse ründesisuga URL-ide ja failide eest](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) juhiste järgi.</span><span class="sxs-lookup"><span data-stu-id="caf5d-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>