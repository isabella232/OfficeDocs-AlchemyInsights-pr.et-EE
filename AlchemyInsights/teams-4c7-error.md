---
title: Teams 4c7 tõrge
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786665"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="de65c-102">4c7 tõrge Microsoft Teamsis</span><span class="sxs-lookup"><span data-stu-id="de65c-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="de65c-103">See tõrge ilmneb seetõttu, et Microsoft Teams nõuab vormide autentimist.</span><span class="sxs-lookup"><span data-stu-id="de65c-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="de65c-104">Teenuse Active Directory Federation Services (AD FS) juurutamisel pole vormide autentimine sisevõrgu jaoks vaikimisi lubatud.</span><span class="sxs-lookup"><span data-stu-id="de65c-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="de65c-105">Kui Windowsi integreeritud autentimine nurjub, palutakse teil vormide autentimise abil sisse logida.</span><span class="sxs-lookup"><span data-stu-id="de65c-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="de65c-106">Probleemi lahendamiseks lubage vormide autentimine AD FS-i Microsofti halduskonsooli (MMC) lisandmooduli abil arvutis, kus on Active Directory kohalik koopia.</span><span class="sxs-lookup"><span data-stu-id="de65c-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="de65c-107">Selleks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="de65c-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="de65c-108">Liikuge navigeerimispaanil sirvides jaotisesse **Autentimispoliitikad.**</span><span class="sxs-lookup"><span data-stu-id="de65c-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="de65c-109">Valige **üksikasjapaani** jaotises Toimingud käsk **Redigeeri globaalset primaarautentimist**.</span><span class="sxs-lookup"><span data-stu-id="de65c-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="de65c-110">Valige vahekaardil **Sisevõrk** suvand Vormide **autentimine**.</span><span class="sxs-lookup"><span data-stu-id="de65c-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="de65c-111">Valige **OK** (või **Rakenda).**</span><span class="sxs-lookup"><span data-stu-id="de65c-111">Select **OK** (or **Apply**).</span></span>