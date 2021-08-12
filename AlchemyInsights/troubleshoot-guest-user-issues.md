---
title: Külaliskasutaja probleemide tõrkeotsing
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939375"
---
# <a name="troubleshoot-guest-user-issues"></a>Külaliskasutaja probleemide tõrkeotsing

1. Juhised külalisjuurdepääsu haldamise kohta rakendustele leiate teemast [Külalisjuurdepääsu haldamine Azure AD juurdepääsu arvustustega.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Külaliskasutajate](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)lisamine Azure'i portaali kataloogi. Selles kiirsõnumis saate Azure'i portaali kaudu azure AD kataloogi lisada uue külaliskasutaja, saata kutse ja vaadata, milline külaliskasutaja kutse lunastamise protsess välja näeb.
1. [Külalise kasutaja lisamine PowerShelli](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)abil. Selles kiirtoimingus saate kasutada käsku New-AzureADMSInvitation, et lisada azure'i rentnikusse üks külaliskasutaja.
1. Teavet selle kohta, kuidas määrata Azure Active Directory (Azure AD) ettevõtterakendustele kasutajaid ja rühmi kas Azure'i portaalis või PowerShelli abil, leiate teemast Rakenduse kasutaja määramise haldamine [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B-koostöö töötab enamiku Azure AD-ga integreeritud rakendustega. Selles artiklis [on](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)toodud juhised, kuidas konfigureerida mõned populaarsed SaaS-i rakendused Azure AD B2B-ga kasutamiseks.
1. Ettevõttena, mis kasutab Azure Active Directory (Azure AD) B2B koostöövõimalusi, et kutsuda külaliskasutajaid partnerorganisatsioonidest azure AD-sse, saate nüüd anda neile B2B-kasutajatele juurdepääsu kohapealstele rakendustele. Need asutusesisesed rakendused saavad kasutada SAML-i-põhist autentimist või Windows (IWA) koos Kerberose piiratud delegeerimise (KCD) abil. Lisateavet leiate teemast Azure [AD-s B2B-kasutajatele juurdepääsu andmine teie kohapealstele rakendustele.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Siit saate [teada, kuidas anda Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)koostöö abil kohalikult hallatavatele partnerkontodele juurdepääs pilveressurssidele.