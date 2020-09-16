---
title: Windows 10 sisselogimine parooliga kasutamata
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719949"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="fbab1-102">Windows 10 sisselogimine parooliga kasutamata</span><span class="sxs-lookup"><span data-stu-id="fbab1-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="fbab1-103">Et vältida parooli tippimist Windowsi käivitamisel, soovitame kasutada ühte Windows Hello turvalist sisselogimise suvandit (nt PIN-koodi, näo tuvastust või sõrmejälge), kui see on saadaval.</span><span class="sxs-lookup"><span data-stu-id="fbab1-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="fbab1-104">Kui soovite kindlasti turvalise sisselogimise keelata, lugege allpool olevat jaotist "Automaatne sisselogimine opsüsteemi Windows 10".</span><span class="sxs-lookup"><span data-stu-id="fbab1-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="fbab1-105">**Turvaliste Windows Hello alternatiivid konto parooli**</span><span class="sxs-lookup"><span data-stu-id="fbab1-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="fbab1-106">Valige **sätted, > kontode > sisselogimise suvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="fbab1-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="fbab1-107">Saadaolevad sisselogimise suvandid on loetletud.</span><span class="sxs-lookup"><span data-stu-id="fbab1-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="fbab1-108">Näiteks.</span><span class="sxs-lookup"><span data-stu-id="fbab1-108">For example:</span></span>

![Sisselogimise suvandid.](media/sign-in-options.png)

<span data-ttu-id="fbab1-110">Selle konfigureerimiseks klõpsake või puudutage mõnda suvandit.</span><span class="sxs-lookup"><span data-stu-id="fbab1-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="fbab1-111">Järgmine kord, kui käivitate või avate Windowsi, saate parooli asemel kasutada uut suvandit.</span><span class="sxs-lookup"><span data-stu-id="fbab1-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="fbab1-112">**Windows 10 automaatne sisselogimine**</span><span class="sxs-lookup"><span data-stu-id="fbab1-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="fbab1-113">**Märkus**: Automaatne sisselogimine on otstarbekas, kuid see tutvustab turvariski, eriti juhul, kui teie arvuti on juurdepääsetav mitmele inimesele.</span><span class="sxs-lookup"><span data-stu-id="fbab1-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="fbab1-114">Klõpsake või puudutage tegumiribal nuppu **Start** .</span><span class="sxs-lookup"><span data-stu-id="fbab1-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="fbab1-115">Tippige **netplwiz** ja vajutage akna Kasutajakontod avamiseks sisestusklahvi (ENTER).</span><span class="sxs-lookup"><span data-stu-id="fbab1-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="fbab1-116">Klõpsake jaotises **kasutajakontod**kontot, millele soovite Windowsi käivitumisel automaatselt sisse logida.</span><span class="sxs-lookup"><span data-stu-id="fbab1-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="fbab1-117">Tühjendage ruut "kasutajad peavad selle arvuti kasutamiseks sisestama kasutajanime ja parooli".</span><span class="sxs-lookup"><span data-stu-id="fbab1-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Kasutajad peavad sisestama suvandi kasutajanimi ja parool.](media/users-must-enter-username.png)

5. <span data-ttu-id="fbab1-119">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="fbab1-119">Click **OK**.</span></span> <span data-ttu-id="fbab1-120">Teil palutakse valitud konto parool sisestada ja kinnitada.</span><span class="sxs-lookup"><span data-stu-id="fbab1-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="fbab1-121">Lõpuleviimiseks klõpsake nuppu **OK** .</span><span class="sxs-lookup"><span data-stu-id="fbab1-121">Click **OK** to finish.</span></span> <span data-ttu-id="fbab1-122">Järgmine kord, kui Windows 10 käivitub, logib see automaatselt sisse teie valitud kontole.</span><span class="sxs-lookup"><span data-stu-id="fbab1-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
