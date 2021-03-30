---
title: Rakenduse registreerimise kliendi salajase või serdiga seotud probleemid
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404458"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Rakenduse registreerimise kliendi salajase või serdiga seotud probleemid

Kas rakendusklient aegub salaja?

Olenemata sellest, kuidas registreeritud rakendus loodi( kas rakenduste registreerimise portaalis tavapärase registreerimisprotsessi kaudu või kui teenusesubjekt loodi teie rentnikus rakenduse nõusoleku alusel), tuleb enne praeguse rakendusekoodi aegumist luua uus kliendisaladus. Maksimaalne kehtivusaeg on 2 aastat. Meeldetuletusena tuleb salajane väärtus salvestada, kuna see ei ole enam nähtav pärast portaalis rakenduse registreerimiste lehelt lahkumist. Lisateavet leiate teemast [Quickstart: Rakenduse](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) registreerimine Microsofti identiteediplatvormil ja Microsofti [identiteediplatvormi head tavad.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Lisateavet leiate teemast [Azure AD-rakenduse & teenusesubjekti loomine portaalis – Microsofti identiteediplatvorm](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
