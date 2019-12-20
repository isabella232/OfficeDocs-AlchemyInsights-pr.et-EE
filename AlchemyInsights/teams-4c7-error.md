---
title: Meeskonnad 4c7 viga
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796072"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="ea8ea-102">4c7 tõrge Microsoft Teamsi</span><span class="sxs-lookup"><span data-stu-id="ea8ea-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="ea8ea-103">See tõrge ilmneb seetõttu, et Microsoft Teams nõuab vormide autentimist.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="ea8ea-104">Kui juurutate Active Directory Federation Services (AD FS), vormide autentimine on lubatud sisevõrgu vaikimisi.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="ea8ea-105">Kui Windowsi integreeritud autentimine nurjub, palutakse teil vormide autentimise abil sisse logida.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="ea8ea-106">Selle probleemi lahendamiseks lubage vormide autentimine AD FS Microsofti halduskonsooli (MMC) lisandmooduli abil arvutis, millel on Active Directory kohaliku koopia.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="ea8ea-107">Selleks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="ea8ea-108">Liikuge navigeerimispaanil **autentimise poliitikad**.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="ea8ea-109">Tehke jaotises üksikasjade paanil **toimingud** valik **Redigeeri globaalset esmast autentimist**.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="ea8ea-110">Valige vahekaardil **sisevõrgu** **vormide autentimine**.</span><span class="sxs-lookup"><span data-stu-id="ea8ea-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="ea8ea-111">Valige **OK** (või **Rakenda**).</span><span class="sxs-lookup"><span data-stu-id="ea8ea-111">Select **OK** (or **Apply**).</span></span>