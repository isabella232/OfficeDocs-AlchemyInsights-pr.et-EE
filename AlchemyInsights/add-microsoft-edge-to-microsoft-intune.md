---
title: Microsoft Edge ' i lisamine Microsoft Intune ' i
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194478"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="865b4-102">Microsoft Edge ' i lisamine Microsoft Intune ' i</span><span class="sxs-lookup"><span data-stu-id="865b4-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="865b4-103">Windows 10 jaoks mõeldud Microsoft Edge ' i juurutamise, konfigureerimise, jälgimise ja kaitsmise võimaldamiseks peate selle esmalt lisama Microsoft Intune ' i.</span><span class="sxs-lookup"><span data-stu-id="865b4-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="865b4-104">Intune toetab Microsoft Edge 77 ja uuemate versioonidega.</span><span class="sxs-lookup"><span data-stu-id="865b4-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="865b4-105">Intune tuvastab Microsoft Edge ' i olemasoleva installi.</span><span class="sxs-lookup"><span data-stu-id="865b4-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="865b4-106">Kui Microsoft Edge on installitud kasutaja kontekstis, kirjutatakse süsteemi installimine kasutaja kontekstis üle.</span><span class="sxs-lookup"><span data-stu-id="865b4-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="865b4-107">Kui Microsoft Edge on süsteemi kontekstis installitud, siis esitatakse installi edukus.</span><span class="sxs-lookup"><span data-stu-id="865b4-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="865b4-108">Eelinstallitud Microsoft Edge 77 ja uuemad versioonid, mis on mõeldud kõigi kasutajate kontekstis, kirjutatakse süsteemi konteksti installitud Microsoft Edge ' i kaudu.</span><span class="sxs-lookup"><span data-stu-id="865b4-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="865b4-109">**Eeltingimus**</span><span class="sxs-lookup"><span data-stu-id="865b4-109">**Prerequisite**</span></span>

<span data-ttu-id="865b4-110">Windows 10 versioon 1709 või uuemad versioonid</span><span class="sxs-lookup"><span data-stu-id="865b4-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="865b4-111">**Servale Intune ' i lisamise juhised**</span><span class="sxs-lookup"><span data-stu-id="865b4-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="865b4-112">[Rakenduse konfigureerimine Intune ' is](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="865b4-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="865b4-113">[Rakenduse teabe konfigureerimine](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="865b4-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="865b4-114">[Konfigureerige rakenduse sätted](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="865b4-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="865b4-115">[Valige ulatuse sildid (valikuline)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="865b4-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="865b4-116">[Lisage rakendus](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="865b4-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="865b4-117">Lisateavet leiate teemast [tõrkeotsing](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="865b4-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




