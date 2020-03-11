---
title: Sõrmejälje avamise suvandi kasutamine Windows 10-s
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588312"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="91eb1-102">Sõrmejälje avamise suvandi kasutamine Windows 10-s</span><span class="sxs-lookup"><span data-stu-id="91eb1-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="91eb1-103">**Luba Windows Hello sõrmejälg**</span><span class="sxs-lookup"><span data-stu-id="91eb1-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="91eb1-104">Windows 10 avamiseks sõrmejälje abil peate seadistama Windows Hello sõrmejälje, lisades (lastes Windowsil seda ära tunda) vähemalt üks sõrm.</span><span class="sxs-lookup"><span data-stu-id="91eb1-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="91eb1-105">Avage **sätted > kontod > Sisselogimissuvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="91eb1-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="91eb1-106">Saadaolevad Sisselogimissuvandid loetletakse.</span><span class="sxs-lookup"><span data-stu-id="91eb1-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="91eb1-107">Näiteks.</span><span class="sxs-lookup"><span data-stu-id="91eb1-107">For example:</span></span>

    ![Sisselogimissuvandid.](media/sign-in-options.png)

2. <span data-ttu-id="91eb1-109">Klõpsake või koputage **Windows Hello sõrmejälg**, seejärel klõpsake nuppu **Seadista**.</span><span class="sxs-lookup"><span data-stu-id="91eb1-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="91eb1-110">Klõpsake aknas Windows Hello häälestus **nuppu Alusta.**</span><span class="sxs-lookup"><span data-stu-id="91eb1-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="91eb1-111">Sõrmejäljeandur aktiveeritakse ja teil palutakse panna sõrm sensoril:</span><span class="sxs-lookup"><span data-stu-id="91eb1-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sõrmejälje andur.](media/fingerprint-sensor.png)

3. <span data-ttu-id="91eb1-113">Järgige juhiseid, mis palub teil oma sõrme korduvalt skannida.</span><span class="sxs-lookup"><span data-stu-id="91eb1-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="91eb1-114">Kui see on lõppenud, on teil võimalus lisada muid sõrmi, mida võiksite sisselogimiseks kasutada.</span><span class="sxs-lookup"><span data-stu-id="91eb1-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="91eb1-115">Järgmine kord, kui logite sisse Windows 10, on teil võimalus kasutada oma sõrmejälg seda teha.</span><span class="sxs-lookup"><span data-stu-id="91eb1-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="91eb1-116">**Windows Hello sõrmejälg pole sisselogimissuvandiga saadaval**</span><span class="sxs-lookup"><span data-stu-id="91eb1-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="91eb1-117">Kui Windows Hello sõrmejälge ei kuvata **Sisselogimissuvandite**suvandiga, tähendab see, et Windows ei tea ühtegi teie arvutiga ühendatud sõrmejäljelugejat/skannerit või süsteemipoliitika takistab selle kasutamist (nt teie arvuti haldab teie töökoht).</span><span class="sxs-lookup"><span data-stu-id="91eb1-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="91eb1-118">Tõrkeotsingu sooritamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="91eb1-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="91eb1-119">Valige tegumiribal nupp **Start** ja otsige **seadmehaldurit**.</span><span class="sxs-lookup"><span data-stu-id="91eb1-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="91eb1-120">Klõpsake või koputage **Seadmehalduri**avamiseks.</span><span class="sxs-lookup"><span data-stu-id="91eb1-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="91eb1-121">Laiendage Seadmehalduris biomeetrilisi seadmeid, klõpsates selle glüüfi.</span><span class="sxs-lookup"><span data-stu-id="91eb1-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biomeetrilised seadmed.](media/biometric-devices.png)

4. <span data-ttu-id="91eb1-123">Sõrmejäljelugeja tuleks loetleda biomeetrilise seadena (nt Synaptics WBDI skanner):</span><span class="sxs-lookup"><span data-stu-id="91eb1-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biomeetrilised seadmed.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="91eb1-125">Kui sõrmejäljelugeja ei kuvata ja skanner on arvutisse integreeritud, arvuti tootja veebisaidile.</span><span class="sxs-lookup"><span data-stu-id="91eb1-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="91eb1-126">Otsige oma arvuti mudeli tehnilise toe sektsioonis üles Windows 10 draiver skanneri jaoks, mida saate installida.</span><span class="sxs-lookup"><span data-stu-id="91eb1-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="91eb1-127">Kui skanner on ARVUTIST eraldi (manustatud USB kaudu), skanneri tootja veebisaidile, et leida ja installida Windows 10 seadmedraiveri tarkvara teie skanneri mudelile.</span><span class="sxs-lookup"><span data-stu-id="91eb1-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
