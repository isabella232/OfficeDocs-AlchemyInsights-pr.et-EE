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
# <a name="issue-with-security-groups"></a>Probleem turvalisuse rühmadega

**Kui teile kuvatakse võrgutõrge AADDS104**

Lubamatu võrgu turbe rühma reeglid on Azure Active Directory Domain Services (AD DS) võrgutõrge. Virtual Network Security Group peab lubama juurdepääsu teatud portidele ja protokollidele. Kui need pordid on blokeeritud, ei saa Azure ' i platvorm hallatavat domeeni jälgida ega värskendada. Azure AD ja Azure AD DS-i vahelist sünkroonimist mõjutavad ka. Veenduge, et hoiate vaikimisi avatud pordid, et vältida teenuse katkestust.

Võrgu turvalisuse rühma konfigureerimise probleemide kohta leiate teavet teemast [turberühma lisamine ja kinnitamine](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
