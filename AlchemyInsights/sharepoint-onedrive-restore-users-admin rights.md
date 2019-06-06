---
title: Võimaldada kasutajatele juurdepääs SharePointis või OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736644"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="a6007-102">Võimaldada kasutajatele juurdepääs SharePointis või OneDrive</span><span class="sxs-lookup"><span data-stu-id="a6007-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="a6007-103">See probleem tekib kõige sagedamini kui kasutaja kustutada ja uuesti luua sama Kasutaja turvasubjektinime (UPN).</span><span class="sxs-lookup"><span data-stu-id="a6007-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a6007-104">Uue konto loomiseks kasutatakse erinevaid PUID (passi kordumatu ID) väärtus.</span><span class="sxs-lookup"><span data-stu-id="a6007-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a6007-105">Kui kasutaja üritab pääseda saidikogumi või oma OneDrive, kasutajal on vale PUID.</span><span class="sxs-lookup"><span data-stu-id="a6007-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a6007-106">Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksusele (OU).</span><span class="sxs-lookup"><span data-stu-id="a6007-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a6007-107">See probleem võib tekkida, kui kasutajad on juba sisse logida SharePoint, siis kolis eri OU ja on SharePointi resynced, nad.</span><span class="sxs-lookup"><span data-stu-id="a6007-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a6007-108">Selle probleemi lahendamiseks peaks taastama algse UPN koos artikli,[taastada kasutaja Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide)juhiseid.</span><span class="sxs-lookup"><span data-stu-id="a6007-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="a6007-109">Kui see on tehtud, saate kontrollida kasutaja on admin õigused saidil OneDrive, järgides juhiseid [Lisa admin on kasutaja OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="a6007-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="a6007-110">Õiguste kohta lisateabe saamiseks lugege artiklit, [mõistmise õigusetasemed SharePointi](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a6007-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
