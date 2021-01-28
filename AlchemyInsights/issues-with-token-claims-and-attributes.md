---
title: Turbelubade nõuete ja atribuutidega seotud probleemid
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035888"
---
# <a name="issues-with-token-claims-and-attributes"></a>Turbelubade nõuete ja atribuutidega seotud probleemid

**Turbelubade nõuete värskendamine, konfigureerimine või eemaldamine**

1. Azure Active Directory (Azure AD) abil saate [kohandada nõude tüüpi argumenti](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) , mis on esitatud vastuses, mis kuvatakse pärast rakenduse autoriseerimist.
2. Rakenduse arendajad saavad oma Azure AD rakendustes kasutada fakultatiivseid nõudeid, et määrata, milliseid nõudeid nad soovivad oma rakendusse saadetavate märkidega. Lisateavet leiate teemast [valikuliste nõuete pakkumine rakenduse](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)jaoks.
3. [Rühma taotluste konfigureerimine Azure Active Directory rakenduste jaoks](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Kui kasutate rakenduse sujuvat ühekordset sisselogimist, lugege teemat [SAML lubamine Enterprise ' i rakenduste jaoks välja antud nõuete kohandamine](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Nõuded atribuutide vastendamiseks**

1. Nõuete vastendamise poliitika konfigureerimiseks PowerShelli abil lugege artiklit [rentniku jaoks teatud rakenduse märkidest eralduvate nõuete kohandamine (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Directory skeemi laiendi atribuudid pakuvad võimalust salvestada täiendavaid andmeid Azure Active Directory kasutaja objektid ja muud Directory objektid (nt rühmad, rentniku andmed, teenuse põhiosa). Taotlustele nõuete tekitamiseks saab kasutada ainult kasutajate objektide laienduste atribuute. [Directory skeemi laiendi atribuutide kasutamine nõuetes kirjeldab,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) kuidas kasutada kataloogi skeemi laiendi atribuute, et saata kasutaja andmeid turbelubade taotlustele.

Lisateavet turbelubade kohta leiate järgmistest teemadest.

- [Nõuded Accessi märkidest](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Id_token nõuded](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Nõuded](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , mida võid oodata AZURE ad B2C väljastatud ID märkide ja juurdepääsulubaega
- [SAML loa nõuete viide](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
