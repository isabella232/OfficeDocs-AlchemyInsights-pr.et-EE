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
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951489"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Rakenduse registreerimise kliendi salajase või serdiga seotud probleemid

Kas rakendusklient aegub salaja?

Olenemata sellest, kuidas registreeritud rakendus loodi( kas rakenduste registreerimise portaalis tavapärase registreerimisprotsessi kaudu või kui teenusesubjekt loodi teie rentnikus rakenduse nõusoleku alusel), tuleb enne praeguse rakendusekoodi aegumist luua uus kliendisaladus. Maksimaalne kehtivusaeg on 2 aastat. Meeldetuletusena tuleb salajane väärtus salvestada, kuna see ei ole enam nähtav pärast portaalis rakenduse registreerimiste lehelt lahkumist. Lisateavet leiate teemast [Quickstart: Register an app in the Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and Best practices for the [Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Lisateavet leiate teemast [Azure AD-rakenduse & teenusesubjekti loomine portaalis – Microsofti identimisplatvorm](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
