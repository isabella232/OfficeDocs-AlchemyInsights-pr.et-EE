---
title: 932 täiendamine AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389667"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="e205f-102">Ühendage uuendada Azure AD</span><span class="sxs-lookup"><span data-stu-id="e205f-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="e205f-103">Vaikimisi on lubatud automaatne uuendus Azure AD ühenduse, mis võimaldab kiirendada teie arvutis Viimane versioon.</span><span class="sxs-lookup"><span data-stu-id="e205f-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="e205f-104">Kontrollige automaatse uuendamise sätteid, kasutada Azure AD PowerShelli cmdleti **Get-ADSyncAutoUpgrade** .</span><span class="sxs-lookup"><span data-stu-id="e205f-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="e205f-105">Cmdleti naaseb üks järgmistest väärtustest:</span><span class="sxs-lookup"><span data-stu-id="e205f-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="e205f-106">**Enabled**: automaatne uuendus on lubatud.</span><span class="sxs-lookup"><span data-stu-id="e205f-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="e205f-107">**Keelatud**: automaatne uuendus on keelatud.</span><span class="sxs-lookup"><span data-stu-id="e205f-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="e205f-108">**Suspended**: süsteem ei ole enam saada automaatsed versiooniuuendused.</span><span class="sxs-lookup"><span data-stu-id="e205f-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="e205f-109">Te ei saa konfigureerida see; See on süsteemi poolt seatud.</span><span class="sxs-lookup"><span data-stu-id="e205f-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="e205f-110">Lisateabe saamiseks vaadake [Automaatne uuendus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="e205f-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="e205f-111">Uusim versioon Azure AD ühenduse, minge [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="e205f-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
