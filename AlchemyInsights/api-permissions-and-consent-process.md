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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404503"
---
# <a name="api-permissions-and-consent-process"></a>API-õigused ja nõusolekuprotsess

Selleks et teie rakendus pääseks Microsoft Graphis andmetele juurde, peab kasutaja või administraator andma sellele nõusolekuprotsessi kaudu õiged õigused. [Microsoft Graphi õiguste viidetes](https://docs.microsoft.com/graph/permissions-reference) loetletakse kõigi Microsoft Graphi API-de põhikomplektiga seotud õigused. Samuti annab see juhiseid õiguste kasutamise kohta.

**Teenusesubjekti häälestamine või värskendamine**

- [Teenuseprintipaali loomine](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – selles artiklis kirjeldatakse, kuidas luua uus servicePrincipal-objekt.
- [Azure AD-&](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) teenusesubjekti loomine portaalis – selles artiklis kirjeldatakse, kuidas luua uus Azure Active Directory (Azure AD) rakendus ja teenusesubjekt, mida saab kasutada rollipõhise juurdepääsu juhtelemendiga.
- [Rakendused & Teenusesubjektid Azure AD-s](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) . Selles artiklis kirjeldatakse Rakenduse registreerimist, rakenduseobjekte ja teenusesubjekte Azure Active Directorys: mis need on, kuidas neid kasutatakse ja kuidas need on omavahel seotud.

**Rakenduse registreerimise lisamine või värskendamine ja administraatori nõusoleku andmine**

- [Rakenduse registreerimise loomine](https://docs.microsoft.com/graph/api/application-post-applications) – selles artiklis kirjeldatakse, kuidas luua uus rakendusobjekt.
- [Rakenduse registreerimise värskendamine – API-õigused](https://docs.microsoft.com/graph/api/application-update) – selles artiklis kirjeldatakse, kuidas värskendada rakenduseobjekti atribuute.
- [Administraatori nõusoleku andmine](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – administraatori nõusoleku ja nõusoleku andmiseks üldiselt nõuame, et administraator annab selgesõnaliselt nõusoleku.
- [RBAC (beetaversioon)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – rollihalduse ümbris ühtse rollimääratluste ja rolliülesannete jaoks Microsoft 365 RBAC-i pakkujatele, kes toetavad ühte rollimäärangut mitmele subjektile ja mitmele ulatusele. See erineb *ressursitüübist rbacApplication.* Microsoft Intune on näide sellisest RBAC-pakkujast. Intune'i rollimäärangul võib olla subjektide massiiv ja ulatuserühmade massiiv. **See on beetaversioon, mis tähendab, et see on alles arenduses ja seda ei soovitata kasutada tootmises.**
