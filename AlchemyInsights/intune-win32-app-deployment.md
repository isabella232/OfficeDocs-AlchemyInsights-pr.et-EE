---
title: Rakenduse Intune Win32 juurutamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461794"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="d1d11-102">Rakenduse Intune Win32 juurutamine</span><span class="sxs-lookup"><span data-stu-id="d1d11-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="d1d11-103">Microsoft Intune võimaldab Win32 rakendused, sealhulgas, kuid mitte ainult MSI ja. EXE tuleb juurutada Windows 10 seadmetes.</span><span class="sxs-lookup"><span data-stu-id="d1d11-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="d1d11-104">Kasutatava juurutuse mehhanismi jaoks on vaja Intune Managementi laiendit (IME), et see oleks TARGETi seadmes olemas.</span><span class="sxs-lookup"><span data-stu-id="d1d11-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="d1d11-105">IME installitakse automaatselt, kui see on suunatud PowerShelli skriptile või Win32-rakenduse juurutusele kasutajale/seadmele.</span><span class="sxs-lookup"><span data-stu-id="d1d11-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="d1d11-106">Olemas on ka komplekt eeltingimustest, mis peavad olema täidetud, et juurutada Win32 rakendusi, mis sisaldavad järgmist:</span><span class="sxs-lookup"><span data-stu-id="d1d11-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="d1d11-107">Toetatud platvormid: Windows 10 versioon 1607 või uuem versioon (Enterprise, Pro ja Educationi versioonid).</span><span class="sxs-lookup"><span data-stu-id="d1d11-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="d1d11-108">Toetatud arhitektuur: x86 ja x64.</span><span class="sxs-lookup"><span data-stu-id="d1d11-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="d1d11-109">Seadme haldus: AAD liitunud ja automaatselt registreerunud (sh hübriid-Domeen liidetud ja rühmapoliitika automaatselt registreerunud).</span><span class="sxs-lookup"><span data-stu-id="d1d11-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="d1d11-110">Rakenduse paketi vorming:. [Microsoft Win32 sisu prep tööriist](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)on koostanud **intunewin** -failid.</span><span class="sxs-lookup"><span data-stu-id="d1d11-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="d1d11-111">Piirangud</span><span class="sxs-lookup"><span data-stu-id="d1d11-111">Limitations:</span></span>
    - <span data-ttu-id="d1d11-112">Maksimaalne suurus: 8GB.</span><span class="sxs-lookup"><span data-stu-id="d1d11-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="d1d11-113">Toetuseta arhitektuur: relvad.</span><span class="sxs-lookup"><span data-stu-id="d1d11-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="d1d11-114">Vaadake üle doc "[Lisa, määra ja jälgige Microsoft Intune ' is Win32 rakendust](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)".</span><span class="sxs-lookup"><span data-stu-id="d1d11-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="d1d11-115">Windowsi rakenduste juurutuse tõrkeotsingu üksikasju (sh Win32 rakendusi) saab vaadata järgmistes dokumentides.</span><span class="sxs-lookup"><span data-stu-id="d1d11-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="d1d11-116">Rakenduse installimise probleemide tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="d1d11-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="d1d11-117">Win32 rakenduste tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="d1d11-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)