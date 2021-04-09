---
title: OneDrive 0x8004de40 i tõrke lahendamiseks
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649744"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="107ce-102">OneDrive 0x8004de40 i tõrke lahendamiseks</span><span class="sxs-lookup"><span data-stu-id="107ce-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="107ce-103">Kui kasutate opsüsteemi Windows 7 ja teile kuvatakse see tõrketeade, värskendage [Windowsis WinHTTP-s TLS 1.1 ja TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)lubamiseks turvaliste vaikeprotokollidena.</span><span class="sxs-lookup"><span data-stu-id="107ce-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="107ce-104">Kui kasutate opsüsteemi Windows 10 ja teile kuvatakse OneDrive'0x8004de40 tõrketeade:</span><span class="sxs-lookup"><span data-stu-id="107ce-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="107ce-105">Taaskäivitage mõjutatud arvuti, kui see on ühendatud teie Acitve'i kataloogi domeeniga.</span><span class="sxs-lookup"><span data-stu-id="107ce-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="107ce-106">Kui taaskäivitamine probleemi ei lahenda, lülitage seade Azure AD-st välja ja ühinege uuesti.</span><span class="sxs-lookup"><span data-stu-id="107ce-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="107ce-107">**Märkus.** Neid toiminguid tehes peaksite olema oma ettevõtte võrgus.</span><span class="sxs-lookup"><span data-stu-id="107ce-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="107ce-108">Ärge tehke neid toiminguid, kui te pole ühendatud oma ettevõtte taristuga (nt reisil olles).</span><span class="sxs-lookup"><span data-stu-id="107ce-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="107ce-109">Avage laiendatud käsuviip, valides **Start**, paremklõpsake käsku **Käsuviip** ja seejärel valige **Käivita administraatorina**.</span><span class="sxs-lookup"><span data-stu-id="107ce-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="107ce-110">Tippige *dsregcmd /leave ja vajutage* sisestusklahvi **(Enter).**</span><span class="sxs-lookup"><span data-stu-id="107ce-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="107ce-111">Kui see on valmis, tippige *dsregcmd /join ja* vajutage sisestusklahvi **(Enter).**</span><span class="sxs-lookup"><span data-stu-id="107ce-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="107ce-112">Kui see on valmis, sulgege käsuviip.</span><span class="sxs-lookup"><span data-stu-id="107ce-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="107ce-113">Taaskäivitage arvuti ja logige sisse OneDrive'i.</span><span class="sxs-lookup"><span data-stu-id="107ce-113">Reboot the computer, and log into OneDrive.</span></span>