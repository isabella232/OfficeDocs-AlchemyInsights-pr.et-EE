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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707950"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="93b95-102">SharePointi/OneDrive ' i administreerimiskeskuses keelatud sõnumite juurdepääsu tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="93b95-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="93b95-103">Kui saate SharePointi/OneDrive ' i administreerimiskeskuse sirvimisel juurdepääsu keelamise teate, veenduge, et [määrate kasutajale litsentsi](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="93b95-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="93b95-104">Kui kasutajal on litsents, peate veenduma, et neile määratakse administraatori keskustele juurdepääsuks [administraatori roll](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) .</span><span class="sxs-lookup"><span data-stu-id="93b95-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="93b95-105">See probleem võib ilmneda ka siis, kui kasutaja kustutatakse ja luuakse uuesti sama kasutaja põhinimega (UPN).</span><span class="sxs-lookup"><span data-stu-id="93b95-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="93b95-106">Uue konto loomisel kasutatakse mõnda muud PUID (passi kordumatu ID).</span><span class="sxs-lookup"><span data-stu-id="93b95-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="93b95-107">Kui kasutaja proovib juurde pääseda saidikogumile või nende OneDrive ' i, on kasutajal vale PUID.</span><span class="sxs-lookup"><span data-stu-id="93b95-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="93b95-108">Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksuse (OU) abil.</span><span class="sxs-lookup"><span data-stu-id="93b95-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="93b95-109">Kui kasutajad on juba SharePointi sisse loginud ja seejärel teisaldatakse need teise OU ja sünkroonitakse SharePointiga, võivad nad seda probleemi kogeda.</span><span class="sxs-lookup"><span data-stu-id="93b95-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="93b95-110">Selle probleemi lahendamiseks peaksite taastama algse UPN-i artikli juhistega, [taastama kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="93b95-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="93b95-111">Märkus: kui OneDrive ' i või SharePointi halduskeskus pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib tegemist olla ajutise teenuse probleemiga.</span><span class="sxs-lookup"><span data-stu-id="93b95-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="93b95-112">[Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="93b95-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


