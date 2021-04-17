---
title: Windows 10 sisselogimine ilma paroolita
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830542"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="7bc9b-102">Windows 10 sisselogimine ilma paroolita</span><span class="sxs-lookup"><span data-stu-id="7bc9b-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="7bc9b-103">Windowsi käivitamisel parooli tippimise vältimiseks soovitame kasutada ühte Windows Hello turvalist sisselogimissuvandeid (nt PIN-kood, näotuvastus või sõrmejälg), kui see on saadaval.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="7bc9b-104">Kui soovite turvalise sisselogimise keelata, lugege allpool toodud juhiseid "Logi automaatselt windows 10 sisse".</span><span class="sxs-lookup"><span data-stu-id="7bc9b-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="7bc9b-105">**Secure Windows Hello alternatives to the account password**</span><span class="sxs-lookup"><span data-stu-id="7bc9b-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="7bc9b-106">Avage **Sätted > Kontod > sisselogimissuvandid** (või klõpsake [siin).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="7bc9b-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="7bc9b-107">Kuvatakse saadaolevad sisselogimissuvandid.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="7bc9b-108">Näide.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-108">For example:</span></span>

![Sisselogimissuvandid.](media/sign-in-options.png)

<span data-ttu-id="7bc9b-110">Konfigureerimiseks klõpsake või puudutage ühte suvanditest.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="7bc9b-111">Järgmine kord, kui käivitate või avate Windowsi, saate parooli asemel kasutada uut suvandit.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="7bc9b-112">**Windows 10 automaatne sisselogimine**</span><span class="sxs-lookup"><span data-stu-id="7bc9b-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="7bc9b-113">**Märkus.** Automaatne sisselogimine on mugav, kuid see kehtestab turberiski, eriti juhul, kui teie arvutile pääsevad juurde mitu inimest.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="7bc9b-114">Klõpsake või **puudutage tegumiribal** nuppu Start.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="7bc9b-115">Tippige **netplwiz** ja vajutage akna Kasutajakontod avamiseks sisestusklahvi (Enter).</span><span class="sxs-lookup"><span data-stu-id="7bc9b-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="7bc9b-116">Klõpsake **kaustas Kasutajakontod** kontot, kuhu soovite Windowsi käivitamisel automaatselt sisse logida.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="7bc9b-117">Tühjendage ruut "Kasutajad peavad selle arvuti kasutamiseks sisestama kasutajanime ja parooli".</span><span class="sxs-lookup"><span data-stu-id="7bc9b-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Kasutajad peavad sisestama kasutajanime ja parooli suvandi.](media/users-must-enter-username.png)

5. <span data-ttu-id="7bc9b-119">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-119">Click **OK**.</span></span> <span data-ttu-id="7bc9b-120">Teil palutakse sisestada ja kinnitada valitud konto parool.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="7bc9b-121">Lõpetamiseks klõpsake nuppu **OK.**</span><span class="sxs-lookup"><span data-stu-id="7bc9b-121">Click **OK** to finish.</span></span> <span data-ttu-id="7bc9b-122">Järgmine kord, kui Windows 10 käivitub, logitakse see automaatselt teie valitud kontole sisse.</span><span class="sxs-lookup"><span data-stu-id="7bc9b-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
