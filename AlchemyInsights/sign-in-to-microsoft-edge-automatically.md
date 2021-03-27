---
title: Microsoft Edge'i automaatne sisselogimine
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398725"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Microsoft Edge'i automaatne sisselogimine

Microsoft Edge kasutab operatsioonisüsteemi vaikekontot kasutaja automaatseks sisselogimiseks vastavalt kasutaja seadme konfigureerimise viisidele. 

Allpool kirjeldatakse igat tüüpi seadme konfiguratsiooni ja sellest sõltuva kasutaja sisselogimisprotsessi stsenaariume.

- **Seade on hübriid/AAD-J.** See suvand on saadaval opsüsteemis Windows 10, windowsi allatasemel ja vastavates serveriversioonides. Kasutajad logitakse automaatselt sisse oma Azure Active Directory (AD) kontodega.
- **Seade on domeeniga liidetud.** See suvand on saadaval Opsüsteemis Windows 10, windowsi allatasemel ja vastavates serveriversioonides. Vaikimisi ei logita domeenikontodega kasutajad automaatselt sisse; nende jaoks automaatse sisselogimise lubamiseks kasutage **poliitikat ConfigureOnPremisesAccountAutoSignIn.** Azure AD-kontodega kasutajate jaoks automaatse sisselogimise lubamiseks kaaluge nende seadmete hübriidjuurutust.
- **Os-i vaikekonto** on Microsofti konto. See suvand on saadaval opsüsteemis Windows 10 RS3 (versioon 1709, järk 10.0.16299) ja uuemates versioonides. See stsenaarium ei ole ettevõtte seadmetes tõenäoline. Kui aga os-i vaikekonto on Microsofti konto, logib Microsoft Edge kasutaja automaatselt sisse Microsofti kontoga.
 
 
