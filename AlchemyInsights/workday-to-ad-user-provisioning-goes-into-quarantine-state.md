---
title: Tööpäeval AD kasutaja ettevalmistamine läheb karantiini olekusse
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481356"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="f296a-102">Tööpäeval AD kasutaja ettevalmistamine läheb karantiini olekusse</span><span class="sxs-lookup"><span data-stu-id="f296a-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="f296a-103">**Tööpäeval AD kasutaja ettevalmistamine läheb karantiini olekusse ja REKLAAME ei looda kasutajad**</span><span class="sxs-lookup"><span data-stu-id="f296a-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="f296a-104">Tööpäev AD kasutaja ettevalmistamisel on läinud karantiini olekusse ja auditilogi kuvatakse tõrketeade tõrketeade **: OperationsError-SvcErr: ilmnes toimingu tõrge. Kataloogiteenuse jaoks pole ühtegi Superior-viidet konfigureeritud. Kataloogiteenus ei saa seega anda viiteid objektidele väljaspool seda metsa**.</span><span class="sxs-lookup"><span data-stu-id="f296a-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="f296a-105">See tõrge kuvatakse tavaliselt siis, kui Active Directory ümbris OU pole õigesti määratud või kui **parentDistinguishedName** jaoks kasutatakse avaldiste vastendamisega seotud probleeme.</span><span class="sxs-lookup"><span data-stu-id="f296a-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="f296a-106">Märkige ruut **uute kasutajate** jaoks, kui teil on olemas kirjavigu käsitlev parameeter.</span><span class="sxs-lookup"><span data-stu-id="f296a-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="f296a-107">Veenduge, et määratud OU on teie REKLAAMIs juba olemas.</span><span class="sxs-lookup"><span data-stu-id="f296a-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="f296a-108">Kui kasutate atribuutide vastendamisel **parentDistinguishedName** , veenduge, et see hindaks alati teadaolevat konteinerit ad-domeenis.</span><span class="sxs-lookup"><span data-stu-id="f296a-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="f296a-109">Loodud väärtuse kuvamiseks märkige jaotises auditi logid ruut ekspordi sündmus.</span><span class="sxs-lookup"><span data-stu-id="f296a-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="f296a-110">Lisateavet tööpäevade automaatseks ettevalmistamiseks konfigureerimise kohta leiate teemast [õpetus: tööpäevade automaatseks](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)ettevalmistamiseks konfigureerimine.</span><span class="sxs-lookup"><span data-stu-id="f296a-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

