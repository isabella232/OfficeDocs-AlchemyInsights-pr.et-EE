---
title: Iseteeninduslik PowerShelli ost
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
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797717"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="bd5e1-102">Iseteeninduslik PowerShelli ost</span><span class="sxs-lookup"><span data-stu-id="bd5e1-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="bd5e1-103">MSCommerce PowerShelli mooduli kasutamiseks peate selle installima Windows 10 seadmesse, kus on TLS 1.2 (nõutav on kohalik administraatoriõigus).</span><span class="sxs-lookup"><span data-stu-id="bd5e1-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="bd5e1-104">Importige ja looge ühendus MSCommerce'i mooduliga.</span><span class="sxs-lookup"><span data-stu-id="bd5e1-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="bd5e1-105">Kui teil palutakse sisse logida, peate kasutama üld- või arveldusadministraatori rolli identimisteavet.</span><span class="sxs-lookup"><span data-stu-id="bd5e1-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="bd5e1-106">Kui teil pole TLS 1.2, võidakse poliitika toomise või värskendamise katsel kuvada järgmine tõrketeade.</span><span class="sxs-lookup"><span data-stu-id="bd5e1-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="bd5e1-107">*ErrorMessage – aluseks olev ühendus suleti: saatmisel ilmnes ootamatu tõrge.*</span><span class="sxs-lookup"><span data-stu-id="bd5e1-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



