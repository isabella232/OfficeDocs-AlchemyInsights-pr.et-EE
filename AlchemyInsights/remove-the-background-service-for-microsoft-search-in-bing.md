---
title: Microsoft Searchi taustapildi eemaldamine Bingis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816126"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="a42b9-102">Microsoft Searchi taustapildi eemaldamine Bingis</span><span class="sxs-lookup"><span data-stu-id="a42b9-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="a42b9-103">Bingis Microsoft Searchi taustapildi eemaldamiseks võite proovida järgmisi õiguskaitsevahendeid.</span><span class="sxs-lookup"><span data-stu-id="a42b9-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="a42b9-104">Algsete otsingumootori sätete taastamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="a42b9-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="a42b9-105">loomine.</span><span class="sxs-lookup"><span data-stu-id="a42b9-105">a.</span></span> <span data-ttu-id="a42b9-106">Aktiveerige **Bingi kasutamine vaike-otsimootori [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)** väljalülitamiseks.</span><span class="sxs-lookup"><span data-stu-id="a42b9-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="a42b9-107">b.</span><span class="sxs-lookup"><span data-stu-id="a42b9-107">b.</span></span> <span data-ttu-id="a42b9-108">[Avage Microsoft 365 halduskeskus](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ja tühjendage säte, mis mõjutab kõiki teie asutuse kasutajaid.</span><span class="sxs-lookup"><span data-stu-id="a42b9-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="a42b9-109">Kui soovite tausta teenuse üksikult seadmelt eemaldada, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="a42b9-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="a42b9-110">loomine.</span><span class="sxs-lookup"><span data-stu-id="a42b9-110">a.</span></span> <span data-ttu-id="a42b9-111">Valige Juhtpaneel **> programmid > programmid ja funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="a42b9-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="a42b9-112">b.</span><span class="sxs-lookup"><span data-stu-id="a42b9-112">b.</span></span> <span data-ttu-id="a42b9-113">Paremklõpsake installitud programmide loendis jaotises **Microsoft Search (Bing** ) ja seejärel klõpsake käsku **desinstalli**.</span><span class="sxs-lookup"><span data-stu-id="a42b9-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="a42b9-114">Oma asutuse mitmest seadmest tausta teenuse eemaldamiseks logige sisse administraatorina ja käivitage skript järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="a42b9-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
