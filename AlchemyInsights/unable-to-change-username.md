---
title: Kasutajanime ei saa muuta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439099"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="25404-102">Kasutajanime ei saa muuta</span><span class="sxs-lookup"><span data-stu-id="25404-102">Unable to change UserName</span></span>

<span data-ttu-id="25404-103">Mõnel juhul ei levitata UPN-i (UserPrincipalName) muutusi pilve.</span><span class="sxs-lookup"><span data-stu-id="25404-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="25404-104">Võidakse kuvada Office 365 portaalis valideerimise tõrked või muuta kasutajanime või meiliaadressi.</span><span class="sxs-lookup"><span data-stu-id="25404-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="25404-105">Probleemi lahendamiseks seadke UserPrincipalName käsitsi selle PowerShelli käsu abil.</span><span class="sxs-lookup"><span data-stu-id="25404-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="25404-106">**Näide: kasutaja ümbernimetamine**</span><span class="sxs-lookup"><span data-stu-id="25404-106">**Example: Rename a user**</span></span>

<span data-ttu-id="25404-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="25404-107">PowerShellCopy</span></span>

<span data-ttu-id="25404-108">PS C: \> Set-MsolUserPrincipalName-userPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="25404-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="25404-109">Selle käsuga nimetatakse davidc@contoso.com davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="25404-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="25404-110">Lisateavet leiate teemast [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="25404-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>