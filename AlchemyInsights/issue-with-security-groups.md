---
title: Probleem turvalisuse rühmadega
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177421"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="f31ed-102">Probleem turvalisuse rühmadega</span><span class="sxs-lookup"><span data-stu-id="f31ed-102">Issue with security groups</span></span>

<span data-ttu-id="f31ed-103">**Kui teile kuvatakse võrgutõrge AADDS104**</span><span class="sxs-lookup"><span data-stu-id="f31ed-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="f31ed-104">Lubamatu võrgu turbe rühma reeglid on Azure Active Directory Domain Services (AD DS) võrgutõrge.</span><span class="sxs-lookup"><span data-stu-id="f31ed-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="f31ed-105">Virtual Network Security Group peab lubama juurdepääsu teatud portidele ja protokollidele.</span><span class="sxs-lookup"><span data-stu-id="f31ed-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="f31ed-106">Kui need pordid on blokeeritud, ei saa Azure ' i platvorm hallatavat domeeni jälgida ega värskendada.</span><span class="sxs-lookup"><span data-stu-id="f31ed-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="f31ed-107">Azure AD ja Azure AD DS-i vahelist sünkroonimist mõjutavad ka.</span><span class="sxs-lookup"><span data-stu-id="f31ed-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="f31ed-108">Veenduge, et hoiate vaikimisi avatud pordid, et vältida teenuse katkestust.</span><span class="sxs-lookup"><span data-stu-id="f31ed-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="f31ed-109">Võrgu turvalisuse rühma konfigureerimise probleemide kohta leiate teavet teemast [turberühma lisamine ja kinnitamine](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="f31ed-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
