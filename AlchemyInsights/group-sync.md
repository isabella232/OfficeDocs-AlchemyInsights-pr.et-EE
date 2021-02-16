---
title: Rühma sünkroonimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256719"
---
# <a name="group-sync"></a><span data-ttu-id="7dd37-102">Rühma sünkroonimine</span><span class="sxs-lookup"><span data-stu-id="7dd37-102">Group sync</span></span>

<span data-ttu-id="7dd37-103">Selles artiklis antakse juhised rühma sünkroonimiseks.</span><span class="sxs-lookup"><span data-stu-id="7dd37-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="7dd37-104">Kui üldadministraator või rühma omanik ei saa muuta rühma atribuute või lisada liikmeid või määrata omanikke Azure ' i portaalis, siis veenduge, et rühma asutuse allikas on Azure Active Directory (Azure AD), mille abil saate rühma muuta.</span><span class="sxs-lookup"><span data-stu-id="7dd37-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="7dd37-105">Enne kui proovite Azure AD sünkroonitud rühma kustutada, veenduge, et olete [kustutanud kõik määratud litsentsid](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) tõrgete vältimiseks.</span><span class="sxs-lookup"><span data-stu-id="7dd37-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="7dd37-106">Kasutajate, rühmade ja kontaktide sünkroonimise kohta leiate teavet teemast [AZURE ad Connecti sünkroonimine](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)ja järgige Azure AD Connecti abil Azure AD Connecti abil Azure [ad](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) Connecti abil.</span><span class="sxs-lookup"><span data-stu-id="7dd37-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="7dd37-107">Sünkroonimisel levinud tõrgete tõrkeotsinguks järgige selle juhendi [tõrkeotsingu tõrkeid](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) .</span><span class="sxs-lookup"><span data-stu-id="7dd37-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

