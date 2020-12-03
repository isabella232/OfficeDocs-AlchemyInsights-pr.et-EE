---
title: Rentniku kustutamine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564485"
---
# <a name="delete-tenant"></a><span data-ttu-id="7e459-102">Rentniku kustutamine</span><span class="sxs-lookup"><span data-stu-id="7e459-102">Delete tenant</span></span>

<span data-ttu-id="7e459-103">Azure ' i reklaami kustutamiseks veenduge järgmist.</span><span class="sxs-lookup"><span data-stu-id="7e459-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="7e459-104">Olete kataloogis globaalse administraatorina.</span><span class="sxs-lookup"><span data-stu-id="7e459-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="7e459-105">Te pole sisse logitud kontoga, mille vaikekaustana (nt contoso.onmicrosoft.com) on sisse logitud konto (nt admin@contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="7e459-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="7e459-106">Eemaldage enne kustutamist kõik kataloogis olevad aktiivsed rakendused.</span><span class="sxs-lookup"><span data-stu-id="7e459-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="7e459-107">Aktiivsete rakenduste eemaldamiseks liikuge rakenduse registreerimistele ja eemaldage olemasolevad rakendused.</span><span class="sxs-lookup"><span data-stu-id="7e459-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="7e459-108">Ühtegi Microsoft Online ' i teenust (nt Microsoft Azure ' i, Office 365 või Azure AD Premiumi, mis on seotud kataloogiga) pole ühtegi aktiivset paketti.</span><span class="sxs-lookup"><span data-stu-id="7e459-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="7e459-109">Edastage oma tellimused või kiirendage aktiivsete tellimuste tühistamist Azure ' i toe ja arvelduse kaudu.</span><span class="sxs-lookup"><span data-stu-id="7e459-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="7e459-110">Lugege lisateavet Office ' i 365 ja Azure ' i tellimuste tühistamise kohta.</span><span class="sxs-lookup"><span data-stu-id="7e459-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="7e459-111">Lisateavet rentniku jaoks olemasoleva tellimuse seostamise või lisamise kohta leiate teemast Azure ' i [reklaami rentniku jaoks Azure ' i tellimuse lisamine või lisamine](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="7e459-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="7e459-112">Aktiivset litsentsi pole.</span><span class="sxs-lookup"><span data-stu-id="7e459-112">There are no Active license.</span></span> <span data-ttu-id="7e459-113">Litsentside eemaldamise kohta leiate teavet teemast [tellimuse eemaldamine litsentsi eemaldamiseks](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="7e459-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="7e459-114">Kui proovite Azure ' i reklaami kustutada, pole kataloogis ühtegi teist aktiivset kasutajat peale enda kui globaalse administraatorina.</span><span class="sxs-lookup"><span data-stu-id="7e459-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="7e459-115">Eemaldada kõik muud aktiivsed kasutajad ja kõik rentniku kohandatud domeeninimega seotud sõltuvused tuleb eemaldada ka siis, kui admin@contoso.com on loodud kasutajad.</span><span class="sxs-lookup"><span data-stu-id="7e459-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="7e459-116">Üksikasjalikumad juhised selle kohta, kuidas:</span><span class="sxs-lookup"><span data-stu-id="7e459-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="7e459-117">Kustutage "Azure Active Directory" või "tellimus", lugege teemat [Azure Active Directory kustutamine](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="7e459-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="7e459-118">Rakenduste eemaldamine kataloogist leiate teavet teemast [Rakenduste eemaldamine](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="7e459-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
