---
title: Ressursi või teenuse põhilise probleemid
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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713661"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Ressursi või teenuse põhilise probleemid

1. Kui olete hakanud alles alustama, siis [rakenduse ja teenuse põhiobjektid Azure Active Directory ' s](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) kirjeldab rakenduse registreerimist, rakendusobjektide ja teenuse põhitoiminguid Azure Active Directory: mis need on, kuidas neid kasutatakse ja kuidas nad on üksteisega seotud. Esitatakse ka mitme rentniku näite stsenaarium, kus on kujutatud rakenduse rakendusobjekti ja vastavate teenuse põhiliste objektide vahelist seost.
2. Rakenduste ja teenuste põhiliste seoste kohta leiate lisateavet teemast [Azure Active Directory rakenduste ja teenuste põhiobjektide](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)lugemine.
3. [Kuidas: portaali abil saate luua AZURE ad Applicationi ja teenuse põhiosa, mis võimaldab juurdepääsu ressurssidele](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) , kui soovite luua uue Azure Active Directory (Azure AD) rakenduse ja teenuse põhiosa, mida saab kasutada rolli-põhise Accessi juhtelement.
4. Teenuse põhirakenduse [API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)abil saate programmiliselt hallata rakenduste eksemplare ja määrata, millist rakendust saab rentniku siseselt teha.
5. [servicePrincipal ressursi tüüp](https://docs.microsoft.com/graph/api/resources/serviceprincipal) loetleb kõik servicePrincipal ressursi tüübi atribuudid ja meetodid.
6. [AZURE ad Graphi ja Microsoft Graphi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) erinevuste erinevuste tõttu on Azure AD Graphi ja Microsoft Graphi ressursside erinevused esile tõstetud. Sellel on kujutatud ressursid, millel on erinevad nimed või mida pole saadaval; See tõstab esile ka ressursid, mis on saadaval Microsoft Graphi beetaversioonis, kuid v 1.0 versioonis.

**Probleemid külalise kasutajatega**

- [Kiirjuhend: kasutajate lisamine Azure ' i portaalis](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) olevasse kataloogi näitab teile, kuidas lisada Azure ' i portaali kaudu uut külaliste kasutajat Azure ' i reklaamide kataloogi, saata kutse ja vaadata, mis on külaliste kutsete lunastamise protsess välja näeb.
- [Õpetus: Azure Active DIRECTORY B2C kasutajate voogude loomine](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) näitab teile, kuidas luua Azure ' i portaali abil mõne soovitatava kasutaja vooge. Kui otsite teavet selle kohta, kuidas häälestada rakenduses ressursi omaniku parooli mandaat (ROPC), lugege teemat ressursi omaniku parooli mandaadi voo konfigureerimine Azure AD B2C.
