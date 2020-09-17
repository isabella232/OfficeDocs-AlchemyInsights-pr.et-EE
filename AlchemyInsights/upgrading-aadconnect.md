---
title: 932 versioonitäienduse Aadconnecti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806035"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="9415f-102">Azure AD Connecti värskendamine</span><span class="sxs-lookup"><span data-stu-id="9415f-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="9415f-103">Vaikimisi on Azure AD Connecti jaoks lubatud automaatne täiendamine, mis aitab tagada, et kasutate uusimat versiooni.</span><span class="sxs-lookup"><span data-stu-id="9415f-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="9415f-104">Automaatse ülemineku sätete kinnitamiseks kasutage Azure AD PowerShelli cmdlet **-käsku Get-ADSyncAutoUpgrade** .</span><span class="sxs-lookup"><span data-stu-id="9415f-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="9415f-105">Cmdlet-käsk tagastab ühe järgmistest väärtustest.</span><span class="sxs-lookup"><span data-stu-id="9415f-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="9415f-106">**Lubatud**: automaatne uuendamine on lubatud.</span><span class="sxs-lookup"><span data-stu-id="9415f-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="9415f-107">**Keelatud**: automaatne uuendamine on keelatud.</span><span class="sxs-lookup"><span data-stu-id="9415f-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="9415f-108">**Peatatud**: süsteem ei vasta enam automaatsete versioonitäienduste saamise tingimustele.</span><span class="sxs-lookup"><span data-stu-id="9415f-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="9415f-109">Seda väärtust ei saa konfigureerida; See on määratud süsteemis.</span><span class="sxs-lookup"><span data-stu-id="9415f-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="9415f-110">Lisateavet leiate teemast [Automaatne täiendus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="9415f-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="9415f-111">Azure AD Connecti uusima versiooni allalaadimiseks avage [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="9415f-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
