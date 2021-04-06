---
title: Windows Virtual Desktopi teenusediagnostika tööriist
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595632"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="0f59f-102">Windows Virtual Desktopi teenusediagnostika tööriist</span><span class="sxs-lookup"><span data-stu-id="0f59f-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="0f59f-103">Windows Virtual Desktop (WVD) pakub diagnostikatööriista, mis võimaldab administraatoritel tuvastada tõrkeid ühe liidese kaudu.</span><span class="sxs-lookup"><span data-stu-id="0f59f-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="0f59f-104">See tööriist logib diagnostikaga seotud teavet iga kord, kui WVD-d kasutab keegi, kellele on määratud WVD roll.</span><span class="sxs-lookup"><span data-stu-id="0f59f-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="0f59f-105">Iga logi sisaldab teavet tegevusega seotud WVD rolli, seansi ajal kuvatavate tõrketeadete ning rentniku ja kasutaja kohta.</span><span class="sxs-lookup"><span data-stu-id="0f59f-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="0f59f-106">Azure'i logianalüüsi saab konfigureerida jäädvustama diagnostikatööriista loodud tegevuste logi, järgides järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="0f59f-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="0f59f-107">Logianalüüsi tööruumi loomine [Azure'i portaali või](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShelli abil.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="0f59f-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="0f59f-108">[Ühendage Windowsi arvutid Azure'i kuvariga.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="0f59f-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="0f59f-109">Hankige tööruumi ID ja tööruumi primaarvõti.</span><span class="sxs-lookup"><span data-stu-id="0f59f-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="0f59f-110">Häälestusviisard vajab seda teavet agendi õigeks konfigureerimiseks ja Azure Monitoriga suhtlemiseks.</span><span class="sxs-lookup"><span data-stu-id="0f59f-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="0f59f-111">[Lükake diagnostikaandmed oma tööruumi.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="0f59f-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="0f59f-112">Saate oma WVD rentniku diagnostikaandmed oma tööruumi logianalüüsisse lükata.</span><span class="sxs-lookup"><span data-stu-id="0f59f-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="0f59f-113">[Tuvastage ja diagnoosige probleeme,](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) mis on WVD-ga seoses sisemised või välisprobleemid.</span><span class="sxs-lookup"><span data-stu-id="0f59f-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="0f59f-114">Lisateavet WVD teenusediagnostikatööriista konfigureerimise kohta leiate teemast Logianalüüsi kasutamine diagnostikafunktsiooni jaoks.</span><span class="sxs-lookup"><span data-stu-id="0f59f-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>