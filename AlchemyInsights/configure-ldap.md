---
title: LDAP-i konfigureerimine
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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090408"
---
# <a name="configure-ldap"></a>LDAP-i konfigureerimine

LDAP konfigureerimiseks tehke järgmist.

1. Kontrollige oma domeeni seisundit [Azure'i portaalis.](https://aka.ms/aadds-health)
1. Veenduge, et kehtiv Azure AD tellimus on saadaval ja Azure AD domeeniteenused on lubatud.
1. Turvalise LDAP-i lubamiseks nõutav sert peab olema pärit usaldusväärsest avalikust sertimiskeskusest või olema ise allkirjastatud sert.
1. Veenduge, et sert järgiks nõutud [juhiseid.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Kehtetu sert**
1. Serdi pikendamiseks järgige uue serdi loomise ja uuestilaadimise juhiseid. [Konfigureerige LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Azure Active directory domain Services secure LDAP-teatistega seotud teadaoleva probleemi lahendamiseks lugege [teemat LDAP-teatiste lahendamine.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
