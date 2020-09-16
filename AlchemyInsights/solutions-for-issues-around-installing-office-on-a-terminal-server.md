---
title: Lahendused Office ' i installimisega seotud probleemide lahendamiseks terminalserveri jaoks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738453"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="d0107-102">Lahendused Office ' i installimisega seotud probleemide lahendamiseks terminalserveri jaoks</span><span class="sxs-lookup"><span data-stu-id="d0107-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="d0107-103">Ühiskasutusega arvuti aktiveerimiseks peab teil olema tellimus, mis sisaldab Enterprise ' i jaoks mõeldud Microsoft 365 rakendusi.</span><span class="sxs-lookup"><span data-stu-id="d0107-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="d0107-104">Veenduge, et ühiskasutusega arvuti aktiveerimine oleks lubatud.</span><span class="sxs-lookup"><span data-stu-id="d0107-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="d0107-105">Veenduge, et aktiveerimine õnnestus</span><span class="sxs-lookup"><span data-stu-id="d0107-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="d0107-106">Vaadake üle ühiskasutusega arvuti aktiveerimise tõrketeated.</span><span class="sxs-lookup"><span data-stu-id="d0107-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="d0107-107">"Teie kontolt leitud tooteid ei saa kasutada Office ' i aktiveerimiseks ühiskasutatavates arvuti olukordades"</span><span class="sxs-lookup"><span data-stu-id="d0107-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="d0107-108">See tõrge tähendab, et teil pole paketti, mis sisaldab Microsoft 365 rakendusi Enterprise ' i jaoks.</span><span class="sxs-lookup"><span data-stu-id="d0107-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="d0107-109">"Litsentsimata toode"</span><span class="sxs-lookup"><span data-stu-id="d0107-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="d0107-110">Kontrollige, kas kasutajale on määratud Microsoft 365 rakenduste litsents Enterprise ' i jaoks.</span><span class="sxs-lookup"><span data-stu-id="d0107-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="d0107-111">Kontrollige, kas kasutaja logib sisse kasutaja kontoga.</span><span class="sxs-lookup"><span data-stu-id="d0107-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="d0107-112">Veenduge, et ühiskasutusse antud arvuti ja Interneti vahel oleks Ühenduvus.</span><span class="sxs-lookup"><span data-stu-id="d0107-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="d0107-113">Muude tõrkeotsingu näpunäidete kohta leiate teavet teemast [ühiskasutusega arvuti aktiveerimisega seotud probleemide tõrkeotsing](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation) .</span><span class="sxs-lookup"><span data-stu-id="d0107-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>