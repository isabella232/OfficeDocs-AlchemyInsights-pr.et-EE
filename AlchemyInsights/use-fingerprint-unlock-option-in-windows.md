---
title: Sõrmejälje lukust vabastamise suvandi kasutamine opsüsteemis Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796673"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="a2b35-102">Sõrmejälje lukust vabastamise suvandi kasutamine opsüsteemis Windows 10</span><span class="sxs-lookup"><span data-stu-id="a2b35-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="a2b35-103">**Luba Windows Hello sõrmejälg**</span><span class="sxs-lookup"><span data-stu-id="a2b35-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="a2b35-104">Windows 10 avamiseks sõrmejälje abil peate häälestama Windows Hello sõrmejälje, lisades (lastes Windowsil ära tunda) vähemalt ühe sõrme.</span><span class="sxs-lookup"><span data-stu-id="a2b35-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="a2b35-105">Avage **Sätted > Kontod > sisselogimissuvandid** (või klõpsake [siin).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="a2b35-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="a2b35-106">Kuvatakse saadaolevad sisselogimissuvandid.</span><span class="sxs-lookup"><span data-stu-id="a2b35-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="a2b35-107">Näide.</span><span class="sxs-lookup"><span data-stu-id="a2b35-107">For example:</span></span>

    ![Sisselogimissuvandid.](media/sign-in-options.png)

2. <span data-ttu-id="a2b35-109">Klõpsake või **puudutage valikut Windows Hello Fingerprint (Windows Hello sõrmejälg)** ja **seejärel nuppu Set up (Häälesta).**</span><span class="sxs-lookup"><span data-stu-id="a2b35-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="a2b35-110">Klõpsake Windows Hello häälestusaknas **nuppu Alustamine.**</span><span class="sxs-lookup"><span data-stu-id="a2b35-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="a2b35-111">Sõrmejäljeandur aktiveeritakse ja teil palutakse sõrm andurile asetada.</span><span class="sxs-lookup"><span data-stu-id="a2b35-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Sõrmejäljeandur.](media/fingerprint-sensor.png)

3. <span data-ttu-id="a2b35-113">Järgige juhiseid, mis paluvad teil sõrme korduvalt skannida.</span><span class="sxs-lookup"><span data-stu-id="a2b35-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="a2b35-114">Kui see on valmis, saate lisada muid sõrmi, mida soovite sisselogimiseks kasutada.</span><span class="sxs-lookup"><span data-stu-id="a2b35-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="a2b35-115">Järgmine kord, kui logite windows 10 sisse, saate selleks kasutada oma sõrmejälge.</span><span class="sxs-lookup"><span data-stu-id="a2b35-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="a2b35-116">**Windows Hello sõrmejälg pole sisselogimissuvandina saadaval**</span><span class="sxs-lookup"><span data-stu-id="a2b35-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="a2b35-117">Kui Windows Hello sõrmejälge ei kuvata sisselogimissuvandites suvandina, siis tähendab see, et Windows ei tea teie arvutile manustatud sõrmejäljelugejat/skannerit või et süsteemipoliitika takistab selle kasutamist (nt teie arvutit haldab teie töökoht).</span><span class="sxs-lookup"><span data-stu-id="a2b35-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="a2b35-118">Tõrkeotsinguks tehke seda.</span><span class="sxs-lookup"><span data-stu-id="a2b35-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="a2b35-119">Valige **tegumiribal** nupp Start ja otsige **seadmehaldurit.**</span><span class="sxs-lookup"><span data-stu-id="a2b35-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="a2b35-120">Klõpsake või puudutage **seadmehalduri avamiseks.**</span><span class="sxs-lookup"><span data-stu-id="a2b35-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="a2b35-121">Laiendage seadmehalduris valikut Biomeetrilised seadmed, klõpsates selle rööpnoolt.</span><span class="sxs-lookup"><span data-stu-id="a2b35-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biomeetrilised seadmed.](media/biometric-devices.png)

4. <span data-ttu-id="a2b35-123">Teie sõrmejäljeskanner peaks olema loetletud biomeetrilise seadmena (nt Synaptics WBDI skanner).</span><span class="sxs-lookup"><span data-stu-id="a2b35-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biomeetrilised seadmed.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="a2b35-125">Kui teie sõrmejäljeskannerit ei kuvata ja skanner on arvutisse integreeritud, minge arvuti tootja veebisaidile.</span><span class="sxs-lookup"><span data-stu-id="a2b35-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="a2b35-126">Otsige arvutimudeli tehnilise toe jaotisest windows 10 draiverit, mille saate installida.</span><span class="sxs-lookup"><span data-stu-id="a2b35-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="a2b35-127">Kui skanner on arvutist eraldi (usb-seadme kaudu manustatud), minge skanneri tootja veebisaidile, et leida ja installida Windows 10 seadmedraiveri tarkvara teie skannerimudeli jaoks.</span><span class="sxs-lookup"><span data-stu-id="a2b35-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
