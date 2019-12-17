---
title: Tõrkeotsing juurdepääs keelatud sõnumid OneDrive for Business saidid
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051601"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="866da-102">Tõrkeotsing juurdepääs keelatud sõnumid OneDrive for Business saidid</span><span class="sxs-lookup"><span data-stu-id="866da-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="866da-103">See probleem ilmneb kõige sagedamini siis, kui kasutaja on kustutatud ja uuesti loodud sama kasutaja turvasubjektinimi (UPN).</span><span class="sxs-lookup"><span data-stu-id="866da-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="866da-104">Uus konto on loodud, kasutades erinevaid PUID (Passporti kordumatu ID) väärtus.</span><span class="sxs-lookup"><span data-stu-id="866da-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="866da-105">Kui kasutaja proovib pääseda saidikogumi või oma OneDrive, kasutaja on vale PUID.</span><span class="sxs-lookup"><span data-stu-id="866da-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="866da-106">Teine stsenaarium hõlmab kataloogi sünkroonimine Active Directory organisatsiooniüksusele (OU).</span><span class="sxs-lookup"><span data-stu-id="866da-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="866da-107">Kui kasutajad on juba SharePointi sisse logitud ja seejärel teisaldatakse teise OU ja uuesti SharePoint, need võivad ilmneda probleem.</span><span class="sxs-lookup"><span data-stu-id="866da-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="866da-108">Selle probleemi lahendamiseks peaksite taastama algse UPN juhiseid artiklis, [taastada kasutaja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="866da-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="866da-109">Kui te ei saa taastada algne kasutaja peaks eemaldama vana kasutaja OneDrive saidi nende juhiste abil, [eemaldage kasutaja kasutajateabe loendist]().</span><span class="sxs-lookup"><span data-stu-id="866da-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="866da-110">Pärast seda, kui see on tehtud, saate kontrollida kasutajal on administraatori õigused OneDrive saidi, järgides juhiseid [lisada admin kasutaja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="866da-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="866da-111">Õigusetasemete kohta lisateabe saamiseks lugege artiklit, [õigusetasemete mõistmine SharePointis](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="866da-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
