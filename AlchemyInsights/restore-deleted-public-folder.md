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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="61c94-102">Kustutatud ühiskausta taastamine</span><span class="sxs-lookup"><span data-stu-id="61c94-102">Restore a deleted public folder</span></span>

<span data-ttu-id="61c94-103">**Ühiskausta kustutatud üksuste taastamiseks**toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="61c94-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="61c94-104">Vaadake [, te ei saa taastada kustutatud üksuste e-posti ühiskausta Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="61c94-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="61c94-105">**Kustutatud ühiskausta (mis tahes tüüpi) taastamiseks**toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="61c94-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="61c94-106">Palun kasutage EXO PowerShelli käsk:</span><span class="sxs-lookup"><span data-stu-id="61c94-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="61c94-107">Süntaks:</span><span class="sxs-lookup"><span data-stu-id="61c94-107">Syntax:</span></span>

    ><span data-ttu-id="61c94-108">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nimi-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. identiteedi-tee \<tee, kus kaust taastatakse></span><span class="sxs-lookup"><span data-stu-id="61c94-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="61c94-109">Näide: järgmine käsk taastab Subfolder1 ja asetage see \Parent1:</span><span class="sxs-lookup"><span data-stu-id="61c94-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="61c94-110">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Nimi-EQ "Subfolder1"}; Set-PublicFolder $pf. identiteedi-tee \Parent1</span><span class="sxs-lookup"><span data-stu-id="61c94-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="61c94-111">Lisateabe saamiseks vaadake [Kustutatud ühiskausta taastamine](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="61c94-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
