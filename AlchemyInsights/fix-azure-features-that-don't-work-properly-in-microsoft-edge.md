---
title: Mida teha, kui Azure ' i funktsioonid ei tööta Microsoft Edge ' is õigesti
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583306"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="65e7e-102">Mida teha, kui Azure ' i funktsioonid ei tööta Microsoft Edge ' is õigesti</span><span class="sxs-lookup"><span data-stu-id="65e7e-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="65e7e-103">Microsoft Edge ' il on [teadaolevad probleemid](https://go.microsoft.com/fwlink/?linkid=2140608) , mis on seotud turvatsooni ja võivad mõjutada seda, kuidas Azure ' i kasutajad Windows halduskeskus sisse logivad.</span><span class="sxs-lookup"><span data-stu-id="65e7e-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="65e7e-104">Kui teil on probleeme Azure ' i funktsioonide kasutamisega Microsoft Edge ' i abil, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="65e7e-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="65e7e-105">Otsige menüüs **Start** üles **Interneti-suvandid** ja valige see.</span><span class="sxs-lookup"><span data-stu-id="65e7e-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="65e7e-106">Valige dialoogiboksis **Interneti-atribuudid** vahekaart **Turve** .</span><span class="sxs-lookup"><span data-stu-id="65e7e-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="65e7e-107">Valige **usaldusväärsete saitide** tsoon ja seejärel klõpsake nuppu **saidid** .</span><span class="sxs-lookup"><span data-stu-id="65e7e-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="65e7e-108">Lisage dialoogiboksis **Usaldusväärsed saidid** oma LÜÜSi URL, samuti [https://login.microsoftonline.com](https://login.microsoftonline.com) ja [https://login.live.com](https://login.live.com) seejärel valige **Sule**.</span><span class="sxs-lookup"><span data-stu-id="65e7e-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="65e7e-109">Valige dialoogiboksis **Interneti-atribuudid** vahekaart **Privaatsus** .</span><span class="sxs-lookup"><span data-stu-id="65e7e-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="65e7e-110">Valige jaotises **hüpikakende blokeerija** nupp **sätted**.</span><span class="sxs-lookup"><span data-stu-id="65e7e-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="65e7e-111">Lisage avanevas dialoogiboksis oma lüüsi URL, samuti [https://login.microsoftonline.com](https://login.microsoftonline.com) ja ja [https://login.live.com](https://login.live.com) seejärel valige **Sule**.</span><span class="sxs-lookup"><span data-stu-id="65e7e-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
