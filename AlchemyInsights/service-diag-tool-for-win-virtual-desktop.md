---
title: Teenuse diagnostika tööriist Windows Virtual Desktopi jaoks
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677651"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="9d384-102">Teenuse diagnostika tööriist Windows Virtual Desktopi jaoks</span><span class="sxs-lookup"><span data-stu-id="9d384-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="9d384-103">Windowsi Virtual Desktop (WVD) pakub diagnostilist tööriista, mis võimaldab administraatoritel tuvastada tõrkeid ühe liidese kaudu.</span><span class="sxs-lookup"><span data-stu-id="9d384-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="9d384-104">See tööriist logib diagnostikaga seotud teavet alati, kui WVD kasutab keegi, kellele on määratud WVD roll.</span><span class="sxs-lookup"><span data-stu-id="9d384-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="9d384-105">Iga logi sisaldab teavet tegevusega seotud WVD rolli, seansi ajal kuvatavate tõrketeadete ning rentniku ja kasutaja kohta käiva teabe kohta.</span><span class="sxs-lookup"><span data-stu-id="9d384-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="9d384-106">Azure ' i Logi analüüsi saab konfigureerida, et jäädvustada diagnostiline tööriist loodud tegevuste Logi.</span><span class="sxs-lookup"><span data-stu-id="9d384-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="9d384-107">Tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="9d384-107">Here's how:</span></span>

1. <span data-ttu-id="9d384-108">Azure ' i [portaali](https://go.microsoft.com/fwlink/?linkid=2129500) või [Azure PowerShelli](https://go.microsoft.com/fwlink/?linkid=2129501)abil saate luua Logi Analyticsi tööruumi.</span><span class="sxs-lookup"><span data-stu-id="9d384-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="9d384-109">[Ühendage Windowsi arvutid Azure ' i kuvariga](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="9d384-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="9d384-110">Hankige tööruumi ID ja oma tööruumi primaarvõti.</span><span class="sxs-lookup"><span data-stu-id="9d384-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="9d384-111">Installiviisard vajab seda teavet agendi õigeks konfigureerimiseks ning selle tagamiseks, et see saaks suhelda Azure ' i kuvariga.</span><span class="sxs-lookup"><span data-stu-id="9d384-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="9d384-112">[Push diagnostika andmed oma tööruumi](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="9d384-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="9d384-113">Saate WVD rentniku andmeid oma tööruumi Logi analüüsile üle anda.</span><span class="sxs-lookup"><span data-stu-id="9d384-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="9d384-114">WVD seotud sisemiste või väliste [probleemide tuvastamine ja diagnoosimine](https://go.microsoft.com/fwlink/?linkid=2128338) .</span><span class="sxs-lookup"><span data-stu-id="9d384-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="9d384-115">Lisateavet WVD teenuse diagnostika tööriista konfigureerimise kohta leiate teemast [diagnostika funktsiooni jaoks Logi analüüsi kasutamine](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="9d384-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
