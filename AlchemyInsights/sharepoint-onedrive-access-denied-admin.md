---
title: Juurdepääs keelatud sõnumite tõrkeotsing
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503523"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="c3f7c-102">Juurdepääs keelatud sõnumite OneDrive/SharePointi administreerimiskeskuses tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="c3f7c-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="c3f7c-103">Kui kuvatakse juurdepääsu keelamise teade, kui proovite SharePointi/OneDrive Admin kus, veenduge, et [määrata kasutaja litsentsi](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="c3f7c-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="c3f7c-104">Kui kasutajal on litsentsi, samuti veenduge on [administraatoriroll](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) millele juurdepääs admin keskused.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="c3f7c-105">See probleem võib ilmneda ka siis, kui kasutaja kustutada ja uuesti luua sama Kasutaja turvasubjektinime (UPN).</span><span class="sxs-lookup"><span data-stu-id="c3f7c-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c3f7c-106">Uue konto loomiseks kasutatakse erinevaid PUID (passi kordumatu ID) väärtus.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c3f7c-107">Kui kasutaja üritab pääseda saidikogumi või oma OneDrive, kasutajal on vale PUID.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c3f7c-108">Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksusele (OU).</span><span class="sxs-lookup"><span data-stu-id="c3f7c-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c3f7c-109">See probleem võib tekkida, kui kasutajad on juba sisse logida SharePoint, siis kolis eri OU ja on SharePointi resynced, nad.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="c3f7c-110">Selle probleemi lahendamiseks peaks taastama algse UPN koos artikli, [taastada kasutaja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)juhiseid.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="c3f7c-111">Märkus: Kui mitmele kasutajale, kellel juurdepääs puudub OneDrive'i või SharePointi Admin keskus, võib teenuse ajutise probleemi.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="c3f7c-112">[Kontrollige teenuste seisundi armatuurlaud](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c3f7c-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


