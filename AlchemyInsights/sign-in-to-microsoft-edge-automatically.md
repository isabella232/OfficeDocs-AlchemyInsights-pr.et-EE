---
title: Logige Microsoft Edge ' i automaatselt sisse
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677235"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="b4dbe-102">Logige Microsoft Edge ' i automaatselt sisse</span><span class="sxs-lookup"><span data-stu-id="b4dbe-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="b4dbe-103">Microsoft Edge kasutab OPERATSIOONISÜSTEEMI vaikesätet automaatselt kasutaja sisselogimiseks vastavalt sellele, kuidas kasutaja seade on konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="b4dbe-104">Iga tüüpi seadme konfiguratsiooni ja selle sõltuva kasutaja sisselogimise stsenaariumid on kirjeldatud allpool.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="b4dbe-105">**Seade on hübriid/AAD-J**: see suvand on saadaval opsüsteemis Windows 10, ülataseme Windowsi ja vastavate serveri versioonide korral.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="b4dbe-106">Kasutajad logitakse automaatselt sisse oma Azure Active Directory (AD) kontodega.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="b4dbe-107">**Seade on domeeniga liitunud**: see suvand on saadaval opsüsteemis Windows 10, Downi Windowsi ja vastavate serveri versioonide korral.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="b4dbe-108">Vaikimisi ei logita domeeni kontode kasutajad automaatselt sisse; automaatse sisselogimise lubamiseks kasutage **ConfigureOnPremisesAccountAutoSignIn** poliitikat.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="b4dbe-109">Azure AD Accounts kasutajate automaatse sisselogimise lubamiseks kaaluge hübriidiga liitumist oma seadmetega.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="b4dbe-110">**Operatsioonisüsteemi vaikekonto on Microsofti konto**: see suvand on saadaval opsüsteemis Windows 10 RS3 (versioon 1709, järk 10.0.16299) ja uuemates versioonides.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="b4dbe-111">Stsenaarium ei esine tõenäoliselt Enterprise Devices.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="b4dbe-112">Kui aga OS-i vaikekonto on Microsofti konto, logib Microsoft Edge kasutaja automaatselt sisse Microsofti kontoga.</span><span class="sxs-lookup"><span data-stu-id="b4dbe-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
