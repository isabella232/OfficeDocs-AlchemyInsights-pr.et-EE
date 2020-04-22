---
title: Tõrkekood 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Kui te saate viga aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluge ADAL lubamine registri redigeerimisel.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703134"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="3ae89-103">Tõrge Office 2013 aktiveerimine kaugtöölaua teenuste</span><span class="sxs-lookup"><span data-stu-id="3ae89-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="3ae89-104">Kui te saate viga aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluge ADAL lubamine registri redigeerimisel.</span><span class="sxs-lookup"><span data-stu-id="3ae89-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="3ae89-105">**Registri võti**</span><span class="sxs-lookup"><span data-stu-id="3ae89-105">**Registry key**</span></span>|<span data-ttu-id="3ae89-106">**Tüüp**</span><span class="sxs-lookup"><span data-stu-id="3ae89-106">**Type**</span></span>|<span data-ttu-id="3ae89-107">**Väärtus**</span><span class="sxs-lookup"><span data-stu-id="3ae89-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3ae89-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="3ae89-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="3ae89-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="3ae89-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="3ae89-110">1</span><span class="sxs-lookup"><span data-stu-id="3ae89-110">1</span></span>  <br/> |

<span data-ttu-id="3ae89-111">Lisateabe saamiseks vaadake [lubamine kaasaegne autentimine Office 2013 Windowsi seadmetes](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="3ae89-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="3ae89-112">ADAL on vaikimisi lubatud Microsoft 365 apps Enterprise ja Office 2016.</span><span class="sxs-lookup"><span data-stu-id="3ae89-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="3ae89-113">Kaugtöölaua teenuste (RDS) oli varem nimega Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="3ae89-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  