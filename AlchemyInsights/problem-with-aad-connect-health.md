---
title: Probleem AAD Ühendus Health
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
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923748"
---
# <a name="problem-with-aad-connect-health"></a>Probleem AAD Ühendus Health

- Veenduge, et teil oleks õigus seda toimingut teha. Üldadministraatoritel on vaikimisi juurdepääs. Lisaks saate rollipõhise accessi juhtelemendi [abil delegeerida](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) kaasautorile registreerimisõigused.
- Veenduge, et nõutavad lõpp-punktid on lubatud, mitte tulemüüri tõttu blokeeritud. Lisateavet leiate teemast [Nõuded.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registreerimine võib nurjuda, kuna võrgukiht läbib väljamineva suhtluse SSL-i kontrolli.
- Veenduge, et olete kinnitanud Azure AD Ühendus olekusätted. Vaadake oma säte üle. Sellest [juhendist](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) saate teada, kuidas konfigureerida Azure AD-Ühendus olekuteatisi.
- Lisateavet AAD-Ühendus seisundi sünkroonimise aruande ja selle allalaadimise kohta leiate teemast [Objektitaseme sünkroonimise aruanne.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

AAD Ühendus Seisunditeatised tõrkeotsinguks järgige [AAD Ühendus Seisundiandmete](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) värskuse teatiste tõrkeotsingujuhist ja korduma kippuvaid küsimusi leiate teemast [Levinumad AAD Ühendus Healthi installiga](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)seotud küsimused .
