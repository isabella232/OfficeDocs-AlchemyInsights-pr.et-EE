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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943371"
---
# <a name="restore-a-deleted-public-folder"></a>Kustutatud avaliku kausta taastamine

**Kustutatud üksuste taastamiseks avalikust kaustast:**

- Vt [Teemat Kustutatud üksusi ei saa](https://aka.ms/pfrec)taastada kaustas Outlook 2016.
 
**Kustutatud ühiskausta (mis tahes tüüpi) taastamiseks:** 

- Kasutage järgmist EXO PowerShelli käsku.

    Süntaks:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Näide: järgmine käsk taastab alamkausta1 ja paigutab selle jaotisesse \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Lisateavet [leiate teemast Kustutatud avaliku](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) kausta taastamine.
