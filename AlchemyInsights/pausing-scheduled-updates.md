---
title: Ajastatud värskenduste peatamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555104"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="673db-102">Ajastatud värskenduste peatamine</span><span class="sxs-lookup"><span data-stu-id="673db-102">Pausing scheduled updates</span></span>

<span data-ttu-id="673db-103">Kui käsk Peata on välja antud, ei töötle seadmed käsku enne, kui nad järgmine kord Intune ' i sisse möllivad.</span><span class="sxs-lookup"><span data-stu-id="673db-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="673db-104">Selle tõttu võivad teie seadmed olla järgmised.</span><span class="sxs-lookup"><span data-stu-id="673db-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="673db-105">Enne sisseregistreerimiseks installitud ajastatud värskendused on installitud.</span><span class="sxs-lookup"><span data-stu-id="673db-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="673db-106">Käsk paus on välja lülitatud.</span><span class="sxs-lookup"><span data-stu-id="673db-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="673db-107">Sel juhul, kui seadmed on sisse lülitatud, võivad nad olla alla laaditud ja installitud ajastatud värskendused enne sisseregistreerimist.</span><span class="sxs-lookup"><span data-stu-id="673db-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>