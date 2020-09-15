---
title: Teamsi 4c7 tõrge
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700199"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="3e441-102">Microsoft Teamsi 4c7 tõrge</span><span class="sxs-lookup"><span data-stu-id="3e441-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="3e441-103">See tõrge ilmneb, sest Microsoft Teamsi jaoks on vaja vorme autentida.</span><span class="sxs-lookup"><span data-stu-id="3e441-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="3e441-104">Kui juurutate Active Directory Federation Services (AD FS), pole vormide autentimine vaikimisi sisevõrgu jaoks lubatud.</span><span class="sxs-lookup"><span data-stu-id="3e441-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="3e441-105">Kui Windowsi integreeritud autentimine nurjub, palutakse teil vormide autentimise abil sisse logida.</span><span class="sxs-lookup"><span data-stu-id="3e441-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="3e441-106">Selle probleemi lahendamiseks lubage vormide autentimine, kasutades AD FS-i Microsoft Management Console (MMC) lisandmoodulit arvutis, kus on Active Directory kohalik koopia.</span><span class="sxs-lookup"><span data-stu-id="3e441-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="3e441-107">Selleks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="3e441-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="3e441-108">Liikuge navigeerimispaanil sirvides **autentimise poliitikale**.</span><span class="sxs-lookup"><span data-stu-id="3e441-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="3e441-109">Valige üksikasjade paani jaotises **toimingud** nupp **Redigeeri globaalset esmast autentimist**.</span><span class="sxs-lookup"><span data-stu-id="3e441-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="3e441-110">Valige vahekaardil **sisevõrk** suvand **vormide autentimine**.</span><span class="sxs-lookup"><span data-stu-id="3e441-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="3e441-111">Valige **OK** (või **Rakenda**).</span><span class="sxs-lookup"><span data-stu-id="3e441-111">Select **OK** (or **Apply**).</span></span>