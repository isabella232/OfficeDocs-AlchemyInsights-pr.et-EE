---
title: Kasutajate halduse probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035531"
---
# <a name="user-management-issues"></a><span data-ttu-id="457b7-102">Kasutajate halduse probleemid</span><span class="sxs-lookup"><span data-stu-id="457b7-102">User management issues</span></span>

<span data-ttu-id="457b7-103">**Mis juhtub rakendusega praegune määratud kasutajad, kui ma keelan atribuudi "kasutaja määramine on nõutav" (selle atribuudi seadmine pole)?**</span><span class="sxs-lookup"><span data-stu-id="457b7-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="457b7-104">**Nõutud kasutaja ülesande** keelamine ei mõjuta praegu määratud kasutajaid.</span><span class="sxs-lookup"><span data-stu-id="457b7-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="457b7-105">Selle atribuudi keelamine lubab ainult kõigil kasutajatel rakendusele juurde pääseda.</span><span class="sxs-lookup"><span data-stu-id="457b7-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="457b7-106">Kõik loetletud kasutajad ja rakenduse rühmadele määratud kasutajad jäävad endiselt kehtima.</span><span class="sxs-lookup"><span data-stu-id="457b7-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="457b7-107">Rakenduse piiramiseks kindlate kasutajate kogumiga lugege teemat [AZURE ad ' i rakenduse piiramine kasutajate kogumiga – Microsoft Identity Platform | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="457b7-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="457b7-108">Kasutajate ja rühmade määramiseks rakenduses Azure Active Directory (Azure AD) Azure ' i portaalis või PowerShelli abil leiate [lisateavet teemast rakenduse User määrang haldamine rakenduses Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="457b7-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="457b7-109">Rakenduse loomise ja haldamise õiguse delegeerimise kohta leiate teavet teemast [delegaadi rakenduse halduse administraatoriõigused – AZURE ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="457b7-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="457b7-110">**Teatud Enterprise ' i rakenduste peitmine kasutajate hulgast** – järgmiste toimingute abil saate peita kõik Microsoft 365 rakendused **MyApps** paanilt.</span><span class="sxs-lookup"><span data-stu-id="457b7-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="457b7-111">Rakendused on endiselt nähtavad Office 365 portaalis.</span><span class="sxs-lookup"><span data-stu-id="457b7-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="457b7-112">Logige Azure ' i portaali sisse oma kataloogi globaalse administraatorina.</span><span class="sxs-lookup"><span data-stu-id="457b7-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="457b7-113">Valige **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="457b7-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="457b7-114">Valige **Kasutajad**.</span><span class="sxs-lookup"><span data-stu-id="457b7-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="457b7-115">Valige **kasutaja sätted**.</span><span class="sxs-lookup"><span data-stu-id="457b7-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="457b7-116">Klõpsake jaotises **Enterprise Applications (Enterprise Applications**) nuppu **Halda, kuidas lõppkasutajad rakendusi käivitada ja vaadata**</span><span class="sxs-lookup"><span data-stu-id="457b7-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="457b7-117">**Kasutajatele saab office 365 portaalis vaadata ainult office 365 rakendusi**, klõpsake nuppu **Jah**.</span><span class="sxs-lookup"><span data-stu-id="457b7-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="457b7-118">Klõpsake nuppu **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="457b7-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="457b7-119">Lisateavet leiate teemast [ettevõtte rakenduse peitmine kasutaja AZURE ad rakenduses | Microsoft docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="457b7-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="457b7-120">Kui pakute tarkvara teenusena (SaaS) mitmele organisatsioonile, saate oma rakenduse konfigureerida nii, et see aktsepteeriks sisselogimisi mis tahes Azure Active Directory (Azure AD) rentniku kaudu.</span><span class="sxs-lookup"><span data-stu-id="457b7-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="457b7-121">Selle konfiguratsiooni nimi on "mitme rentniku taotluse koostamine".</span><span class="sxs-lookup"><span data-stu-id="457b7-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="457b7-122">Mis tahes Azure AD rentniku kasutajad saavad teie rakendusse sisse logida pärast seda, kui olete oma konto kasutamisega oma kontoga nõustunud.</span><span class="sxs-lookup"><span data-stu-id="457b7-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="457b7-123">Lisateavet leiate teemast [AZURE ad kasutajate sisselogimise rakendused – Microsoft Identity Platform | Microsoft docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="457b7-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="457b7-124">**Kuidas saab lõppkasutaja kasutada rakendust, kui ta on rakendusele määratud?**</span><span class="sxs-lookup"><span data-stu-id="457b7-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="457b7-125">Iga rakenduses Enterprise Application Blade on link lõppkasutajatele juurdepääsemiseks.</span><span class="sxs-lookup"><span data-stu-id="457b7-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="457b7-126">Kasutajad pääsevad rakenduse kaudu **Myapps** portaali kaudu juurde ka lihtsal viisil.</span><span class="sxs-lookup"><span data-stu-id="457b7-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="457b7-127">**Kas soovite teada, milliseid rakendusi ja tüüpi rakendusi kasutajad kasutavad?**</span><span class="sxs-lookup"><span data-stu-id="457b7-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="457b7-128">Saate alla laadida viimase 30 päeva **portal.azure.com > Azure Active directory> Signins> alla laadida aruandeid**.</span><span class="sxs-lookup"><span data-stu-id="457b7-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="457b7-129">Siit saate teada, kuidas [anda rakenduse rentniku jaoks administraatorile nõusolekut](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) ja [konfigureerida, kuidas lõppkasutajad rakendustega nõustuvad](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span><span class="sxs-lookup"><span data-stu-id="457b7-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="457b7-130">Saate teada, [Kuidas nõusolek toimib](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ja [haldab rakenduste nõusolekut](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span><span class="sxs-lookup"><span data-stu-id="457b7-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


