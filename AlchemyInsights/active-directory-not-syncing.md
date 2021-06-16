---
title: Active Directoryt ei sünkroonita
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930971"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="6c72b-102">Active Directoryt ei sünkroonita</span><span class="sxs-lookup"><span data-stu-id="6c72b-102">Active Directory not syncing</span></span>

<span data-ttu-id="6c72b-103">Kui saate sünkroonimistõrkeid (nt "viimatist sünkroonimist pole" või märkate kataloogisünkroonimise olekut Office haldusportaalis, ütleb "Viimati sünkroonitud rohkem kui 3 päeva tagasi", võib olla see, et AADConnectil on valed sätted või sünkroonimiseks pole piisavalt õigusi.</span><span class="sxs-lookup"><span data-stu-id="6c72b-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="6c72b-104">AADConnecti uuesti installimine kiirsätete abil võib probleemi kiiresti lahendada.</span><span class="sxs-lookup"><span data-stu-id="6c72b-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="6c72b-105">[Laadige alla AADConnecti uusim versioon.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="6c72b-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="6c72b-106">[Järgige kiirinstalli juhiseid.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="6c72b-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="6c72b-107">Azure AD Connect peab olema opsüsteemis Windows Server 2012 või uuemas versioonis installitud.</span><span class="sxs-lookup"><span data-stu-id="6c72b-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="6c72b-108">See server peab olema domeeniga ühendatud ja võib olla domeenikontroller või liikmest server.</span><span class="sxs-lookup"><span data-stu-id="6c72b-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="6c72b-109">Azure AD Ühendus eeltingimuste täieliku loendi vaatamiseks vaadake [läbi Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Ühendus.</span><span class="sxs-lookup"><span data-stu-id="6c72b-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="6c72b-110">Lisateavet AADConnecti teenusekontode kohta leiate teemast [Azure AD Ühendus: Kontod ja õigused](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="6c72b-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
