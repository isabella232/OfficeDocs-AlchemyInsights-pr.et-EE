---
title: 932 täiendamine AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766489"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="840c8-102">Azure AD ühenduse täiendamine</span><span class="sxs-lookup"><span data-stu-id="840c8-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="840c8-103">Vaikimisi on automaatne täiendamine lubatud Azure AD ühenduse jaoks, mis aitab tagada uusima versiooni käitamise.</span><span class="sxs-lookup"><span data-stu-id="840c8-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="840c8-104">Kontrollige automaatse versiooniuuenduse installimise sätted, kasutage Azure AD PowerShelli cmdlet **-käsu Get-ADSyncAutoUpgrade** .</span><span class="sxs-lookup"><span data-stu-id="840c8-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="840c8-105">Cmdlet-käsk tagastab ühe järgmistest väärtustest:</span><span class="sxs-lookup"><span data-stu-id="840c8-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="840c8-106">**Lubatud**: automaatne täiendamine on lubatud.</span><span class="sxs-lookup"><span data-stu-id="840c8-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="840c8-107">**Keelatud**: automaatne täiendamine on keelatud.</span><span class="sxs-lookup"><span data-stu-id="840c8-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="840c8-108">**Peatatud**: süsteem ei vasta enam automaatvärskendusteenuse saamise tingimustele.</span><span class="sxs-lookup"><span data-stu-id="840c8-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="840c8-109">Seda väärtust ei saa konfigureerida; See on süsteemi poolt määratud.</span><span class="sxs-lookup"><span data-stu-id="840c8-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="840c8-110">Lisateabe saamiseks vaadake [automaatset täiendamist](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="840c8-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="840c8-111">Azure AD ühenduse uusima versiooni allalaadimiseks [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="840c8-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
