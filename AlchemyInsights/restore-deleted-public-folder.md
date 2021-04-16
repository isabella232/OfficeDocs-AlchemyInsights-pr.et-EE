---
title: Kustutatud avaliku kausta taastamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809435"
---
# <a name="restore-a-deleted-public-folder"></a>Kustutatud avaliku kausta taastamine

**Kustutatud üksuste taastamiseks avalikust kaustast:**

- Vaadake [teemat Kustutatud üksusi ei saa rakenduses Outlook 2016 mittepostitavast avalikust kaustast taastada.](https://aka.ms/pfrec)
 
**Kustutatud ühiskausta (mis tahes tüüpi) taastamiseks:** 

- Kasutage järgmist EXO PowerShelli käsku.

    Süntaks:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Näide: järgmine käsk taastab alamkausta1 ja paigutab selle jaotisesse \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lisateavet [leiate teemast Kustutatud avaliku](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) kausta taastamine.
