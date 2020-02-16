---
title: Kustutatud ühiskausta taastamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063634"
---
# <a name="restore-a-deleted-public-folder"></a>Kustutatud ühiskausta taastamine

**Ühiskausta kustutatud üksuste taastamiseks**toimige järgmiselt.

- Vaadake [, te ei saa taastada kustutatud üksuste e-posti ühiskausta Outlook 2016](https://aka.ms/pfrec).
 
**Kustutatud ühiskausta (mis tahes tüüpi) taastamiseks**toimige järgmiselt. 

- Palun kasutage EXO PowerShelli käsk:

    Süntaks:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nimi-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. identiteedi-tee \<tee, kus kaust taastatakse>

    Näide: järgmine käsk taastab Subfolder1 ja asetage see \Parent1:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nimi-EQ "Subfolder1"}; Set-PublicFolder $pf. identiteedi-tee \Parent1

Lisateabe saamiseks vaadake [Kustutatud ühiskausta taastamine](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
