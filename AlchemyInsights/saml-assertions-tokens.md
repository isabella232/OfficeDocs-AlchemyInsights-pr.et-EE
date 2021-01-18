---
title: SAML kinnitused (märked)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885218"
---
# <a name="saml-assertions-tokens"></a>SAML kinnitused (märked)

1. Turbe kinnitused märgistuskeel (SAML) märgid on nõuete XML-esitus. Vaikimisi väljastatakse SAML märgid Windowsi teatise Sihtasutus (WCF) välise turvalisuse stsenaariumid. Lisateavet leiate teemast [SAML märgid ja nõuded](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Microsoft Identity Platform eraldab iga autentimise voo töötlemiseks mitu tüüpi turbelubade. [SAML sümboolne nõuete viide](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) kirjeldab vormingut, turbe omadusi ja SAML 2,0 märkide sisu.
3. Kui soovite teada, kuidas konfigureerida turbelubade eluiga, järgige juhiseid [Microsoft Identity Platformi konfigureeritav turbelubade eluajal](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) .
4. Järgige [selles artiklis](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) kirjeldatud juhiseid, et saada teada, kuidas KONFIGUREERIDA AZURE ad SAML turbelubade krüptimist.
5. Rakenduses Azure AD saate häälestada serdi allkirjastamise suvandeid ja serdi allkirjastamise algoritmi. Lisateavet leiate teemast [Täpsemad serdi allkirjastamise suvandid rakenduses Azure Active Directory rakenduse Galerii rakenduste SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
