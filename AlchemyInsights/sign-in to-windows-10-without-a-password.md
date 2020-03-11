---
title: Sisselogimine Windows 10 parooli kasutamata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588277"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="9fabc-102">Sisselogimine Windows 10 parooli kasutamata</span><span class="sxs-lookup"><span data-stu-id="9fabc-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="9fabc-103">Et vältida parooli sisestamist Windowsi käivitamisel, soovitame kasutada ühte Windows Hello turvalise sisselogimise suvanditest, nagu PIN-kood, näotuvastus või sõrmejälg, kui see on saadaval.</span><span class="sxs-lookup"><span data-stu-id="9fabc-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="9fabc-104">Kui soovite kindlasti turvalise sisselogimise keelata, lugege allolevaid juhiseid jaotisest "automaatselt sisse logida Windows 10".</span><span class="sxs-lookup"><span data-stu-id="9fabc-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="9fabc-105">**Secure Windows Hello alternatiivid konto parool**</span><span class="sxs-lookup"><span data-stu-id="9fabc-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="9fabc-106">Avage **sätted > kontod > Sisselogimissuvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="9fabc-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="9fabc-107">Saadaolevad Sisselogimissuvandid loetletakse.</span><span class="sxs-lookup"><span data-stu-id="9fabc-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="9fabc-108">Näiteks.</span><span class="sxs-lookup"><span data-stu-id="9fabc-108">For example:</span></span>

![Sisselogimissuvandid.](media/sign-in-options.png)

<span data-ttu-id="9fabc-110">Klõpsake või koputage selle konfigureerimiseks ühte suvandit.</span><span class="sxs-lookup"><span data-stu-id="9fabc-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="9fabc-111">Järgmisel korral, kui käivitate või avate Windowsi, saate kasutada parooli asemel uut suvandit.</span><span class="sxs-lookup"><span data-stu-id="9fabc-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="9fabc-112">**Sisselogimine automaatselt Windows 10-sse**</span><span class="sxs-lookup"><span data-stu-id="9fabc-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="9fabc-113">**Märkus**: Automaatne sisselogimine on mugav, kuid tutvustab turberiski, eriti kui teie arvutil on juurdepääs mitmele inimesele.</span><span class="sxs-lookup"><span data-stu-id="9fabc-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="9fabc-114">Klõpsake või koputage tegumiribal nuppu **Start** .</span><span class="sxs-lookup"><span data-stu-id="9fabc-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="9fabc-115">Tippige **netplwiz** ja vajuta sisenema võti kasutajakontode akna avamiseks.</span><span class="sxs-lookup"><span data-stu-id="9fabc-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="9fabc-116">Klõpsake **kasutajakontode**kontol, kuhu soovite Windowsi käivitumisel automaatselt sisse logida.</span><span class="sxs-lookup"><span data-stu-id="9fabc-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="9fabc-117">Tühjendage märkeruut "kasutajad peavad sisestama kasutajanime ja parooli selle arvuti kasutamiseks".</span><span class="sxs-lookup"><span data-stu-id="9fabc-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Kasutajad peavad sisestama kasutajanime ja parooli suvandi.](media/users-must-enter-username.png)

5. <span data-ttu-id="9fabc-119">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="9fabc-119">Click **OK**.</span></span> <span data-ttu-id="9fabc-120">Teil palutakse sisestada ja kinnitada valitud konto parool.</span><span class="sxs-lookup"><span data-stu-id="9fabc-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="9fabc-121">Lõpetamiseks klõpsake nuppu **OK** .</span><span class="sxs-lookup"><span data-stu-id="9fabc-121">Click **OK** to finish.</span></span> <span data-ttu-id="9fabc-122">Järgmine kord, kui Windows 10 käivitub, läheb see automaatselt teie valitud kontole sisse.</span><span class="sxs-lookup"><span data-stu-id="9fabc-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
