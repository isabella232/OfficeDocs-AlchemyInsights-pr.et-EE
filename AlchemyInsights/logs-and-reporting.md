---
title: Logid ja aruandlus
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035912"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="e097f-102">Logid ja aruandlus</span><span class="sxs-lookup"><span data-stu-id="e097f-102">Logs and Reporting</span></span>

<span data-ttu-id="e097f-103">[Azure Active Directory aruandluse KKK](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) vastused korduma kippuvatele küsimustele Azure Active Directory (Azure AD) aruandluse kohta.</span><span class="sxs-lookup"><span data-stu-id="e097f-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="e097f-104">Lisateavet leiate teemast [Azure Active Directory aruandlus](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="e097f-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="e097f-105">**Auditiga seotud probleemide lahendamine**</span><span class="sxs-lookup"><span data-stu-id="e097f-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="e097f-106">Kui teil on probleeme audititega ja puuduv tegevus on selles [loendis](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), palume teil esitada pilet.</span><span class="sxs-lookup"><span data-stu-id="e097f-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="e097f-107">Kui teil on rentniku audititega seotud probleeme, siis palume teil esitada pilet.</span><span class="sxs-lookup"><span data-stu-id="e097f-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="e097f-108">Kui teie auditid pole Azure ' i portaalis kohe nähtaval, vaadake meie [latentsuse teavet](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) ja kui viivitus ületab dokumenteeritud latentsuse, saate selle kohta lisateavet.</span><span class="sxs-lookup"><span data-stu-id="e097f-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="e097f-109">Azure AD Activity logide säilitamine</span><span class="sxs-lookup"><span data-stu-id="e097f-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="e097f-110">Kui te ei näe valitud kuupäevavahemiku auditit, saate alla laadida kuni 250K ridu (sorditud uusimate) sisselogimisest Azure ' i portaalis.</span><span class="sxs-lookup"><span data-stu-id="e097f-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="e097f-111">Lisateavet leiate teemast [auditi toimingute allalaadimine](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="e097f-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="e097f-112">**Sisselogimistega seotud probleemide tõrkeotsing**</span><span class="sxs-lookup"><span data-stu-id="e097f-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="e097f-113">Kui teil on rentniku jaoks Azure AD Premium (P1 või P2) litsents, saate vaadata ainult viimase 30 päeva andmeid.</span><span class="sxs-lookup"><span data-stu-id="e097f-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="e097f-114">Sisselogimised on saadaval ainult Azure AD Premiumi rentnike jaoks.</span><span class="sxs-lookup"><span data-stu-id="e097f-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="e097f-115">See pole saadaval tasuta või põhilise litsentsiga rentnike jaoks.</span><span class="sxs-lookup"><span data-stu-id="e097f-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="e097f-116">Kui teie Rentnik on Premium P1 litsents ja te ei näe sisselogimisi, vaadake meie [latentsuse teavet ja esitage](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) pilet, kui viivitus ületab dokumenteeritud latentsuse.</span><span class="sxs-lookup"><span data-stu-id="e097f-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="e097f-117">Kui te ei näe valitud kuupäevavahemiku jaoks kõiki lisandmooduleid, võtke arvesse, et saate alla laadida kuni 250K ridu (sorditud) Azure ' i portaalist sisselogimisest.</span><span class="sxs-lookup"><span data-stu-id="e097f-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="e097f-118">Lisateavet leiate teemast [sisselogimise tegevuste allalaadimine](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="e097f-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="e097f-119">**Turvalisuse aruannete tõrkeotsing (ohus olevad kasutajad, riskantne sisselogimine)**</span><span class="sxs-lookup"><span data-stu-id="e097f-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="e097f-120">Riskide turvalisuse aruannete lipuga märgitud kasutajad</span><span class="sxs-lookup"><span data-stu-id="e097f-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="e097f-121">Riskantne sisselogimise aruanded Azure Active Directory portaalis</span><span class="sxs-lookup"><span data-stu-id="e097f-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="e097f-122">Azure Active Directory riskitegurid</span><span class="sxs-lookup"><span data-stu-id="e097f-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
