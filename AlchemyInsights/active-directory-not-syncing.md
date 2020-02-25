---
title: Active Directory ei sünkroonita
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265157"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="f10ef-102">Active Directory ei sünkroonita</span><span class="sxs-lookup"><span data-stu-id="f10ef-102">Active Directory not syncing</span></span>

<span data-ttu-id="f10ef-103">Kui te saate sünkroonimise tõrked, näiteks "ei ole hiljutine sünkroonimine" või teade kataloogi sünkroonimise olekut Office ' i haldusportaal ütleb: "viimati sünkroonitud rohkem kui 3 päeva tagasi" võib olla, et AADConnect on valed sätted või ebapiisav sünkroonimise sooritamiseks vajalikud õigused.</span><span class="sxs-lookup"><span data-stu-id="f10ef-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="f10ef-104">AADConnect uuesti installimine kiirseadete abil võib probleemi kiiresti lahendada:</span><span class="sxs-lookup"><span data-stu-id="f10ef-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="f10ef-105">[Laadige alla AADConnect uusim versioon](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="f10ef-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="f10ef-106">[Järgige kiire paigaldamise juhiseid](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="f10ef-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="f10ef-107">AADConnect teenusekontode kohta lisateabe saamiseks vaadake [AZURE AD ühenduse: kontod ja õigused](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="f10ef-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
