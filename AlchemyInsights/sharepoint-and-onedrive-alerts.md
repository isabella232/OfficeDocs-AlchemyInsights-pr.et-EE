---
title: Viivitused SharePointi ja OneDrive ' i teatiste vastuvõtmisel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727239"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="dfca2-102">Viivitused SharePointi ja OneDrive ' i teatiste vastuvõtmisel</span><span class="sxs-lookup"><span data-stu-id="dfca2-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="dfca2-103">Esmalt kontrollige meili rämpsposti kausta rämpsposti.</span><span class="sxs-lookup"><span data-stu-id="dfca2-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="dfca2-104">Kui **Kõik teatised mitmest failist või teegist on hilinenud**, leiate [teenuse tervise armatuurlaualt](https://portal.office.com/adminportal/home?ref=/servicehealth) , et kontrollida, kas SharePointis või Exchange ' is esinevad nõustajad/intsidendid on saadaval.</span><span class="sxs-lookup"><span data-stu-id="dfca2-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="dfca2-105">Probleem võib olla SharePointi teatiste võimalustega või meilisõnumite kaudu Exchange ' iga viivitatud.</span><span class="sxs-lookup"><span data-stu-id="dfca2-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="dfca2-106">Pange tähele, kas muud meilisõnumid toimetatakse kohale – kui mitte, on probleem tõenäoliselt ka Exchange ' i viivitusega.</span><span class="sxs-lookup"><span data-stu-id="dfca2-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="dfca2-107">Kui **kindla faili või teegi konkreetset teatist ei edastata**, proovige see kustutada ja uuesti luua.</span><span class="sxs-lookup"><span data-stu-id="dfca2-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="dfca2-108">Teatise uuesti loomise kohta leiate teavet teemast [SharePointi teatiste haldamine, kuvamine ja kustutamine](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="dfca2-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="dfca2-109">Teatisi ei saa leviloendile saata.</span><span class="sxs-lookup"><span data-stu-id="dfca2-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="dfca2-110">Toetatakse ainult turbe-ja O365 rühmi.</span><span class="sxs-lookup"><span data-stu-id="dfca2-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="dfca2-111">Teatise e-posti malle ei saa kohandada.</span><span class="sxs-lookup"><span data-stu-id="dfca2-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="dfca2-112">Nende saavutamiseks peate kasutama Microsoft Flow või SharePoint Designeri töövoogu.</span><span class="sxs-lookup"><span data-stu-id="dfca2-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
