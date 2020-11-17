---
title: Rühma loomine
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088689"
---
# <a name="create-a-group"></a><span data-ttu-id="33c2b-102">Rühma loomine</span><span class="sxs-lookup"><span data-stu-id="33c2b-102">Create a group</span></span>

<span data-ttu-id="33c2b-103">Selles teemas kirjeldatakse rühma loomist.</span><span class="sxs-lookup"><span data-stu-id="33c2b-103">This topic describes group creation.</span></span>

<span data-ttu-id="33c2b-104">**Rühma loomise õigus**</span><span class="sxs-lookup"><span data-stu-id="33c2b-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="33c2b-105">Veenduge, et teil on õigus luua uus rühm.</span><span class="sxs-lookup"><span data-stu-id="33c2b-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="33c2b-106">Globaalsed administraatorid saavad rühma loomise keelata Azure ' i portaalis või Accessi paanil.</span><span class="sxs-lookup"><span data-stu-id="33c2b-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="33c2b-107">Teil võib olla vaja administraatorit, et luua uus rühm või anda teile vastavad õigused.</span><span class="sxs-lookup"><span data-stu-id="33c2b-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="33c2b-108">**Rühma loomise õiguse haldamine**</span><span class="sxs-lookup"><span data-stu-id="33c2b-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="33c2b-109">Globaalsed administraatorid saavad hallata Azure ' i portaalis või Accessi paneelis loodud rühma loomise õiguseid (turbega seotud põhjustel) või Office 365 rühmi, valides "kasutajad saavad luua turberühma Azure ' i portaalis" või "kasutajad saavad luua Office 365 rühmi Azure ' i portaalis" **kõigi rühmade**  >  **üldised suvandid (sätted)**.</span><span class="sxs-lookup"><span data-stu-id="33c2b-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="33c2b-110">Kui teil on Azure Active Directory P1 Premiumi litsents, saate rühma loomist piirata ka kasutajate rühma valimiseks.</span><span class="sxs-lookup"><span data-stu-id="33c2b-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="33c2b-111">**Uute Office 365 rühma liikmete jaoks tervitusprogrammi teatise keelamine**</span><span class="sxs-lookup"><span data-stu-id="33c2b-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="33c2b-112">Office 365 rühmadesse lisatud kasutajatele, kes on lisatud Office rühmadesse, saab keelata, kui säte **UnifiedGroupWelcomeMessageEnabled** on PowerShellis FALSE.</span><span class="sxs-lookup"><span data-stu-id="33c2b-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="33c2b-113">[Siit](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)saate teada, kuidas see säte käib.</span><span class="sxs-lookup"><span data-stu-id="33c2b-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

