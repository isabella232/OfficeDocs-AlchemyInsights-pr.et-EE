---
title: Probleem ühe kasutajaga
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429711"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="e967e-102">Probleem ühe kasutajaga</span><span class="sxs-lookup"><span data-stu-id="e967e-102">Problem with single user</span></span>

- <span data-ttu-id="e967e-103">Kasutaja ei pruugi olla ette valmistatud, sest teenusel pole olnud võimalust kasutajat veel hinnata.</span><span class="sxs-lookup"><span data-stu-id="e967e-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="e967e-104">Vaadake juhiseid selle kohta, kuidas pikalt ette valmistada, ning ka edenemisriba lehel ettevalmistamine konfigureerimine.</span><span class="sxs-lookup"><span data-stu-id="e967e-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="e967e-105">Kui jaotises täiendavad üksikasjad määratud püsiv olek on enne kasutaja loomise/värskendamise/kustutamise kuupäeva, tähendab see seda, et me pole kasutajat veel hinnanud.</span><span class="sxs-lookup"><span data-stu-id="e967e-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="e967e-106">Selle stsenaariumi korral on parim asi, mida teha on oodata ettevalmistuste lõpuleviimiseks.</span><span class="sxs-lookup"><span data-stu-id="e967e-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="e967e-107">Pange tähele, et meie teenus on teadlik ainult lähteprogrammi kasutaja muudatustest (pilveteenuse HR).</span><span class="sxs-lookup"><span data-stu-id="e967e-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="e967e-108">Azure AD allikas süsteemis peab olema kehtiv muudatus, mis tuvastab muudatuse ja kasutab seda Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="e967e-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="e967e-109">Ettevalmistamise teenus hindas kasutajat ja see ei tohiks olla ette valmistatud.</span><span class="sxs-lookup"><span data-stu-id="e967e-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="e967e-110">Kui olete määranud atribuudi määramisel põhineva filtri, veenduge, et kasutaja vastab teie määratud kriteeriumidele.</span><span class="sxs-lookup"><span data-stu-id="e967e-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="e967e-111">Kui kasutajad on TARGETi süsteemis juba olemas ja kasutaja olek on allikas ja TARGETi vaste, ei võta me täiendavaid toiminguid.</span><span class="sxs-lookup"><span data-stu-id="e967e-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="e967e-112">Teenuse ettevalmistamine proovis kasutajat ette valmistada ja see ebaõnnestus.</span><span class="sxs-lookup"><span data-stu-id="e967e-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="e967e-113">Nende stsenaariumide korral vaadake üle ettevalmistuste logide vahekaart tõrkeotsing ja soovitused.</span><span class="sxs-lookup"><span data-stu-id="e967e-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="e967e-114">Kasutaja nõutav atribuut võib puududa kohapealsest Active Directory või Azure AD-s.</span><span class="sxs-lookup"><span data-stu-id="e967e-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="e967e-115">Näiteks userPrincipalName või sAMAccountName loomise reeglid ei teeni õiget väärtust.</span><span class="sxs-lookup"><span data-stu-id="e967e-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="e967e-116">Vastavat atribuuti (tavaliselt employeeId) ei lahendata kohapealse Active Directory või Azure AD ainulaadse kasutajana.</span><span class="sxs-lookup"><span data-stu-id="e967e-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="e967e-117">Näiteks on kaks kasutajat, kellel on sama employeeId AD ja teenus annab tõrketeate, mis viitab sama Allikatähise kahekordsetele kirjetele.</span><span class="sxs-lookup"><span data-stu-id="e967e-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="e967e-118">Kui soovite vaadata ühe kasutaja ja rühma logisid, lugege teemat [konkreetse kasutajaga seotud probleemi paranduste läbivaatus](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="e967e-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
