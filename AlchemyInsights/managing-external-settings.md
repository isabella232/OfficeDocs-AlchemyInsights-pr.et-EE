---
title: Väliste sätete haldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294213"
---
# <a name="managing-external-settings"></a><span data-ttu-id="3a07f-102">Väliste sätete haldamine</span><span class="sxs-lookup"><span data-stu-id="3a07f-102">Managing External Settings</span></span>

<span data-ttu-id="3a07f-103">**Teadaanne**</span><span class="sxs-lookup"><span data-stu-id="3a07f-103">**Announcement**</span></span>

- <span data-ttu-id="3a07f-104">[Google ' i WebView väljalogimine alates jaanuarist 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="3a07f-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="3a07f-105">Kontrollige, kas teie rakendused mõjutavad teie rakendusi, järgides Google ' i juhiseid ühilduvuse testimise kohta.</span><span class="sxs-lookup"><span data-stu-id="3a07f-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="3a07f-106">Veenduge, et kasutate oma kasutajatele Google ' i kontoga sisselogimisel süsteemi WebView või süsteemi brauserit.</span><span class="sxs-lookup"><span data-stu-id="3a07f-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="3a07f-107">**Kutse sätete haldamine**</span><span class="sxs-lookup"><span data-stu-id="3a07f-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="3a07f-108">Veenduge, et olete [konfigureerinud väliskoostöö sätted](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) , et lubada vastavatel inimestel kutsed saata.</span><span class="sxs-lookup"><span data-stu-id="3a07f-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="3a07f-109">**Külaliste pääsuõiguste haldamine**</span><span class="sxs-lookup"><span data-stu-id="3a07f-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="3a07f-110">Globaalsed administraatorid saavad hallata Külastajate juurdepääsu kasutusõigusi Azure ' i portaali kaudu, konfigureerides Guest Access permissions lehel välise koostöö sätted.</span><span class="sxs-lookup"><span data-stu-id="3a07f-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="3a07f-111">Lisateavet [selle häälestamise kohta](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3a07f-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="3a07f-112">Kui soovite, et külalised pääseksid juurde sellistele rakendustele nagu meeskonnad või SharePointi, kinnitate, et olete konfigureerinud need rakendused lubama juurdepääsu külastajatele.</span><span class="sxs-lookup"><span data-stu-id="3a07f-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="3a07f-113">Lugege lisateavet [teamsi sätete](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) ja [SharePointi](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)kohta.</span><span class="sxs-lookup"><span data-stu-id="3a07f-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3a07f-114">**Kutsete konfigureerimine.**</span><span class="sxs-lookup"><span data-stu-id="3a07f-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="3a07f-115">Luba B2B väline koostöö ja Halda, kes saavad külalisi kutsuda</span><span class="sxs-lookup"><span data-stu-id="3a07f-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3a07f-116">Kindlatelt organisatsioonidelt kasutajate kutsete lubamine või keelamine</span><span class="sxs-lookup"><span data-stu-id="3a07f-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="3a07f-117">**Lubatud identiteedi pakkujate konfigureerimine.**</span><span class="sxs-lookup"><span data-stu-id="3a07f-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="3a07f-118">Google Federation</span><span class="sxs-lookup"><span data-stu-id="3a07f-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3a07f-119">Otse Föderatsioon</span><span class="sxs-lookup"><span data-stu-id="3a07f-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="3a07f-120">Meili ühekordne pääsukoodi autentimine</span><span class="sxs-lookup"><span data-stu-id="3a07f-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
