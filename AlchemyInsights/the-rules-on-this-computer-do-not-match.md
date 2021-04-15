---
title: Tõrge. Selles arvutis kehtivad reeglid ei vasta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782948"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="4436c-102">Tõrge. Selles arvutis kehtivad reeglid ei vasta</span><span class="sxs-lookup"><span data-stu-id="4436c-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="4436c-103">Teadaoleva probleemi värskendatud oleku kuvamiseks lugege teemat Selle arvuti reeglid ei [vasta Microsoft Exchange'i reeglitele.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="4436c-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="4436c-104">Outlooki meeskond on rakendanud paranduse järgus 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="4436c-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="4436c-105">Lahendus on juba Insider Fastis ja see läheb kuupõhisele kanalile juuni lõpus 2020.</span><span class="sxs-lookup"><span data-stu-id="4436c-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="4436c-106">Kui olete fikseeritud järgu saanud, võidakse teil viimast korda kuvada viip "Milliseid reegleid soovite säilitada".</span><span class="sxs-lookup"><span data-stu-id="4436c-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="4436c-107">Kui teilt küsitakse, valige Server ja seejärel minge Outlookis tagasi ja lubage uuesti kõik keelatud reeglid.</span><span class="sxs-lookup"><span data-stu-id="4436c-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="4436c-108">Kuni parandus on saadaval, kasutage järgmist lahendust.</span><span class="sxs-lookup"><span data-stu-id="4436c-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="4436c-109">**Lahendus.** Hiljutistes aruannetes ilmnes probleem nende jaoks, kes on outlooki töölauarakenduses loonud ainult kliendireeglid.</span><span class="sxs-lookup"><span data-stu-id="4436c-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="4436c-110">Kui probleem ei lahene, kaaluge reeglite kustutamist ning seejärel looge ja redigeerige reegleid ainult OWA-s (Outlook Web Appis), kuni probleem on lahendatud.</span><span class="sxs-lookup"><span data-stu-id="4436c-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="4436c-111">Kui te ei saa reegleid käsitsi kustutada, saate Outlooki käivitamisel käivitada Outlooki käsu, käivitades Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="4436c-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="4436c-112">See kustutab nii kliendi- kui ka serverireeglid.</span><span class="sxs-lookup"><span data-stu-id="4436c-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="4436c-113">See kustutab kõik Outlooki profiili kõigi kontode reeglid.</span><span class="sxs-lookup"><span data-stu-id="4436c-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="4436c-114">See käsk on veel dokumenteeritud artiklis Käsurealülitid.</span><span class="sxs-lookup"><span data-stu-id="4436c-114">This command is further documented in the Command-line switches article.</span></span>

