---
title: Priviligeeritud identiteedi haldamise roll
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088676"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="da9e1-102">Privilegeeritud identiteedi haldamise (PIM) roll</span><span class="sxs-lookup"><span data-stu-id="da9e1-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="da9e1-103">**Pärast rolli aktiveerimist ei anta lube.**</span><span class="sxs-lookup"><span data-stu-id="da9e1-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="da9e1-104">Kui aktiveerite rolli Azure AD priviligeeritud identiteedi halduses (PIM), ei pruugi aktiveerimine kohe levida kõigile portaalidele, mis nõuavad privilegeeritud rolli.</span><span class="sxs-lookup"><span data-stu-id="da9e1-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="da9e1-105">Mõnikord, isegi kui muudatus on paljundatud, võib vahemällu salvestamine portaalis põhjustada muudatuse kohese jõustumise.</span><span class="sxs-lookup"><span data-stu-id="da9e1-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="da9e1-106">Kui teie aktiveerimine on hilinenud, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="da9e1-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="da9e1-107">Logige Azure ' i portaalist välja ja seejärel logige uuesti sisse.</span><span class="sxs-lookup"><span data-stu-id="da9e1-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="da9e1-108">Kui aktiveerite Azure AD rolli või Azure ' i ressursi rolli, kuvatakse aktiveerimise etapid.</span><span class="sxs-lookup"><span data-stu-id="da9e1-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="da9e1-109">Kui kõik etapid on valmis, kuvatakse link "Logi välja".</span><span class="sxs-lookup"><span data-stu-id="da9e1-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="da9e1-110">Selle lingi kaudu saate välja logida. See lahendab enamiku juhtumite aktiveerimise viivitusi.</span><span class="sxs-lookup"><span data-stu-id="da9e1-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="da9e1-111">PIM. Veenduge, et olete loetletud rolli liikmena.</span><span class="sxs-lookup"><span data-stu-id="da9e1-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="da9e1-112">Kui aktiveerite Exchange ' i administraatori rolli, veenduge, et logite välja ja logite uuesti sisse.</span><span class="sxs-lookup"><span data-stu-id="da9e1-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="da9e1-113">Kui probleem ei lahene, avage kasutajatoe pilet ja tõstke see probleemina esile.</span><span class="sxs-lookup"><span data-stu-id="da9e1-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="da9e1-114">Kui kasutate turbe-ja vastavuskontrolli keskusele juurdepääsuks Exchange ' i administraatori rolli, lugege järgmist juhist.</span><span class="sxs-lookup"><span data-stu-id="da9e1-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="da9e1-115">Kui aktiveerite rolli juurdepääsuks turbele ja nõuetele vastavuse keskusele või kui aktiveerite SharePointi administraatori rolli, kogete mõne minuti jooksul kuni mõne tunni jooksul mõningast aktiveerimise viivitust.</span><span class="sxs-lookup"><span data-stu-id="da9e1-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="da9e1-116">See on teadaolev probleem ning me töötame nende meeskondadega aktiivselt selle probleemi lahendamiseks niipea kui võimalik.</span><span class="sxs-lookup"><span data-stu-id="da9e1-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="da9e1-117">Lisateavet leiate järgmisest teemast.</span><span class="sxs-lookup"><span data-stu-id="da9e1-117">For more information, see:</span></span>

- [<span data-ttu-id="da9e1-118">Azure AD rollide aktiveerimine PIM-s</span><span class="sxs-lookup"><span data-stu-id="da9e1-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="da9e1-119">Azure ' i ressursside rollide aktiveerimine PIM-s</span><span class="sxs-lookup"><span data-stu-id="da9e1-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="da9e1-120">**Õiguseid ei eemaldata pärast rolli desaktiveerimist või rolli aktiveerimise lõppemist**</span><span class="sxs-lookup"><span data-stu-id="da9e1-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="da9e1-121">Kui desaktiveerite rolli Azure AD priviligeeritud identiteedi halduses või kui rolli aktiveerimise periood aegub, võib esineda viivitusi, kus teil on jätkuvalt juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="da9e1-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="da9e1-122">Kui teie desaktiveerimine on hilinenud, järgige järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="da9e1-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="da9e1-123">Kui desaktiveerite Exchange ' i administraatori rolli või rolli aktiveerimise periood aegub, ja märkate, et enne õiguste eemaldamist on oluline viivitamine, avage tugiteenuste pakett ja teavitage oma klienditoe tehnikut, et saaksite Office ' i selle probleemi lahendamiseks kasutada privilegeeritud juurdepääsu haldust (PAM).</span><span class="sxs-lookup"><span data-stu-id="da9e1-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="da9e1-124">Kui aktiveerimise aeg on aegunud, kuid brauseri seanss on endiselt avatud, sulgege brauser.</span><span class="sxs-lookup"><span data-stu-id="da9e1-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="da9e1-125">Kui olete selle seansi sulgenud, saate rolli edasi kasutada.</span><span class="sxs-lookup"><span data-stu-id="da9e1-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="da9e1-126">See on teadaolev probleem ja me otsime võimalikku lahendust iga seansi aktiivseks tühistamiseks, kui aktiveerimine on aegunud.</span><span class="sxs-lookup"><span data-stu-id="da9e1-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="da9e1-127">Kui teie viivitus on erinev kui need kaks stsenaariumit, siis avage kasutajatugi.</span><span class="sxs-lookup"><span data-stu-id="da9e1-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
