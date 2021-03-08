---
title: Parooli logid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525136"
---
# <a name="password-logs"></a><span data-ttu-id="904ea-102">Parooli logid</span><span class="sxs-lookup"><span data-stu-id="904ea-102">Password logs</span></span>

<span data-ttu-id="904ea-103">**Mul on probleeme parooli lähtestamise auditilogi logidele juurdepääsuga**</span><span class="sxs-lookup"><span data-stu-id="904ea-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="904ea-104">Parooli lähtestamise auditi logidele juurdepääsuga seotud probleemide tõrkeotsingu sooritamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="904ea-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="904ea-105">Veenduge, et teil on õigus vaadata auditi logisid.</span><span class="sxs-lookup"><span data-stu-id="904ea-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="904ea-106">Lubatud on ainult järgmised rollid.</span><span class="sxs-lookup"><span data-stu-id="904ea-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="904ea-107">Globaalne administraator</span><span class="sxs-lookup"><span data-stu-id="904ea-107">Global administrator</span></span>
 - <span data-ttu-id="904ea-108">Security Administrator</span><span class="sxs-lookup"><span data-stu-id="904ea-108">Security administrator</span></span>
 - <span data-ttu-id="904ea-109">Security Reader</span><span class="sxs-lookup"><span data-stu-id="904ea-109">Security reader</span></span>

<span data-ttu-id="904ea-110">**Soovin näha kõiki parooli lähtestamise auditeid alates hetkest, kui ma algselt juurutasin**</span><span class="sxs-lookup"><span data-stu-id="904ea-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="904ea-111">Kuni 120 000 parooli lähtestamise/registreerimise sündmusi talletatakse viimase 30 päeva aruannetes.</span><span class="sxs-lookup"><span data-stu-id="904ea-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="904ea-112">See piirmäär rakendub CSV-i allalaadimisel UI-le.</span><span class="sxs-lookup"><span data-stu-id="904ea-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="904ea-113">1 000 000 sündmused on saadaval PowerShelli kaudu.</span><span class="sxs-lookup"><span data-stu-id="904ea-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="904ea-114">Lisateavet leiate järgmistest linkidest.</span><span class="sxs-lookup"><span data-stu-id="904ea-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="904ea-115">Iseteeninduskeskuse parooli lähtestamise sündmused Azure AD aruannetes ja sündmuste API-s</span><span class="sxs-lookup"><span data-stu-id="904ea-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="904ea-116">Parooli lähtestamise registreerimise sündmuste Kiire allalaadimine PowerShelli abil</span><span class="sxs-lookup"><span data-stu-id="904ea-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="904ea-117">**Soovin saada lisateavet salasõna lähtestamise aruandluse võimaluste kohta**</span><span class="sxs-lookup"><span data-stu-id="904ea-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="904ea-118">Kontrollige, kes registreerub või lähtestab paroolid Azure AD Password reset auditiga Azure ' i portaalis jaotises **kasutajad ja rühmad**.</span><span class="sxs-lookup"><span data-stu-id="904ea-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="904ea-119">Lisateavet leiate järgmistest linkidest.</span><span class="sxs-lookup"><span data-stu-id="904ea-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="904ea-120">Parooli lähtestamise aruannete ülevaade</span><span class="sxs-lookup"><span data-stu-id="904ea-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="904ea-121">Kuidas vaadata Azure ' i portaalis parooli lähtestamise aruandeid?</span><span class="sxs-lookup"><span data-stu-id="904ea-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="904ea-122">Iseteeninduskeskuse parooli lähtestamise sündmused Azure AD aruannetes ja sündmuste API-s</span><span class="sxs-lookup"><span data-stu-id="904ea-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="904ea-123">Parooli lähtestamise registreerimise sündmuste Kiire allalaadimine PowerShelli abil</span><span class="sxs-lookup"><span data-stu-id="904ea-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


