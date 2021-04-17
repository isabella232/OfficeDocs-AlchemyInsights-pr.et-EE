---
title: Rühma loomine
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816344"
---
# <a name="create-a-group"></a><span data-ttu-id="985ae-102">Rühma loomine</span><span class="sxs-lookup"><span data-stu-id="985ae-102">Create a group</span></span>

<span data-ttu-id="985ae-103">Selles teemas kirjeldatakse rühma loomist.</span><span class="sxs-lookup"><span data-stu-id="985ae-103">This topic describes group creation.</span></span>

<span data-ttu-id="985ae-104">**Rühma loomise õigus**</span><span class="sxs-lookup"><span data-stu-id="985ae-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="985ae-105">Veenduge, et teil oleks õigus luua uus rühm.</span><span class="sxs-lookup"><span data-stu-id="985ae-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="985ae-106">Üldadministraatorid saavad keelata rühma loomise Azure'i portaalis või Accessi paanil.</span><span class="sxs-lookup"><span data-stu-id="985ae-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="985ae-107">Võimalik, et vajate uue rühma loomiseks või teile asjakohaste õiguste andmiseks administraatorit.</span><span class="sxs-lookup"><span data-stu-id="985ae-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="985ae-108">**Rühma loomise õiguste haldamine**</span><span class="sxs-lookup"><span data-stu-id="985ae-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="985ae-109">Üldadministraatorid saavad hallata rühma loomise õigusi (turbega seotud põhjustel) või Azure'i portaalis või Accessi paanil loodud Office 365 rühmi, valides jaotises Kõik rühmad Üldine (Sätted) käsu "Kasutajad saavad luua Turberühmi Azure'i portaalides" või "Kasutajad saavad luua Office 365 rühmi Azure'i   >  **portaalides".**</span><span class="sxs-lookup"><span data-stu-id="985ae-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="985ae-110">Kui teil on Azure Active Directory P1 Premiumi litsents, saate rühma loomist piirata ka kasutajate rühma valimiseks.</span><span class="sxs-lookup"><span data-stu-id="985ae-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="985ae-111">**Uute Office 365 rühmaliikmete tervitusteatise keelamine**</span><span class="sxs-lookup"><span data-stu-id="985ae-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="985ae-112">Office 365 rühmadesse lisatud kasutajatele saadetava tervitusteatise saab keelata, määrates **PowerShellis Sätte UnifiedGroupWelcomeMessageEnabled** väärtuseks False.</span><span class="sxs-lookup"><span data-stu-id="985ae-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="985ae-113">Lisateavet selle sätte kohta [leiate siit.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="985ae-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

