---
title: SMTP-autentimisega seotud probleemide lahendamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826411"
---
# <a name="solving-smtp-authentication-issues"></a>SMTP-autentimisega seotud probleemide lahendamine

Kui saate SMTP-meili saatmisel ja kliendi või rakendusega autentimisel tõrkeid 5.7.57 või 5.7.3, peaksite kontrollima järgmist.

- Autenditud SMTP-edastus võib olla teie rentnikus või postkastis, mida proovite kasutada(kontrollige mõlemaid sätteid). Lisateavet leiate teemast [Autenditud kliendi SMTP-edastuse lubamine või keelamine.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Kontrollige, [kas teie rentniku jaoks on](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) lubatud Azure'i turbe vaikesätted; kui see on lubatud, nurjub SMTP-autentimine põhiautentimise (ehk pärandi; see kasutab kasutajanime ja parooli) kasutamisel.
