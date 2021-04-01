---
title: Microsoft Edge'i teenusekomplekti seamine vaikebrauseriks domeeniga ühendatud seadmes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491439"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="32c29-102">Microsoft Edge'i teenusekomplekti seamine vaikebrauseriks domeeniga ühendatud seadmes</span><span class="sxs-lookup"><span data-stu-id="32c29-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="32c29-103">Seadke Microsoft Edge vaikebrauseriks.</span><span class="sxs-lookup"><span data-stu-id="32c29-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="32c29-104">[Looge vaikeseose konfiguratsioonifail](https://go.microsoft.com/fwlink/?linkid=2132437) ja salvestage see kohalikult või võrgukohalt.</span><span class="sxs-lookup"><span data-stu-id="32c29-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="32c29-105">Avage rühmapoliitika redaktor ja seejärel valige Arvuti konfiguratsiooni  >  **haldusmallid**  >  **Windowsi komponendid** File  >  **Explorer.**</span><span class="sxs-lookup"><span data-stu-id="32c29-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="32c29-106">Valige **Määra vaikeseose konfiguratsioonifail.**</span><span class="sxs-lookup"><span data-stu-id="32c29-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="32c29-107">Valige **Poliitikasäte** ja seejärel **lubatud**.</span><span class="sxs-lookup"><span data-stu-id="32c29-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="32c29-108">Sisestage **jaotises** Suvandid vaikeseotud konfiguratsioonifaili asukoht ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="32c29-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
