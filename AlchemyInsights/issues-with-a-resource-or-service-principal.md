---
title: Ressursi- või teenusesubjektiga seotud probleemid
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028072"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Ressursi- või teenusesubjektiga seotud probleemid

1. Kui olete just alustanud, kirjeldavad rakenduse- ja [teenusesubjektiobjektid Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) rakenduse registreerimist, rakenduseobjekte ja teenusesubjekte rakenduses Azure Active Directory: mis need on, kuidas neid kasutatakse ja kuidas need omavahel seotud on. Esitatakse ka mitme rentnikuga näidisstsenaarium, mis illustreerib rakenduse rakendusobjekti ja vastavate teenusesubjektiobjektide vahelist seost.
2. Rakenduste ja teenusesubjektide vahelise seose kohta lisateabe saamiseks lugege rakenduserakendusi ja [teenusesubjektiobjekte](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)Azure Active Directory.
3. [Kuidas teha järgmist. Portaali](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) abil saate luua Azure AD rakenduse ja teenusesubjekti, mis pääseb juurde ressurssidele, näitab, kuidas luua uus Azure Active Directory (Azure AD) rakendus ja teenusesubjekt, mida saab kasutada rollipõhise juurdepääsu juhtelemendiga.
4. Teenuse [põhi-API abil](https://docs.microsoft.com/graph/api/resources/serviceprincipal)saate programmiliselt hallata rakenduste eksemplare ja määrata, mida rakendus saab teie rentnikus teha.
5. [servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.
6. [Ressursitüübi erinevused Azure AD Graph ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) tõstab esile Azure AD Graph ja Microsoft Graph ressursside erinevused. Kuvatakse ressursid, mille nimed on erinevad või mis pole saadaval; Samuti tõstetakse esile Microsoft Graph beetaversioonis saadaolevad ressursid, kuid mitte versioonis v1.0.

**Külaliskasutajatega seotud probleemid**

- [Kiirülevaated: Azure'i](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) portaalis külaliskasutajate lisamine kataloogi näitab, kuidas azure'i portaali kaudu Azure AD kataloogi lisada uus külaliskasutaja, saata kutse ja vaadata, milline külaliskasutaja kutse lunastamise protsess välja näeb.
- [Õpetus. Kasutajavoogude loomine Azure Active Directory B2C-s](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) näitab teile, kuidas Azure'i portaali abil luua soovitatud kasutajavooge. Kui otsite teavet selle kohta, kuidas häälestada oma rakenduses ressursiomaniku parooli identimisteabe (ROPC) voog, lugege teemat Ressursiomaniku parooli identimisteabe voo konfigureerimine Azure AD B2C-s.
