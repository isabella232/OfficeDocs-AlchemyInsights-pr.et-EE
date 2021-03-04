---
title: SSPR tõrkeotsing
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429722"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="da4c5-102">SSPR tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="da4c5-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="da4c5-103">**Mul on probleeme parooli lähtestamise konfigureerimisega**</span><span class="sxs-lookup"><span data-stu-id="da4c5-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="da4c5-104">Kui olete administraator ja otsite, kuidas lubada iseteeninduskeskuse parooli lähtestamist, lugege artiklit [õpetuse lubamine SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), et konfigureerida oma asutuse parooli lähtestamine.</span><span class="sxs-lookup"><span data-stu-id="da4c5-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="da4c5-105">Võib-olla soovite ka [litsentsimise nõuded](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)üle vaadata.</span><span class="sxs-lookup"><span data-stu-id="da4c5-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="da4c5-106">Teil peab olema vähemalt ühe ettevõttes määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="da4c5-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="da4c5-107">**Ainult pilveteenuse kasutajad** – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid</span><span class="sxs-lookup"><span data-stu-id="da4c5-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="da4c5-108">**Pilv ja/või kohapealsed kasutajad** – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="da4c5-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="da4c5-109">Lisateavet iseteeninduse parooli lähtestamise kohta leiate [meie KKK](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)-s.</span><span class="sxs-lookup"><span data-stu-id="da4c5-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="da4c5-110">**Kuvatakse tõrketeade**</span><span class="sxs-lookup"><span data-stu-id="da4c5-110">**I'm getting an error message**</span></span>

<span data-ttu-id="da4c5-111">Vaadake seda artiklit, et leida levinud tõrked ja nende lahendused: [iseteeninduskeskuse parooli lähtestamise tõrkeotsing](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="da4c5-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="da4c5-112">**Mul on parooli lähtestamise poliitikaga probleeme**</span><span class="sxs-lookup"><span data-stu-id="da4c5-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="da4c5-113">Kui teie parooli lähtestamise poliitika ei käitu ootuspäraselt või kui teil on küsimusi parooli lähtestamise poliitika kohta, vaadake seda artiklit: [Azure Active Directory parooliga seotud reeglid ja piirangud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="da4c5-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="da4c5-114">Parooli lähtestamise poliitika ei rakendu administraatoritele.</span><span class="sxs-lookup"><span data-stu-id="da4c5-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="da4c5-115">Microsoft jõustab iga Azure ' i administraatori rolli jaoks tugeva vaike-kahe värava parooli lähtestamise poliitika.</span><span class="sxs-lookup"><span data-stu-id="da4c5-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="da4c5-116">Veenduge, et katsetate kasutajaga, kes pole administraator.</span><span class="sxs-lookup"><span data-stu-id="da4c5-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="da4c5-117">Lisateavet administraatori lähtestamise poliitika kohta leiate sellest artiklist: [administraatori lähtestamise poliitika erinevused](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="da4c5-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="da4c5-118">**Ma ei soovi, et kasutajad registreeriks parooli lähtestamiseks täiendava turbeteabe**</span><span class="sxs-lookup"><span data-stu-id="da4c5-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="da4c5-119">Saate oma kasutajatele API, PowerShelli või Azure AD Connecti kaudu andmeid (meili ja telefoni atribuudid) eelnevalt asustada.</span><span class="sxs-lookup"><span data-stu-id="da4c5-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="da4c5-120">Lugege, kuidas lugeda:</span><span class="sxs-lookup"><span data-stu-id="da4c5-120">To learn how read:</span></span>

- [<span data-ttu-id="da4c5-121">Parooli lähtestamise juurutamine, mis ei nõua kasutajatelt registreerumist</span><span class="sxs-lookup"><span data-stu-id="da4c5-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="da4c5-122">Milliseid andmeid parooli lähtestamine kasutab?</span><span class="sxs-lookup"><span data-stu-id="da4c5-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="da4c5-123">**Soovin, et kasutajad registreeriks parooli lähtestamiseks täiendava turbeteabe**</span><span class="sxs-lookup"><span data-stu-id="da4c5-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="da4c5-124">Kas teie kasutajad registreerivad ise oma turbeteabe parooli lähtestamiseks, suunates need [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="da4c5-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="da4c5-125">Kui kasutaja (kasutaja või administraator) on andmed asustanud, suunatakse kasutaja [aka.MS/SSPR](https://passwordreset.microsoftonline.com/) , et kasutajad saaksid oma paroole lähtestada.</span><span class="sxs-lookup"><span data-stu-id="da4c5-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="da4c5-126">Kui kasutajatel esineb endiselt probleeme, on need tõenäoliselt **ühendatud** või **parool Hash sünkroonitud** kasutajad.</span><span class="sxs-lookup"><span data-stu-id="da4c5-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="da4c5-127">See tähendab, et tõenäoliselt esineb probleeme parooliga tagasikirjutusega teenusega.</span><span class="sxs-lookup"><span data-stu-id="da4c5-127">This means there is likely a problem with the Password Writeback service.</span></span>