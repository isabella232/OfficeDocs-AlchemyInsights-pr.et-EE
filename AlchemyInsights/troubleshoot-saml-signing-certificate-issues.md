---
title: SAML allkirjastamise probleemide tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692910"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>SAML allkirjastamise probleemide tõrkeotsing

SAML allkirjastamise serdi probleemi lahendamiseks tehke järgmised Soovitatavad toimingud.

1. Kui lisate ettevõtte rakenduse, mis toetab SSO-d, loob Azure serdi, mida nimetatakse [SAML allkirjastamise serdiks](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Sellel serdil on tähtaeg 3 aastat. Serdi aegumiskuupäeva muutmiseks lugege teemat [Föderatsiooni serdi aegumiskuupäeva kohandamine ja selle ümberpaigutamine uuele serdile](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure kasutab seda serti rakenduse nõutud SAML märkide allkirjastamiseks ja saadab selle eduka SSO taotlusele. Selle lõpule viimiseks Laadige alla Azure ' i portaalist sert ja saatke see SSO protsessi lõpuleviimiseks rakenduse tarnijale.

Kui toiming on lõpule jõudnud, usaldab rakendus selle serdi ja kõik selle serdi allkirjastatud SAML kinnitatakse rakendusega.

3. Kui see sert aegub, looge uus sert, värskendage see rakenduse tarnijaga ja seejärel aktiveerige see Azure ' i poolel. Lisateavet leiate teemast [varsti aegunud serdi pikendamine](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Kui sert aegub, siis kasutajat ei blokeerita.

4. [Saate lisada](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) meiliaadressid enne praeguse serdi aegumist saadud teatiste jaoks.

> [!NOTE]
> Step-4 on valikuline.

5. Saate muuta rakenduse SAML serdi allkirjastamise suvandeid ja serdi allkirjastamise algoritmi. Lisateavet leiate teemast [serdi allkirjastamise suvandite ja allkirjastamise algoritmi muutmine](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

