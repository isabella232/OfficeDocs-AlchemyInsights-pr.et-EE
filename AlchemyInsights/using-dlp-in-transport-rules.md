---
title: DLP kasutamine transpordireeglites
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827212"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="65e4a-102">DLP kasutamine transpordireeglites</span><span class="sxs-lookup"><span data-stu-id="65e4a-102">Using DLP in transport rules</span></span>

<span data-ttu-id="65e4a-103">Andmete kaotsimineku vältimise (DLP) integreerimiseks olemasolevasse transporti kasutage transpordireegli sättes tingimust „**Kui sõnum sisaldab... Tundlik teave**“.</span><span class="sxs-lookup"><span data-stu-id="65e4a-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="65e4a-104">**Lisateabe saamiseks vaadake järgnevat.**</span><span class="sxs-lookup"><span data-stu-id="65e4a-104">**For more details, see:**</span></span>

- <span data-ttu-id="65e4a-105">Integreeritud DLP tundliku teabe tüübid transpordireeglites: [Tundliku teabe reeglite integreerimine](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="65e4a-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="65e4a-106">Samuti saate testida reeglit koos või ilma poliitika testita, kasutades reeglil testimisrežiimi.</span><span class="sxs-lookup"><span data-stu-id="65e4a-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="65e4a-107">Pärast reegli loomist peaksite ootama 30 minutt enne selle testimist.</span><span class="sxs-lookup"><span data-stu-id="65e4a-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="65e4a-108">Vaadake teemat [Meilivoo/transpordireeglite testimine](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).</span><span class="sxs-lookup"><span data-stu-id="65e4a-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="65e4a-109">**Märkus**. Kui proovite EAC-s juurutada koos transpordireeglitega uut DLP poliitikat, kasutage selle asemel suvandit [DLP poliitikad turbe- ja vastavuskeskuses](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="65e4a-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
