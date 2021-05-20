---
title: Kasutaja loomine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569717"
---
# <a name="create-user"></a><span data-ttu-id="fa9a2-102">Kasutaja loomine</span><span class="sxs-lookup"><span data-stu-id="fa9a2-102">Create user</span></span>

<span data-ttu-id="fa9a2-103">**TEADAANNE:**</span><span class="sxs-lookup"><span data-stu-id="fa9a2-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="fa9a2-104">Teenuse WebView sisselogimistoe väljaarvamine [Google'is alates 4. jaanuarist 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="fa9a2-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="fa9a2-105">Kontrollige, kas ühilduvuse testimise juhised [võivad mõjutada](https://go.microsoft.com/fwlink/?linkid=2157323) teie rakendusi.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="fa9a2-106">Veenduge, et kasutate kasutajate sisse logimisel Google'i tarbijakontodega süsteemi veebivaadet või süsteemibrauseri.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="fa9a2-107">Lisateavet leiate teemast Ainult [Chrome'i brauseri abil rakendus(te)sse sisselogimisega seotud probleemid.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="fa9a2-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="fa9a2-108">**Azure AD kataloogis ei saa uut kasutajat luua**</span><span class="sxs-lookup"><span data-stu-id="fa9a2-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="fa9a2-109">Veenduge, et teil oleks õigus luua uus tavakasutaja.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="fa9a2-110">Uue tavakasutaja saab luua ainult Azure Active Directory (AD) üldadministraatori või kasutajaadministraatori rolli.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="fa9a2-111">Kui te pole üheski neist rollidest, paluge administraatoril lisada teid ühte neist rollidest või luua uus kasutajakonto.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="fa9a2-112">Veenduge, et kasutajanimi oleks teie Azure AD-s kinnitatud domeenis.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="fa9a2-113">Kui teil pole Azure AD-s kinnitatud kohandatud domeeninimesid, saate kasutada Azure AD algdomeeni, mille lõpus on \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="fa9a2-114">Veenduge, et kasutajanimi oleks domeenis, mis pole ühendatud teie asutusesisesest AD-st Azure AD-ga.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="fa9a2-115">Pilveteenusesse ei saa kasutajaid lisada domeeninimedega, mis on ühendatud asutusesisesest domeenist.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="fa9a2-116">Veenduge, et ükski teine kasutaja ega kontakt ei oleks juba loonud kasutajanime, mille soovite uuele kasutajale määrata.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="fa9a2-117">Kasutajanimed peavad olema azure AD-s kordumatud.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="fa9a2-118">Azure [AD rollide ja administraatorite kohta leiate](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) lisateavet teemast Azure AD rollid ja administraatorid.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="fa9a2-119">Vaadake [oma](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD domeeninimesid.</span><span class="sxs-lookup"><span data-stu-id="fa9a2-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="fa9a2-120">Vaadake [läbi auditilogid,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) et näha üksikasjalikumat teavet hiljuti loodud või kustutatud kasutaja kohta(nt toimingu sooritanud ja millal).</span><span class="sxs-lookup"><span data-stu-id="fa9a2-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="fa9a2-121">Lisateavet uute kasutajate lisamise kohta leiate teemast [Azure'i portaali abil azure AD-s uue kasutaja loomine.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="fa9a2-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="fa9a2-122">[Azure AD haldusrollid:](/azure/active-directory/active-directory-assign-admin-roles)administraatori rolliõigused Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="fa9a2-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="fa9a2-123">Uue kasutaja [loomiseks saate kasutada ka Azure AD PowerShelli.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="fa9a2-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
