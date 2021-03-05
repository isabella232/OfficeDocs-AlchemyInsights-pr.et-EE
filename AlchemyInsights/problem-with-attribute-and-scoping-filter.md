---
title: Atribuudi ja ulatuse filtri probleem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481364"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="3acba-102">Atribuudi ja ulatuse filtri probleem</span><span class="sxs-lookup"><span data-stu-id="3acba-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="3acba-103">**Vastuolulised UPN-i väärtuste probleem**</span><span class="sxs-lookup"><span data-stu-id="3acba-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="3acba-104">Tööpäev AD kasutaja ettevalmistamine tööpäevaks AD kasutaja ettevalmistamine kuvab tõrketeate **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="3acba-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="3acba-105">Toiming nurjus, sest UPN-i väärtus, mis on ette nähtud lisamise/muutmisega, pole kogu metsa kordumatu.</span><span class="sxs-lookup"><span data-stu-id="3acba-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="3acba-106">Tõrke üksikasjad: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="3acba-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="3acba-107">**UserPrincipalName** väärtus, mille tööpäeva konnektor proovib määrata, kui loote ad User Account on juba olemas Target ad domeenis.</span><span class="sxs-lookup"><span data-stu-id="3acba-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="3acba-108">See tähendab, et kas (1) kasutaja on juba olemas ja vastavad ID-d ei kontrollinud kasutaja või (2) UPN-i generatsiooni reegel genereeris vastuolulise väärtuse.</span><span class="sxs-lookup"><span data-stu-id="3acba-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="3acba-109">Siit leiate Soovitatavad eraldusvõime juhised.</span><span class="sxs-lookup"><span data-stu-id="3acba-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="3acba-110">Kui kasutaja on juba olemas ja vastava ID kontrollimisel ei õnnestunud linkida tööpäevade kontot Active Directory kontoga, siis kontrollige, kas vastaval tööpäeval ja REKLAAMIl on täpne vaste ID-atribuut (tavaliselt **employeeID**).</span><span class="sxs-lookup"><span data-stu-id="3acba-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="3acba-111">Kui neil pole vastet, on vaja määrata andmete probleem.</span><span class="sxs-lookup"><span data-stu-id="3acba-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="3acba-112">Kui EmployeeID tööpäeval on näiteks 001052 ja AD on 1052, siis ei saa kavandatav mootor kahe konto linkida ning proovib luua juba olemasoleva kasutaja.</span><span class="sxs-lookup"><span data-stu-id="3acba-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="3acba-113">Lahendus sel juhul on muuta AD **EmployeeID** väärtust, et kaasata selle 001052.</span><span class="sxs-lookup"><span data-stu-id="3acba-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="3acba-114">Kui UPN-i genereeriv avaldis ei Genereeri kordumatut väärtust, kaaluge funktsiooni de-dubleerimise funktsiooni **SelectUniqueValue** abil iga kord ainulaadse väärtuse genereerimist.</span><span class="sxs-lookup"><span data-stu-id="3acba-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="3acba-115">**Tööpäeval AD kasutaja ettevalmistamine ei sea AD User Account Manageri atribuudi väärtust**</span><span class="sxs-lookup"><span data-stu-id="3acba-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="3acba-116">Tööpäev AD kasutaja ettevalmistamisel ei määra AD kasutajakontodele **halduri** atribuudi väärtust.</span><span class="sxs-lookup"><span data-stu-id="3acba-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="3acba-117">Selle käitumise ilmnemisel on kaks võimalikku stsenaariumi.</span><span class="sxs-lookup"><span data-stu-id="3acba-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="3acba-118">Tööpäevade haldurit ei saa resolvida vastavale AD kasutajakontole, sest haldur pole ulatuses.</span><span class="sxs-lookup"><span data-stu-id="3acba-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="3acba-119">**Mitme ad-domeeni** stsenaariumi korral ei viibi haldur tööpäevas kasutajaga samas domeenis.</span><span class="sxs-lookup"><span data-stu-id="3acba-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="3acba-120">Probleemi lahendamiseks proovige järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="3acba-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="3acba-121">Kui olete määranud filtrite määratlemine, siis kõigepealt kontrollige, kas haldur on rakendusalas ja kas see vastab ulatuse määramise klauslile.</span><span class="sxs-lookup"><span data-stu-id="3acba-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="3acba-122">Kui haldur ei vasta filtri ulatuse filtrile, Muutke filtrit nii, et haldur oleks ka ettevalmistamisel.</span><span class="sxs-lookup"><span data-stu-id="3acba-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="3acba-123">Kui teil on mitu AD domeeni, on konnektoril teadaolevalt piiratud suutmatus lahendada domeenide halduri viiteid.</span><span class="sxs-lookup"><span data-stu-id="3acba-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="3acba-124">Lisateavet tööpäevade automaatseks ettevalmistamiseks konfigureerimise kohta leiate teemast [õpetus: tööpäevade automaatseks](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ettevalmistamiseks konfigureerimine.</span><span class="sxs-lookup"><span data-stu-id="3acba-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













