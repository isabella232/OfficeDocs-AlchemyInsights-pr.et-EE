---
title: Tõrkeotsing külastaja kasutajate probleemidele
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901172"
---
# <a name="troubleshoot-guest-user-issues"></a>Tõrkeotsing külastaja kasutajate probleemidele

1. Juhiseid rakenduse Guest Access haldamise kohta leiate teemast [Guest Accessi haldamine AZURE ad Accessi arvustuste abil](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Lisa Guest kasutajaid oma kataloogi Azure ' i portaalis](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): selle Kiirjuhend abil saate oma Azure ' i reklaami kataloogi lisada Azure ' i portaali kaudu, saata kutse ja vaadata, mis on külaliste kutsete lunastamise protsess välja näeb.
1. [Külaliste lisamine PowerShelli](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)abil: selles kiirjuhend saate kasutada käsku New-AzureADMSInvitation, et lisada oma Azure ' i rentniku jaoks üks külaline.
1. Lisateavet selle kohta, kuidas määrata kasutajatele ja rühmadele Azure Active Directory (Azure AD) rakenduste Enterprise rakendused Azure ' i portaalis või PowerShelli abil, leiate teemast [rakenduse kasutaja ülesande haldamine Azure Active Directorys](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B koostöö töötab enamiku rakendustega, mis integreerivad Azure AD-ga. Sellest [artiklist](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)leiate juhised selle kohta, kuidas konfigureerida mõned populaarsed Saas-rakendused AZURE ad B2B kasutamiseks.
1. Kui ettevõte kasutab Azure Active Directory (Azure AD) B2B koostöö võimalusi, et kutsuda teie Azure ' i REKLAAMIst partneri organisatsioonide kasutajaid, saate nüüd anda neile B2B kasutajatele juurdepääsu kohapealsetele rakendustele. Need kohapealsed rakendused võivad kasutada SAML autentimist või integreeritud Windowsi autentimist (IWA) koos Kerberose piiranud delegatsiooniga (KCD). Lisateavet leiate teemast [B2B kasutajatele AZURE ad juurdepääsu andmine kohapealsetele rakendustele](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Siit saate teada, kuidas [AZURE ad B2B koostöö abil kasutada kohapeal hallatava partneri kontode juurdepääsu pilve ressurssidele](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).