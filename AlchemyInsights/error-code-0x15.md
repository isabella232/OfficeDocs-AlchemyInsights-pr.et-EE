---
title: Tõrkekood 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Kui Office 2013 aktiveerimisel kaugtöölaua teenuste (RDS) juurutustes kuvatakse tõrketeade, kaaluge ADAL lubamist registri redigeerimise teel.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709183"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="0d0ea-103">Office 2013 aktiveerimisel Remote Desktop Services tõrge</span><span class="sxs-lookup"><span data-stu-id="0d0ea-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="0d0ea-104">Kui Office 2013 aktiveerimisel kaugtöölaua teenuste (RDS) juurutustes kuvatakse tõrketeade, kaaluge ADAL lubamist registri redigeerimise teel.</span><span class="sxs-lookup"><span data-stu-id="0d0ea-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="0d0ea-105">**Registrivõti**</span><span class="sxs-lookup"><span data-stu-id="0d0ea-105">**Registry key**</span></span>|<span data-ttu-id="0d0ea-106">**Tüüp**</span><span class="sxs-lookup"><span data-stu-id="0d0ea-106">**Type**</span></span>|<span data-ttu-id="0d0ea-107">**Väärtus**</span><span class="sxs-lookup"><span data-stu-id="0d0ea-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0d0ea-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="0d0ea-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="0d0ea-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="0d0ea-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="0d0ea-110">1</span><span class="sxs-lookup"><span data-stu-id="0d0ea-110">1</span></span>  <br/> |

<span data-ttu-id="0d0ea-111">Lisateavet leiate teemast [Office 2013 modernse autentimise lubamine Windowsi seadmetes](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="0d0ea-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="0d0ea-112">Microsoft 365 rakendustes Enterprise and Office 2016 on ADAL vaikimisi lubatud.</span><span class="sxs-lookup"><span data-stu-id="0d0ea-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="0d0ea-113">Kaugtöölaua teenused (RDS) kasutasid varem terminaliteenuste nime.</span><span class="sxs-lookup"><span data-stu-id="0d0ea-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  