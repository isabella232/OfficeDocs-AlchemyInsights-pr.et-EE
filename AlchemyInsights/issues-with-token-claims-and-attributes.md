---
title: Loataotluste ja atribuutidega seotud probleemid
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012880"
---
# <a name="issues-with-token-claims-and-attributes"></a>Loataotluste ja atribuutidega seotud probleemid

**Loataotluste värskendamine, konfigureerimine või eemaldamine**

1. Funktsiooni Azure Active Directory (Azure AD) abil [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) saate kohandada rollinõude nõudetüüpi vastuses, mille saate pärast rakenduse autoriseerimist.
2. Rakenduse arendajad saavad azure AD-rakendustes kasutada valikulisi nõudeid, et määrata, milliseid nõudeid nad soovivad oma rakendusele saadetavates märkides. Lisateavet leiate teemast [Rakendusele valikuliste nõuete esitamine.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Rühmataotluste konfigureerimine rakenduste jaoks Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Kui kasutate rakenduses sujuvat ühekordset sisselogimist, lugege teemat [SAML-i loas ettevõtterakenduste](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)jaoks välja antud nõuete kohandamine.

**Nõuete atribuudivastendus**

1. PowerShelli abil taotluste vastenduspoliitika konfigureerimise kohta leiate lisateavet teemast Rentnikus konkreetse rakenduse tõendeid saate kohandada [(eelvaade).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Kataloogiskeemi laiendusatribuudid pakuvad võimalust talletada täiendavaid Azure Active Directory kasutajaobjektide ja muude kataloogiobjektide (nt rühmade, rentniku üksikasjade, teenusesubjektide) kohta. Taotluste esitamiseks rakendustele saab kasutada ainult kasutajaobjektide laiendusatribuute. [Kataloogiskeemilaiendi atribuutide kasutamine nõuetes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) kirjeldab, kuidas kasutada kataloogiskeemilaiendi atribuute kasutajaandmete saatmiseks loataotlustes rakendustesse.

Loataotluste kohta leiate lisateavet teemast

- [Juurdepääsulubadega seotud nõuded](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Nõuded id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Azure](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) AD B2C väljastatud ID-märkides ja juurdepääsulubades eeldatud nõuded
- [SAML-i loataotluste viide](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
