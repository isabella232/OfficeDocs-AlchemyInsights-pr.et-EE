---
title: Juurdepääs keelatud sõnumite tõrkeotsing
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505375"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="a8966-102">Juurdepääs keelatud sõnumite tõrkeotsing SharePointi/OneDrive ' i administreerimiskeskuses</span><span class="sxs-lookup"><span data-stu-id="a8966-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="a8966-103">Kui teil on juurdepääs keelatud sõnumi sirvimisel SharePointi/OneDrive ' i administreerimiskeskus, veenduge, et [määrata litsentsi kasutajale](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="a8966-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="a8966-104">Kui kasutajal on litsents, peaksite ka veenduma, et neile [määratakse administraatoriroll](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , mis pääseb juurde administreerimiskeskustele.</span><span class="sxs-lookup"><span data-stu-id="a8966-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="a8966-105">See probleem võib ilmneda ka siis, kui kasutaja on kustutatud ja uuesti loodud sama kasutaja turvasubjektinimi (UPN).</span><span class="sxs-lookup"><span data-stu-id="a8966-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a8966-106">Uus konto on loodud, kasutades erinevaid PUID (Passporti kordumatu ID) väärtus.</span><span class="sxs-lookup"><span data-stu-id="a8966-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a8966-107">Kui kasutaja proovib pääseda saidikogumi või oma OneDrive, kasutaja on vale PUID.</span><span class="sxs-lookup"><span data-stu-id="a8966-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a8966-108">Teine stsenaarium hõlmab kataloogi sünkroonimine Active Directory organisatsiooniüksusele (OU).</span><span class="sxs-lookup"><span data-stu-id="a8966-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a8966-109">Kui kasutajad on juba SharePointi sisse logitud ja seejärel teisaldatakse teise OU ja uuesti SharePoint, need võivad ilmneda probleem.</span><span class="sxs-lookup"><span data-stu-id="a8966-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a8966-110">Selle probleemi lahendamiseks peaksite taastama algse UPN juhiseid artiklis, [taastada kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="a8966-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="a8966-111">Märkus: kui OneDrive või SharePointi administreerimiskeskus pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib olla ajutine teenuse probleem.</span><span class="sxs-lookup"><span data-stu-id="a8966-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="a8966-112">[Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a8966-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


