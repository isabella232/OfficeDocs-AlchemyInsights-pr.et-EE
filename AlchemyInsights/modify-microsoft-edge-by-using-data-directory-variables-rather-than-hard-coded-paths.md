---
title: Microsoft Edge ' i muutmine, kasutades andmete kataloogi muutujaid, mitte kõva koodiga teed
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035283"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="2b27c-102">Microsoft Edge ' i muutmine, kasutades andmete kataloogi muutujaid, mitte kõva koodiga teed</span><span class="sxs-lookup"><span data-stu-id="2b27c-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="2b27c-103">Kui soovite näiteks Windowsis talletada andmed kasutajate kohaliku rakenduse andmete alusel, mitte vaikeasukohta, määrake *UserDataDir* poliitikaks **$ {local_app_data} \Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="2b27c-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="2b27c-104">Lisateavet leiate teemast [Microsoft Edge ' i kasutajate andmete kataloogi muutujate loomine](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span><span class="sxs-lookup"><span data-stu-id="2b27c-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>