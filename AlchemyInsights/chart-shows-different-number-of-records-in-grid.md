---
title: Diagramm kuvab ruudustiku eri kirjete arvu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439001"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="6caf7-102">Diagramm kuvab ruudustiku eri kirjete arvu</span><span class="sxs-lookup"><span data-stu-id="6caf7-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="6caf7-103">**Sümptom**</span><span class="sxs-lookup"><span data-stu-id="6caf7-103">**Symptom**</span></span>

<span data-ttu-id="6caf7-104">Diagrammil armatuurlaua lehel, kui klõpsate diagrammil "..." ja klõpsake nuppu "Kuva kirjed", liikuge lehele ruudustik, et näha kõiki kirjeid. Mõnikord muutub kirjete arv.</span><span class="sxs-lookup"><span data-stu-id="6caf7-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="6caf7-105">**Põhjustada**</span><span class="sxs-lookup"><span data-stu-id="6caf7-105">**Cause**</span></span>

<span data-ttu-id="6caf7-106">See on tingitud vaadete erinevusest diagrammil, mis paikneb algsel armatuurlaua lehel ja ruudustiku avalehel asuval diagrammil.</span><span class="sxs-lookup"><span data-stu-id="6caf7-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="6caf7-107">**Lahendus**</span><span class="sxs-lookup"><span data-stu-id="6caf7-107">**Solution**</span></span>

1. <span data-ttu-id="6caf7-108">Vaadake vaadet algsest lehest ja ruudustiku vaatest, et näha, kas need on teistsugused.</span><span class="sxs-lookup"><span data-stu-id="6caf7-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="6caf7-109">Muutke ruudustiku vaadet algse lehe vaatele vastavaks.</span><span class="sxs-lookup"><span data-stu-id="6caf7-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="6caf7-110">Kui õiget vaadet ei leita, tähendab see seda, et see ei ole rakenduse kujundajas lubatud.</span><span class="sxs-lookup"><span data-stu-id="6caf7-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="6caf7-111">Avage konkreetse rakenduse rakenduse kujundaja, valige olem ja selle vaated, kontrollige vaadet, mida soovite lubada, salvestada, avaldada ja sulgeda.</span><span class="sxs-lookup"><span data-stu-id="6caf7-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="6caf7-112">Värskendage lehte.</span><span class="sxs-lookup"><span data-stu-id="6caf7-112">Refresh the page.</span></span>