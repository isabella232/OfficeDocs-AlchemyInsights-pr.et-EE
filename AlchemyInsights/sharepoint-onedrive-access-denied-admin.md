---
title: Accessi keelatud sõnumite tõrkeotsing
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767658"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="7c5ec-102">SharePointi/OneDrive ' i administreerimiskeskuses keelatud sõnumite juurdepääsu tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="7c5ec-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="7c5ec-103">Kui saate SharePointi/OneDrive ' i administreerimiskeskuse sirvimisel juurdepääsu keelamise teate, veenduge, et [määrate kasutajale litsentsi](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="7c5ec-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="7c5ec-104">Kui kasutajal on litsents, peate veenduma, et neile määratakse administraatori keskustele juurdepääsuks [administraatori roll](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) .</span><span class="sxs-lookup"><span data-stu-id="7c5ec-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="7c5ec-105">See probleem võib ilmneda ka siis, kui kasutaja kustutatakse ja luuakse uuesti sama kasutaja põhinimega (UPN).</span><span class="sxs-lookup"><span data-stu-id="7c5ec-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="7c5ec-106">Uue konto loomisel kasutatakse mõnda muud PUID (passi kordumatu ID).</span><span class="sxs-lookup"><span data-stu-id="7c5ec-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="7c5ec-107">Kui kasutaja proovib juurde pääseda saidikogumile või nende OneDrive ' i, on kasutajal vale PUID.</span><span class="sxs-lookup"><span data-stu-id="7c5ec-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="7c5ec-108">Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksuse (OU) abil.</span><span class="sxs-lookup"><span data-stu-id="7c5ec-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="7c5ec-109">Kui kasutajad on juba SharePointi sisse loginud ja seejärel teisaldatakse need teise OU ja sünkroonitakse SharePointiga, võivad nad seda probleemi kogeda.</span><span class="sxs-lookup"><span data-stu-id="7c5ec-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="7c5ec-110">Selle probleemi lahendamiseks peaksite taastama algse UPN-i artikli juhistega, [taastama kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="7c5ec-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="7c5ec-111">Märkus: kui OneDrive ' i või SharePointi halduskeskus pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib tegemist olla ajutise teenuse probleemiga.</span><span class="sxs-lookup"><span data-stu-id="7c5ec-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="7c5ec-112">[Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7c5ec-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


