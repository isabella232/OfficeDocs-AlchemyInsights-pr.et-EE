---
title: Probleem ühendava VMs-ga
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885207"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="756ca-102">Probleem ühendava VMs-ga</span><span class="sxs-lookup"><span data-stu-id="756ca-102">Issue joining VMs</span></span>

<span data-ttu-id="756ca-103">VMs-ga liitumisel ilmnevate probleemide lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="756ca-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="756ca-104">Proovige logida sisse **UPN** -vormingus (nt "joeuser@contoso.com") **sAMAccountName** vormingu asemel ("CONTOSO\joeuser").</span><span class="sxs-lookup"><span data-stu-id="756ca-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="756ca-105">Veenduge, et olete lubanud parooli sünkroonimise vastavalt juhistele, mida on kirjeldatud *jaotises Alustamine.*</span><span class="sxs-lookup"><span data-stu-id="756ca-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="756ca-106">Veenduge, et mõjutatud kasutajakonto poleks Azure AD rentniku väline konto.</span><span class="sxs-lookup"><span data-stu-id="756ca-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="756ca-107">Välised kasutajad ei saa hallatavasse domeeni sisse logida, sest Azure AD Domain Services ei ole mandaati selliste kasutajakontode jaoks.</span><span class="sxs-lookup"><span data-stu-id="756ca-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="756ca-108">Kui mõjutatud kasutajakonto on pilveteenuse kasutaja konto, veenduge, et kasutajad on pärast Azure AD Domain Services lubanud parooli muutnud.</span><span class="sxs-lookup"><span data-stu-id="756ca-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="756ca-109">See toiming põhjustab Azure AD Domain Services genereerimiseks nõutavate mandaatide hashes.</span><span class="sxs-lookup"><span data-stu-id="756ca-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="756ca-110">Kui mõjutatud Kasutajakontod sünkroonitakse kohapealsest kataloogist, veenduge, et Azure AD Connecti soovitatav versioon oleks konfigureeritud täieliku sünkroonimise sooritamiseks.</span><span class="sxs-lookup"><span data-stu-id="756ca-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="756ca-111">Kui probleemid püsivad pärast juhise 4 kinnitamist, käivitage sünkroonimisel arvuti kaudu järgmised käsud.</span><span class="sxs-lookup"><span data-stu-id="756ca-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="756ca-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="756ca-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>