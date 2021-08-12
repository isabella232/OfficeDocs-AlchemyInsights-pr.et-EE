---
title: API-õigused ja nõusolekuprotsess
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
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932057"
---
# <a name="api-permissions-and-consent-process"></a>API-õigused ja nõusolekuprotsess

Selleks et teie rakendus pääseks microsoft Graph andmetele juurde, peab kasutaja või administraator andma sellele nõusolekuprotsessi kaudu õiged õigused. [Microsoft Graph õiguste viidetes](https://docs.microsoft.com/graph/permissions-reference) loetletakse kõigi Microsoft Graph API-dega seotud õigused. Samuti annab see juhiseid õiguste kasutamise kohta.

**Teenusesubjekti häälestamine või värskendamine**

- [Teenuseprintipaali loomine](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – selles artiklis kirjeldatakse, kuidas luua uus servicePrincipal-objekt.
- [Portaalis Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) teenusesubjekti loomine – selles artiklis kirjeldatakse, kuidas luua uus Azure Active Directory (Azure AD) rakendus ja teenusesubjekt, mida saab kasutada rollipõhise juurdepääsu juhtelemendiga.
- [Rakendused & Teenusesubjektid Azure AD-s](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – selles artiklis kirjeldatakse rakenduse registreerimist, rakenduseobjekte ja teenusesubjekte Azure Active Directory- mis need on, kuidas neid kasutatakse ja kuidas need omavahel seotud on.

**Rakenduse registreerimise lisamine või värskendamine ja administraatori nõusoleku andmine**

- [Rakenduse registreerimise loomine](https://docs.microsoft.com/graph/api/application-post-applications) – selles artiklis kirjeldatakse, kuidas luua uus rakendusobjekt.
- [Rakenduse registreerimise värskendamine – API-õigused](https://docs.microsoft.com/graph/api/application-update) – selles artiklis kirjeldatakse, kuidas värskendada rakenduseobjekti atribuute.
- [Administraatori nõusoleku andmine](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – administraatori nõusoleku ja nõusoleku andmiseks üldiselt nõuame, et administraator annab selgesõnaliselt nõusoleku.
- [RBAC (beetaversioon)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – rollihalduse ümbris ühtse rollimääratluste ja rollimäärangute jaoks Microsoft 365 RBAC-teenusepakkujatele, kes toetavad ühte rollimäärangut mitmele subjektile ja mitmele ulatusele. See erineb *ressursitüübist rbacApplication.* Microsoft Intune on näide sellisest RBAC-pakkujast. Intune'i rollimäärangul võib olla subjektide massiiv ja ulatuserühmade massiiv. **See on beetaversioon, mis tähendab, et see on alles arenduses ja seda ei soovitata kasutada tootmises.**
