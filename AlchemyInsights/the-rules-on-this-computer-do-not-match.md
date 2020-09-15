---
title: 'Tõrge: selle arvuti reeglid ei ühti'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690959"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="a3a2b-102">Tõrge: selle arvuti reeglid ei ühti</span><span class="sxs-lookup"><span data-stu-id="a3a2b-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="a3a2b-103">Selle teadaoleva probleemi värskendatud oleku vaatamiseks lugege selle [arvuti reegleid, mis ei vasta Microsoft Exchange ' i reeglitele.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="a3a2b-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="a3a2b-104">Outlooki meeskond on rakendanud lahenduse järgus 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="a3a2b-105">Fix on juba Insider Fast ja läheb igakuise kanali juuni lõpus 2020.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="a3a2b-106">Kui teil on püsiv järk, võite saada viiba "milliseid reegleid soovite säilitada" viimast korda.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="a3a2b-107">Valige küsimisel server ja seejärel naaske Outlookis ja lubage kõik keelatud reeglid uuesti.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="a3a2b-108">Kui lahendus on saadaval, kasutage järgmist lahendust.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="a3a2b-109">**Lahendus**: Viimatised aruanded on ilmnenud nende jaoks, kes on Outlooki töölaual loonud ainult klientrakenduste reegleid.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="a3a2b-110">Kui jätkate probleemi, kaaluge reeglite kustutamist ja seejärel looge ja redigeerige reegleid ainult OWA-s (Outlook Web App), kuni probleem laheneb.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="a3a2b-111">Kui te ei saa reegleid käsitsi kustutada, saate Outlooki käsu käivitada Outlooki käivitamisel, käivitades Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="a3a2b-112">See toiming kustutab nii kliendi kui ka serveri reeglid.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="a3a2b-113">See kustutab kõik Outlooki profiilis olevate kontode reeglid.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="a3a2b-114">See käsk on täiendavalt dokumenteeritud käsurea lülitite artiklis.</span><span class="sxs-lookup"><span data-stu-id="a3a2b-114">This command is further documented in the Command-line switches article.</span></span>

