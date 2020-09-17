---
title: Windows 10 sõrmejälgede avamise suvandi kasutamine
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795240"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="7fa37-102">Windows 10 sõrmejälgede avamise suvandi kasutamine</span><span class="sxs-lookup"><span data-stu-id="7fa37-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="7fa37-103">**Luba Windows Hello sõrmejälg**</span><span class="sxs-lookup"><span data-stu-id="7fa37-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="7fa37-104">Kui soovite Windows 10 oma sõrmejälgede abil vabastada, peate häälestama Windows Hello sõrmejälje, lisades (lastes Windows õppima ära tundma) vähemalt ühe sõrmega.</span><span class="sxs-lookup"><span data-stu-id="7fa37-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="7fa37-105">Valige **sätted, > kontode > sisselogimise suvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="7fa37-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="7fa37-106">Saadaolevad sisselogimise suvandid on loetletud.</span><span class="sxs-lookup"><span data-stu-id="7fa37-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="7fa37-107">Näiteks.</span><span class="sxs-lookup"><span data-stu-id="7fa37-107">For example:</span></span>

    ![Sisselogimise suvandid.](media/sign-in-options.png)

2. <span data-ttu-id="7fa37-109">Klõpsake või puudutage valikut **Windows Hello sõrmejälg**ja seejärel klõpsake nuppu **Häälesta**.</span><span class="sxs-lookup"><span data-stu-id="7fa37-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="7fa37-110">Klõpsake Windowsi Hello häälestamise aknas nuppu **Alustamine**.</span><span class="sxs-lookup"><span data-stu-id="7fa37-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="7fa37-111">Sõrmejäljelugeja aktiveerub ja teil palutakse sõrm sensori ette paigutada.</span><span class="sxs-lookup"><span data-stu-id="7fa37-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sõrmejälgede andur.](media/fingerprint-sensor.png)

3. <span data-ttu-id="7fa37-113">Järgige juhiseid, mis paluvad teil sõrme korduvalt skannida.</span><span class="sxs-lookup"><span data-stu-id="7fa37-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="7fa37-114">Kui see on valmis, on teil võimalus lisada muid sõrmi, mida soovite kasutada sisselogimiseks.</span><span class="sxs-lookup"><span data-stu-id="7fa37-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="7fa37-115">Järgmine kord, kui logite sisse operatsioonisüsteemi Windows 10, on teil võimalus kasutada oma sõrmejälge.</span><span class="sxs-lookup"><span data-stu-id="7fa37-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="7fa37-116">**Windows Hello sõrmejälg pole sisselogimise suvandina saadaval**</span><span class="sxs-lookup"><span data-stu-id="7fa37-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="7fa37-117">Kui Windows Hello sõrmejälge ei kuvata **sisselogimise**suvandites, tähendab see seda, et Windows ei ole teadlik teie arvutiga ühendatud sõrmejäljelugeja/skannerist või et süsteemi poliitika takistab selle kasutamist (näiteks teie arvutit haldab teie töökoht).</span><span class="sxs-lookup"><span data-stu-id="7fa37-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="7fa37-118">Tõrkeotsingu sooritamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="7fa37-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="7fa37-119">Valige tegumiribal nupp **Start** ja otsige üles **Seadmehaldur**.</span><span class="sxs-lookup"><span data-stu-id="7fa37-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="7fa37-120">**Seadmehalduri**avamiseks klõpsake või koputage seda.</span><span class="sxs-lookup"><span data-stu-id="7fa37-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="7fa37-121">Seadmehalduris laiendage biomeetriliste seadmete klõpsamisel selle Chevron.</span><span class="sxs-lookup"><span data-stu-id="7fa37-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biomeetrilised seadmed.](media/biometric-devices.png)

4. <span data-ttu-id="7fa37-123">Teie sõrmejälgede skanner tuleks loetleda biomeetriliste seadmetena (nt Synaptics WBDI skanner).</span><span class="sxs-lookup"><span data-stu-id="7fa37-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biomeetrilised seadmed.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="7fa37-125">Kui teie sõrmejälgede skannerit ei kuvata ja skanner on teie ARVUTISSE integreeritud, avage arvuti tootja veebisait.</span><span class="sxs-lookup"><span data-stu-id="7fa37-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="7fa37-126">Otsige oma arvuti mudelist tehnilise toe jaotisest üles Windows 10 draiver skannerile, mida saate installida.</span><span class="sxs-lookup"><span data-stu-id="7fa37-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="7fa37-127">Kui skanner on PC-arvutist eraldi (lisatud USB kaudu), avage skanneri tootja veebisait, et otsida ja installida Windows 10 seadme draiveri tarkvara teie skanneri mudeli jaoks.</span><span class="sxs-lookup"><span data-stu-id="7fa37-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
