---
title: 'Tõrge: selle arvuti reeglid ei ühti'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617964"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="422e5-102">Tõrge: selle arvuti reeglid ei ühti</span><span class="sxs-lookup"><span data-stu-id="422e5-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="422e5-103">Teadaolev probleem värskendatud oleku nägemiseks vaadake [selle arvuti reeglid ei vasta Microsoft Exchange ' i reeglid](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="422e5-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="422e5-104">Outlooki meeskond on rakendanud Fix Build 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="422e5-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="422e5-105">Parandus on juba siseringi Fast ja läheb igakuine kanali lõpus juuni 2020.</span><span class="sxs-lookup"><span data-stu-id="422e5-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="422e5-106">Kui teil on fikseeritud ehitada võite saada viip "milliseid reegleid soovite säilitada" viimast korda.</span><span class="sxs-lookup"><span data-stu-id="422e5-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="422e5-107">Valige server, kui küsitakse ja seejärel tagasi Outlookis ja lubage kõik reeglid, mis olid keelatud.</span><span class="sxs-lookup"><span data-stu-id="422e5-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="422e5-108">Kuni parandus on saadaval palun kasutage järgmist lahendust:</span><span class="sxs-lookup"><span data-stu-id="422e5-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="422e5-109">**Lahendus**: viimastel aruannetes probleem ilmnes need, mis on loodud ainult kliendi reeglid Outlooki töölaual.</span><span class="sxs-lookup"><span data-stu-id="422e5-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="422e5-110">Kui jätkate probleemi, kaaluge reeglite kustutamist ja seejärel luua ja muuta reeglid ainult OWA (Outlook Web Appi) kuni probleem on lahendatud.</span><span class="sxs-lookup"><span data-stu-id="422e5-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="422e5-111">Kui te ei saa reegleid käsitsi kustutada, saate käivitada Outlooki käsu Outlooki käivitamisel, käivitades Outlook. exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="422e5-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="422e5-112">See kustutab kliendi ja serveri reeglid.</span><span class="sxs-lookup"><span data-stu-id="422e5-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="422e5-113">See kustutab kõik Outlooki profiilis olevate kontode reeglid.</span><span class="sxs-lookup"><span data-stu-id="422e5-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="422e5-114">See käsk on veel dokumenteeritud käsurea lüliteid artikkel.</span><span class="sxs-lookup"><span data-stu-id="422e5-114">This command is further documented in the Command-line switches  article.</span></span>