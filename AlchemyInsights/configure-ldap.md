---
title: LDAP-konfigureerimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885165"
---
# <a name="configure-ldap"></a>LDAP-konfigureerimine

LDAP-i konfigureerimiseks tehke järgmist.

1. Kontrollige oma domeeni tervist [Azure ' i portaalis](https://aka.ms/aadds-health).
1. Veenduge, et saadaolev Azure AD tellimus on saadaval ja Azure AD Domain Services on lubatud.
1. Turvalise LDAP-i lubamiseks nõutav sert peab olema saadud usaldusväärsest avaliku sertimiskeskuse või iseallkirjastatud serdiga.
1. Veenduge, et sert järgib nõutavaid [juhiseid](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Kehtetu sert**
1. Serdi pikendamiseks järgige juhiseid uue serdi loomiseks ja uuesti üleslaadimiseks: LDAP-i [konfigureerimine](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Azure Active Directory Domain Services turvaliste LDAP-teatistega teadaoleva probleemi lahendamiseks lugege teemat [LDAP-teatiste lahendamine](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
