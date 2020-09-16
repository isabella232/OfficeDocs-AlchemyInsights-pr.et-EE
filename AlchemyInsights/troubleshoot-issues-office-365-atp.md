---
title: Office 365 täiustatud ohtude kaitsega seotud probleemide tõrkeotsing (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758061"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="601f9-102">Office 365 ATP-ga seotud probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="601f9-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="601f9-103">Kas **teate meilisõnumite kohaletoimetamisega seotud viivitusi**?</span><span class="sxs-lookup"><span data-stu-id="601f9-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="601f9-104">Proovige kasutada oma ATP turvaliste manuste poliitikate jaoks dünaamilist kohaletoimetamise võimalust.</span><span class="sxs-lookup"><span data-stu-id="601f9-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="601f9-105">See väldib meilisõnumi kohaletoimetamisega viivitamist, kaitstes samal ajal adressaate pahatahtlike failide eest.</span><span class="sxs-lookup"><span data-stu-id="601f9-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="601f9-106">**Kas soovid teatada valedest positiivsetest või valedest negatiivist**?</span><span class="sxs-lookup"><span data-stu-id="601f9-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="601f9-107">Kasutage seda linki, et esitada oma toimik analüüsimiseks. [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="601f9-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="601f9-108">**Kas teadsite, et saate lubada, et teie asutuse inimeste vahel saadetava meili korral saab kasutada ATP turvaliste linkide kaitset**?</span><span class="sxs-lookup"><span data-stu-id="601f9-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="601f9-109">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="601f9-109">Follow these steps:</span></span>
    1. <span data-ttu-id="601f9-110">Avage https://protection.office.com ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="601f9-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="601f9-111">Valige **ohustatud halduse**  >  **poliitika**  >  **Turvalised lingid**.</span><span class="sxs-lookup"><span data-stu-id="601f9-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="601f9-112">Redigeerige (või lisage) jaotises **poliitika, mis rakenduvad kindlatele adressaatidele**.</span><span class="sxs-lookup"><span data-stu-id="601f9-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="601f9-113">Valige **organisatsioonis saadetavate sõnumite turvaliste linkide rakendamine**.</span><span class="sxs-lookup"><span data-stu-id="601f9-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="601f9-114">Salvestage oma poliitika ja lubage muudatuste tegemiseks umbes 30 minutit oma Datacenteri kaudu oma teed teha.</span><span class="sxs-lookup"><span data-stu-id="601f9-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="601f9-115">Lisateavet ATP kohta leiate teemast [Office 365 Advanced Thread Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="601f9-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>