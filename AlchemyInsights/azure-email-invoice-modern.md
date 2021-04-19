---
title: ModernNe Azure'i meilipõhine arveldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820822"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="8ad47-102">E-posti arveldamine Azure'is</span><span class="sxs-lookup"><span data-stu-id="8ad47-102">Email invoicing in Azure</span></span>

<span data-ttu-id="8ad47-103">Arve e-posti eelistuse värskendamiseks peab teil olema arveldusprofiilis või selle arvelduskontol omanik või kaasautori roll.</span><span class="sxs-lookup"><span data-stu-id="8ad47-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="8ad47-104">Kui olete sisse valinud, saavad kõik kasutajad, kellel on arveldusprofiilis omaniku, kaasautori, lugeja ja arvehalduri rollid, oma arve meiliga.</span><span class="sxs-lookup"><span data-stu-id="8ad47-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="8ad47-105">Logige sisse [Azure'i portaali.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="8ad47-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8ad47-106">Otsige üksust **Kuluhaldus ja arveldus**.</span><span class="sxs-lookup"><span data-stu-id="8ad47-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="8ad47-107">Valige **vasakpoolsest** servast Arved ja seejärel valige **lehe** ülaservast e-posti arve.</span><span class="sxs-lookup"><span data-stu-id="8ad47-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="8ad47-108">Kui teil on mitu arveldusprofiili, valige arveldusprofiil ja seejärel valige **Vali sisse**.</span><span class="sxs-lookup"><span data-stu-id="8ad47-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="8ad47-109">Valige **Värskenda**.</span><span class="sxs-lookup"><span data-stu-id="8ad47-109">Select **Update**.</span></span>
6. <span data-ttu-id="8ad47-110">Kui teil on mitu arveldusprofiili, valige arveldusprofiil ja seejärel valige **Vali sisse**.</span><span class="sxs-lookup"><span data-stu-id="8ad47-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="8ad47-111">Saate anda teistele juurdepääsu arvete vaatamiseks, allalaadimiseks ja maksmiseks, määrates neile MCA või MPA arveldusprofiili arvehalduri rolli.</span><span class="sxs-lookup"><span data-stu-id="8ad47-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="8ad47-112">Kui olete valinud oma arve meiliga saatmise, saavad kasutajad ka arved meiliga.</span><span class="sxs-lookup"><span data-stu-id="8ad47-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="8ad47-113">Logige sisse [Azure'i portaali.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="8ad47-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8ad47-114">Otsige üksust **Kuluhaldus ja arveldus**.</span><span class="sxs-lookup"><span data-stu-id="8ad47-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="8ad47-115">Valige **vasakpoolses servas** Arveldusprofiilid.</span><span class="sxs-lookup"><span data-stu-id="8ad47-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="8ad47-116">Valige arveldusprofiilide loendist arveldusprofiil, mille jaoks soovite määrata arvehalduri rolli.</span><span class="sxs-lookup"><span data-stu-id="8ad47-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="8ad47-117">Valige **vasakpoolsest servast Accessi juhtelement (IAM)** ja seejärel **valige** lehe ülaservast Lisa.</span><span class="sxs-lookup"><span data-stu-id="8ad47-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="8ad47-118">Valige ripploendis Roll väärtus **Arvehaldur**.</span><span class="sxs-lookup"><span data-stu-id="8ad47-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="8ad47-119">Sisestage juurdepääsu andmiseks kasutaja meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="8ad47-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="8ad47-120">Rolli **määramiseks** valige Salvesta.</span><span class="sxs-lookup"><span data-stu-id="8ad47-120">Select **Save** to assign the role.</span></span>
