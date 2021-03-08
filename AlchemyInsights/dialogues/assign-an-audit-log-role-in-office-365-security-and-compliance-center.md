---
title: Auditi Logi rolli määramine Office 365 turbe & täitmise keskuses
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524790"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="b530b-102">Auditi Logi rolli määramine Office 365 turbe & täitmise keskuses</span><span class="sxs-lookup"><span data-stu-id="b530b-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="b530b-103">Office 365 auditi logist otsimiseks peab administraator olema määratud Exchange Online ' is, et **vaadata ainult auditilogi** rolli või **auditi logisid** .</span><span class="sxs-lookup"><span data-stu-id="b530b-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="b530b-104">Need rollid määratakse vaikimisi vastavuse haldus-ja organisatsiooni halduse rollide rühmadesse.</span><span class="sxs-lookup"><span data-stu-id="b530b-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="b530b-105">Office 365 ja Microsoft 365 globaalsed administraatorid lisatakse automaatselt organisatsiooni halduse rollirühma liikmetena.</span><span class="sxs-lookup"><span data-stu-id="b530b-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="b530b-106">Kui soovite, et kasutaja saaks otsida privileegide miinimumtasemest, saate luua kohandatud rollirühma Exchange Online ' is, lisada **ainult vaate auditi logid** rolli või **auditi logide** rolli ja seejärel lisada kasutaja uue rollirühma liikmena.</span><span class="sxs-lookup"><span data-stu-id="b530b-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="b530b-107">Lisateavet leiate teemast [rollirühma haldamine Exchange Online ' is](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) ja [Otsingu kontrollimine turbe-& vastavuskontrolli keskuses](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="b530b-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>