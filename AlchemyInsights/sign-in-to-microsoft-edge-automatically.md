---
title: Microsoft Edge'i automaatne sisselogimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398725"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="73be9-102">Microsoft Edge'i automaatne sisselogimine</span><span class="sxs-lookup"><span data-stu-id="73be9-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="73be9-103">Microsoft Edge kasutab operatsioonisüsteemi vaikekontot kasutaja automaatseks sisselogimiseks vastavalt kasutaja seadme konfigureerimise viisidele.</span><span class="sxs-lookup"><span data-stu-id="73be9-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="73be9-104">Allpool kirjeldatakse igat tüüpi seadme konfiguratsiooni ja sellest sõltuva kasutaja sisselogimisprotsessi stsenaariume.</span><span class="sxs-lookup"><span data-stu-id="73be9-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="73be9-105">**Seade on hübriid/AAD-J.** See suvand on saadaval opsüsteemis Windows 10, windowsi allatasemel ja vastavates serveriversioonides.</span><span class="sxs-lookup"><span data-stu-id="73be9-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="73be9-106">Kasutajad logitakse automaatselt sisse oma Azure Active Directory (AD) kontodega.</span><span class="sxs-lookup"><span data-stu-id="73be9-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="73be9-107">**Seade on domeeniga liidetud.** See suvand on saadaval Opsüsteemis Windows 10, windowsi allatasemel ja vastavates serveriversioonides.</span><span class="sxs-lookup"><span data-stu-id="73be9-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="73be9-108">Vaikimisi ei logita domeenikontodega kasutajad automaatselt sisse; nende jaoks automaatse sisselogimise lubamiseks kasutage **poliitikat ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="73be9-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="73be9-109">Azure AD-kontodega kasutajate jaoks automaatse sisselogimise lubamiseks kaaluge nende seadmete hübriidjuurutust.</span><span class="sxs-lookup"><span data-stu-id="73be9-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="73be9-110">**Os-i vaikekonto** on Microsofti konto. See suvand on saadaval opsüsteemis Windows 10 RS3 (versioon 1709, järk 10.0.16299) ja uuemates versioonides.</span><span class="sxs-lookup"><span data-stu-id="73be9-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="73be9-111">See stsenaarium ei ole ettevõtte seadmetes tõenäoline.</span><span class="sxs-lookup"><span data-stu-id="73be9-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="73be9-112">Kui aga os-i vaikekonto on Microsofti konto, logib Microsoft Edge kasutaja automaatselt sisse Microsofti kontoga.</span><span class="sxs-lookup"><span data-stu-id="73be9-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
