---
title: Kustutatud ühiskausta taastamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774527"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="acf50-102">Kustutatud ühiskausta taastamine</span><span class="sxs-lookup"><span data-stu-id="acf50-102">Restore a deleted public folder</span></span>

<span data-ttu-id="acf50-103">**Ühiskausta kustutatud üksuste taastamiseks**tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="acf50-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="acf50-104">Siit leiate teavet selle [kohta, et te ei saa Outlook 2016-s ühiskausta kustutatud üksusi taastada](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="acf50-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="acf50-105">**Kustutatud ühiskausta (mis tahes tüüpi) taastamiseks tehke**järgmist.</span><span class="sxs-lookup"><span data-stu-id="acf50-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="acf50-106">Palun kasutage järgmisi EKSO PowerShelli käsku:</span><span class="sxs-lookup"><span data-stu-id="acf50-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="acf50-107">Süntaks</span><span class="sxs-lookup"><span data-stu-id="acf50-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="acf50-108">Näide: järgmine käsk taastab Subfolder1 ja paigutab selle alla \Parent1.</span><span class="sxs-lookup"><span data-stu-id="acf50-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="acf50-109">Lisateavet leiate teemast [Kustutatud ühiskausta taastamine](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="acf50-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
