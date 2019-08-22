---
title: Tõrkekood 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Kui teile kuvatakse tõrge aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluma skeeme ADAL registri.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526983"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="df9d4-103">Kaugtöölaua teenuste aktiveerimise Office 2013 ilmnes tõrge</span><span class="sxs-lookup"><span data-stu-id="df9d4-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="df9d4-104">Kui teile kuvatakse tõrge aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluma skeeme ADAL registri.</span><span class="sxs-lookup"><span data-stu-id="df9d4-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="df9d4-105">**Registrivõtme**</span><span class="sxs-lookup"><span data-stu-id="df9d4-105">**Registry key**</span></span>|<span data-ttu-id="df9d4-106">**Tüüp**</span><span class="sxs-lookup"><span data-stu-id="df9d4-106">**Type**</span></span>|<span data-ttu-id="df9d4-107">**Väärtus**</span><span class="sxs-lookup"><span data-stu-id="df9d4-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="df9d4-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="df9d4-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="df9d4-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="df9d4-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="df9d4-110">1</span><span class="sxs-lookup"><span data-stu-id="df9d4-110">1</span></span>  <br/> |

<span data-ttu-id="df9d4-111">Lisateabe saamiseks vt [Office 2013 Windowsi seadmete lubade kasutada programmi kaasaegne autentimine](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="df9d4-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="df9d4-112">Office 365 ProPlus ja Office 2016 on lubatud ADAL.</span><span class="sxs-lookup"><span data-stu-id="df9d4-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="df9d4-113">Kaugtöölaua teenused (RDS) nimetati varem Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="df9d4-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  