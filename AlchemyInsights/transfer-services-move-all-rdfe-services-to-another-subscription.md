---
title: Teenuste edastamine – kõigi RDFE teenuste teisaldamine teise tellimusse
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692041"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="9b16a-102">Teenuste edastamine – kõigi RDFE teenuste teisaldamine teise tellimusse</span><span class="sxs-lookup"><span data-stu-id="9b16a-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="9b16a-103">**Ressursside ümberpaigutamine**</span><span class="sxs-lookup"><span data-stu-id="9b16a-103">**Move resources**</span></span>

<span data-ttu-id="9b16a-104">Azure ' i ressursse saab teisaldada kas mõnele muule Azure ' i tellimusele või ressursirühma samale tellimusele, kasutades Azure ' i portaali, Azure PowerShelli, Azure ' i või REST API-d.</span><span class="sxs-lookup"><span data-stu-id="9b16a-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="9b16a-105">Enne ressursside liikumist vaadake järgmisi teemasid:</span><span class="sxs-lookup"><span data-stu-id="9b16a-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="9b16a-106">Kontroll-loend enne ressursside teisaldamist</span><span class="sxs-lookup"><span data-stu-id="9b16a-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="9b16a-107">Teenused, mida saab teisaldada</span><span class="sxs-lookup"><span data-stu-id="9b16a-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9b16a-108">Liikumise kinnitamine</span><span class="sxs-lookup"><span data-stu-id="9b16a-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="9b16a-109">Teenuste juhendamine</span><span class="sxs-lookup"><span data-stu-id="9b16a-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="9b16a-110">Olemasolevate ressursside teise ressursirühma või tellimusele liikumiseks saate kasutada järgmist.</span><span class="sxs-lookup"><span data-stu-id="9b16a-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="9b16a-111">Azure ' i portaal</span><span class="sxs-lookup"><span data-stu-id="9b16a-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="9b16a-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="9b16a-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="9b16a-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="9b16a-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="9b16a-114">REST API</span><span class="sxs-lookup"><span data-stu-id="9b16a-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="9b16a-115">Õpetus: [Azure ' i ressursside teise ressursirühma või tellimusele minek](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="9b16a-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="9b16a-116">**Tõrkeotsing tõrgete korral Azure Resource Manageri abil**</span><span class="sxs-lookup"><span data-stu-id="9b16a-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="9b16a-117">Lisateavet levinud Azure ' i juurutamise tõrgete kohta leiate allpool olevatest artiklitest ja nende lahendamiseks saada teavet.</span><span class="sxs-lookup"><span data-stu-id="9b16a-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="9b16a-118">Kui te ei leia oma juurutamise tõrke tõrkekoodi, lugege teemat [tõrkekoodi otsimine](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="9b16a-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="9b16a-119">Juurutamise tõrgete tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="9b16a-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="9b16a-120">Azure ' i ressursside uuele ressursirühma või tellimusele teisaldamise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="9b16a-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="9b16a-121">Pange tähele, et kui soovite oma Azure ' i tellimust täiendada (nt minna tasuta tasulisele tellimusele), peate tellimuse muutma.</span><span class="sxs-lookup"><span data-stu-id="9b16a-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="9b16a-122">Tasuta prooviversiooni värskendamiseks lugege artiklit [tasuta prooviversiooni uuendamine või Microsoft Imagine Azure ' i tellimuse maksmine-AS-You-Mine](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="9b16a-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="9b16a-123">Tasuliste kontode vahetamise kohta leiate lisateavet teemast [Azure ' i tasuliste pakettide muutmine teise pakkumise jaoks](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="9b16a-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="9b16a-124">**Azure ' i tellimuse lisamiseks või seostamiseks Azure Active Directory rentniku jaoks tehke järgmist.**</span><span class="sxs-lookup"><span data-stu-id="9b16a-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="9b16a-125">Logige sisse ja valige pakett, mida soovite [Azure ' i portaalis tellimuste lehel](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)kasutada.</span><span class="sxs-lookup"><span data-stu-id="9b16a-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="9b16a-126">Valige **Muuda kataloogi**.</span><span class="sxs-lookup"><span data-stu-id="9b16a-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="9b16a-127">Vaadake üle kõik kuvatud hoiatused ja seejärel valige **Muuda**.</span><span class="sxs-lookup"><span data-stu-id="9b16a-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="9b16a-128">Kataloogi muudetakse tellimuse jaoks ja teile kuvatakse edukas sõnum.</span><span class="sxs-lookup"><span data-stu-id="9b16a-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="9b16a-129">Kasutage *kataloogi* vahetaja, et minna uude kataloogi.</span><span class="sxs-lookup"><span data-stu-id="9b16a-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="9b16a-130">See võib võtta kuni 10 minutit, et kõik kuvataks õigesti.</span><span class="sxs-lookup"><span data-stu-id="9b16a-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="9b16a-131">**Soovitatavad dokumendid**</span><span class="sxs-lookup"><span data-stu-id="9b16a-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="9b16a-132">Azure ' i tellimuse omandiõiguse üleandmine</span><span class="sxs-lookup"><span data-stu-id="9b16a-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="9b16a-133">Ressursside uude ressursirühma või tellimusesse paigutamine</span><span class="sxs-lookup"><span data-stu-id="9b16a-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="9b16a-134">Ressursside haldamine Azure ' i portaali abil</span><span class="sxs-lookup"><span data-stu-id="9b16a-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
