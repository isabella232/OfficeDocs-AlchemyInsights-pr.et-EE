---
title: Tõrkekood 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Kui teile kuvatakse tõrge aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluma skeeme ADAL registri.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929084"
---
<span data-ttu-id="627ce-103">Kui teile kuvatakse tõrge aktiveerides Office 2013 kaugtöölaua teenuste (RDS) kasutuselevõttu, kaaluma skeeme ADAL registri.</span><span class="sxs-lookup"><span data-stu-id="627ce-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="627ce-104">**Registrivõtme**</span><span class="sxs-lookup"><span data-stu-id="627ce-104">**Registry key**</span></span>|<span data-ttu-id="627ce-105">\*\*Tippige \*\*</span><span class="sxs-lookup"><span data-stu-id="627ce-105">**Type**</span></span>|<span data-ttu-id="627ce-106">**Väärtus**</span><span class="sxs-lookup"><span data-stu-id="627ce-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="627ce-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="627ce-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="627ce-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="627ce-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="627ce-109">1</span><span class="sxs-lookup"><span data-stu-id="627ce-109">1</span></span>  <br/> |
   
<span data-ttu-id="627ce-110">Lisateabe saamiseks vt [Office 2013 Windowsi seadmete lubade kasutada programmi kaasaegne autentimine](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="627ce-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="627ce-p101">Office 365 ProPlus ja Office 2016 on lubatud ADAL. > kaugtöölaua teenused (RDS) nimetati varem Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="627ce-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

