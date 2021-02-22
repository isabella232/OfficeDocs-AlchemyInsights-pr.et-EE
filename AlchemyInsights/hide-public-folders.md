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
# <a name="hide-public-folders"></a>Ühiskaustade peitmine

**Terve ühiskausta puu peitmiseks** tehke järgmist.

[Selle](https://aka.ms/ControlPF) artikli juhiste abil saate peita terve ühiskausta puu valikuliselt või kõigilt kasutajatelt.

**Kindla ühiskausta peitmiseks** tehke järgmist.

1. Ühiskausta juurdepääsu vajavatele kasutajatele õiguse lisamine

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Eemaldage kasutaja **õiguste** loendist **vaikeväärtus** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
