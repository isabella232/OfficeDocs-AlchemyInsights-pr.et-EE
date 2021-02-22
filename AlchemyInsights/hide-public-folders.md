---
title: Ühiskaustade peitmine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315340"
---
# <a name="hide-public-folders"></a><span data-ttu-id="7d8aa-102">Ühiskaustade peitmine</span><span class="sxs-lookup"><span data-stu-id="7d8aa-102">Hide public folders</span></span>

<span data-ttu-id="7d8aa-103">**Terve ühiskausta puu peitmiseks** tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="7d8aa-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="7d8aa-104">[Selle](https://aka.ms/ControlPF) artikli juhiste abil saate peita terve ühiskausta puu valikuliselt või kõigilt kasutajatelt.</span><span class="sxs-lookup"><span data-stu-id="7d8aa-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="7d8aa-105">**Kindla ühiskausta peitmiseks** tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="7d8aa-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="7d8aa-106">Ühiskausta juurdepääsu vajavatele kasutajatele õiguse lisamine</span><span class="sxs-lookup"><span data-stu-id="7d8aa-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="7d8aa-107">Eemaldage kasutaja **õiguste** loendist **vaikeväärtus** :</span><span class="sxs-lookup"><span data-stu-id="7d8aa-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
