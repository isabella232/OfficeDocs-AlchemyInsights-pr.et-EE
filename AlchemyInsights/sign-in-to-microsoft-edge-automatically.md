---
title: Logi sisse Microsoft Edge automaatselt
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050690"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logi sisse Microsoft Edge automaatselt

Microsoft Edge kasutab opsüsteemi vaikekontot kasutaja automaatseks sisselogimiseks vastavalt sellele, kuidas kasutaja seade on konfigureeritud. 

Allpool kirjeldatakse igat tüüpi seadme konfiguratsiooni ja sellest sõltuva kasutaja sisselogimisprotsessi stsenaariume.

- **Seade on hübriid/AAD-J.** See suvand on saadaval Windows 10, Windows ja vastavates serveriversioonides. Kasutajad logitakse automaatselt sisse oma Azure Active Directory (AD)kontodega.
- **Seade on domeeniga ühendatud.** See suvand on saadaval Windows 10, Windows ja vastavates serveriversioonides. Vaikimisi ei logita domeenikontodega kasutajad automaatselt sisse; nende jaoks automaatse sisselogimise lubamiseks kasutage **poliitikat ConfigureOnPremisesAccountAutoSignIn.** Azure AD-kontodega kasutajate jaoks automaatse sisselogimise lubamiseks kaaluge nende seadmete hübriidjuurutust.
- **OS-i vaikekonto** on Microsofti konto. See suvand on saadaval Windows 10 RS3 (versioon 1709, järk 10.0.16299) ja uuemates versioonides. See stsenaarium ei ole ettevõtte seadmetes tõenäoline. Kui os-i vaikekonto on Microsofti konto, siis Microsoft Edge logib kasutaja automaatselt sisse Microsofti kontoga.
 
 
