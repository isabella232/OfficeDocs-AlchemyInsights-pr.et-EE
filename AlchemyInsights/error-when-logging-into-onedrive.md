---
title: OneDrive ' i käivitamisel ilmneb 0x8004de40 tõrge
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823018"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="68b7b-102">OneDrive ' i käivitamisel ilmneb 0x8004de40 tõrge</span><span class="sxs-lookup"><span data-stu-id="68b7b-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="68b7b-103">Kui OneDrive ' i sisselogimisel ilmneb tõrge **0x8004de40** , taaskäivitage arvuti töö või kooli domeeniga ühendatud.</span><span class="sxs-lookup"><span data-stu-id="68b7b-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="68b7b-104">Kui tõrketeade kuvatakse pärast taaskäivitamist, proovige seda siis, kui olete oma töö või kooli domeeniga ühendatud.</span><span class="sxs-lookup"><span data-stu-id="68b7b-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="68b7b-105">Klõpsake nuppu Start ja **Tippige väljale Otsing** tekst **cmd** või Käsuviip, paremklõpsake käsuviiba rakendust ja valige **Käivita administraatorina** .</span><span class="sxs-lookup"><span data-stu-id="68b7b-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="68b7b-106">Kui teilt küsitakse administraatori parooli või kinnitust, tippige parool või klõpsake nuppu **Luba** .</span><span class="sxs-lookup"><span data-stu-id="68b7b-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="68b7b-107">Tippige käsuviiba aknas **dsregcmd/Leave**  ja oodake, kuni käsk on täidetud.</span><span class="sxs-lookup"><span data-stu-id="68b7b-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="68b7b-108">Seejärel tippige **dsregcmd/JOIN** ja oodake, kuni käsk on täidetud.</span><span class="sxs-lookup"><span data-stu-id="68b7b-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="68b7b-109">Taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="68b7b-109">Reboot your computer.</span></span>
