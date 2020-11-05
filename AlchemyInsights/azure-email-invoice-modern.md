---
title: Kaasaegne Azure ' i meilikonto arveldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922060"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="350f1-102">Meili arveldamine Azure ' is</span><span class="sxs-lookup"><span data-stu-id="350f1-102">Email invoicing in Azure</span></span>

<span data-ttu-id="350f1-103">Meilisõnumi arve eelistuste värskendamiseks peab teil olema omanik või kaastööd arvelduse profiilis või selle arvelduskontol.</span><span class="sxs-lookup"><span data-stu-id="350f1-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="350f1-104">Kui olete valinud, saavad kõik arvelduse profiilis olevad omaniku, kaastöötaja, lugejate ja arve halduri rolliga kasutajad arve meili teel.</span><span class="sxs-lookup"><span data-stu-id="350f1-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="350f1-105">Logige sisse [Azure ' i portaali](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="350f1-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="350f1-106">Otsige **kulude haldus + arveldus**.</span><span class="sxs-lookup"><span data-stu-id="350f1-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="350f1-107">Valige vasakus servas olevad **arved** ja seejärel valige lehe ülaosast **e-posti arve** .</span><span class="sxs-lookup"><span data-stu-id="350f1-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="350f1-108">Kui teil on mitu arvelduse profiili, valige arveldamise profiil ja seejärel valige käsk **Vali sisse**.</span><span class="sxs-lookup"><span data-stu-id="350f1-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="350f1-109">Valige **Värskenda**.</span><span class="sxs-lookup"><span data-stu-id="350f1-109">Select **Update**.</span></span>
6. <span data-ttu-id="350f1-110">Kui teil on mitu arvelduse profiili, valige arveldamise profiil ja seejärel valige käsk **Vali sisse**.</span><span class="sxs-lookup"><span data-stu-id="350f1-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="350f1-111">Annate teistele juurdepääsu arvete vaatamiseks, allalaadimiseks ja maksmiseks, määrates neile MCA või MPA arvelduse profiili arve halduri rolli.</span><span class="sxs-lookup"><span data-stu-id="350f1-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="350f1-112">Kui olete valinud oma arve meili teel, saavad kasutajad ka meili teel arveid.</span><span class="sxs-lookup"><span data-stu-id="350f1-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="350f1-113">Logige sisse [Azure ' i portaali](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="350f1-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="350f1-114">Otsige **kulude haldus + arveldus**.</span><span class="sxs-lookup"><span data-stu-id="350f1-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="350f1-115">Valige vasakust servast **arvelduse profiilid** .</span><span class="sxs-lookup"><span data-stu-id="350f1-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="350f1-116">Valige loendist arvelduse profiilid arveldamise profiil, mille jaoks soovite määrata arve halduri rolli.</span><span class="sxs-lookup"><span data-stu-id="350f1-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="350f1-117">Valige vasakpoolsest servast käsk **Access Control (iam)** ja seejärel valige lehe ülaservas nupp **Lisa** .</span><span class="sxs-lookup"><span data-stu-id="350f1-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="350f1-118">Valige ripploendis roll väärtus **arve haldur**.</span><span class="sxs-lookup"><span data-stu-id="350f1-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="350f1-119">Sisestage juurdepääsu andmiseks kasutaja meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="350f1-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="350f1-120">Rolli määramiseks valige **Salvesta** .</span><span class="sxs-lookup"><span data-stu-id="350f1-120">Select **Save** to assign the role.</span></span>
