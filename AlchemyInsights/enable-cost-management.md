---
title: Kulude halduse lubamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677219"
---
# <a name="enable-cost-management"></a><span data-ttu-id="55fcf-102">Kulude halduse lubamine</span><span class="sxs-lookup"><span data-stu-id="55fcf-102">Enable cost management</span></span>

<span data-ttu-id="55fcf-103">**Mida tähendab "kulud on teie ettevõtte jaoks keelatud"?**</span><span class="sxs-lookup"><span data-stu-id="55fcf-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="55fcf-104">Ettevõtted, kes kasutavad Enterprise Agreement (EA) või Microsoft Customer Agreement (MCA) kontosid, võivad keelata juurdepääsu kulude teabele ja hinnakujunduse teabele.</span><span class="sxs-lookup"><span data-stu-id="55fcf-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="55fcf-105">Pärast Azure ' i portaali sisselogimist saavad nad arveldamise API-sid kasutada programmiliselt arvete hankimiseks (kui olete valinud) ja kasutuse üksikasjad.</span><span class="sxs-lookup"><span data-stu-id="55fcf-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="55fcf-106">**Kuidas lubada täiendavate kasutajate juurdepääsu arvetele?**</span><span class="sxs-lookup"><span data-stu-id="55fcf-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="55fcf-107">Avage Azure ' i portaalis **tellimuste labad** .</span><span class="sxs-lookup"><span data-stu-id="55fcf-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="55fcf-108">Valige **arved** ja seejärel **juurdepääs arvetele**.</span><span class="sxs-lookup"><span data-stu-id="55fcf-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="55fcf-109">Juurdepääsu sisselülitamine, millele järgneb muudatuste salvestamine, et kasutajad saaksid arved alla laadida tellimuse ulatusega.</span><span class="sxs-lookup"><span data-stu-id="55fcf-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="55fcf-110">Konto administraator saab konfigureerida ka meili teel saadetud arved.</span><span class="sxs-lookup"><span data-stu-id="55fcf-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="55fcf-111">Lisateavet leiate teemast [arve saamine meili teel](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="55fcf-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="55fcf-112">**Kasutajate lisamine arvelduse lugeja rollile**</span><span class="sxs-lookup"><span data-stu-id="55fcf-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="55fcf-113">Avage Azure ' i portaalis **tellimuste labad** .</span><span class="sxs-lookup"><span data-stu-id="55fcf-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="55fcf-114">Valige **Access Control (iam)** ja seejärel klõpsake nuppu **Lisa**.</span><span class="sxs-lookup"><span data-stu-id="55fcf-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="55fcf-115">Valige lehel **rolli valimine** valik **arvelduse lugeja** .</span><span class="sxs-lookup"><span data-stu-id="55fcf-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="55fcf-116">Tippige selle kasutaja meiliaadress, keda soovite kutsuda, ja seejärel klõpsake kutse saatmiseks nuppu **OK** .</span><span class="sxs-lookup"><span data-stu-id="55fcf-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="55fcf-117">Kui soovite logida sisse arvelduse lugejana, järgige juhiseid, mis on toodud teemas Kutsu meilisõnum.</span><span class="sxs-lookup"><span data-stu-id="55fcf-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="55fcf-118">Lisateavet leiate teemast [Arveldusele juurdepääsu andmine](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="55fcf-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="55fcf-119">**Soovitatavad dokumendid**</span><span class="sxs-lookup"><span data-stu-id="55fcf-119">**Recommended documents**</span></span>

- [<span data-ttu-id="55fcf-120">Luba DA ja AO vaateid EA portaali kaudu</span><span class="sxs-lookup"><span data-stu-id="55fcf-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="55fcf-121">Kulude haldusse kaasatud kulud</span><span class="sxs-lookup"><span data-stu-id="55fcf-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="55fcf-122">Toetatud Microsoft Azure ' i pakkumised</span><span class="sxs-lookup"><span data-stu-id="55fcf-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="55fcf-123">Kulude ülevaade kulude analüüsis</span><span class="sxs-lookup"><span data-stu-id="55fcf-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="55fcf-124">Juurdepääsu andmine arvelduse teabele</span><span class="sxs-lookup"><span data-stu-id="55fcf-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="55fcf-125">Microsofti kliendi lepingule juurdepääsu kontrollimine</span><span class="sxs-lookup"><span data-stu-id="55fcf-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






