---
title: Logige Microsoft Edge ' i automaatselt sisse
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677235"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logige Microsoft Edge ' i automaatselt sisse

Microsoft Edge kasutab OPERATSIOONISÜSTEEMI vaikesätet automaatselt kasutaja sisselogimiseks vastavalt sellele, kuidas kasutaja seade on konfigureeritud. 

Iga tüüpi seadme konfiguratsiooni ja selle sõltuva kasutaja sisselogimise stsenaariumid on kirjeldatud allpool.

1. **Seade on hübriid/AAD-J**: see suvand on saadaval opsüsteemis Windows 10, ülataseme Windowsi ja vastavate serveri versioonide korral. Kasutajad logitakse automaatselt sisse oma Azure Active Directory (AD) kontodega.
2. **Seade on domeeniga liitunud**: see suvand on saadaval opsüsteemis Windows 10, Downi Windowsi ja vastavate serveri versioonide korral. Vaikimisi ei logita domeeni kontode kasutajad automaatselt sisse; automaatse sisselogimise lubamiseks kasutage **ConfigureOnPremisesAccountAutoSignIn** poliitikat. Azure AD Accounts kasutajate automaatse sisselogimise lubamiseks kaaluge hübriidiga liitumist oma seadmetega.
3. **Operatsioonisüsteemi vaikekonto on Microsofti konto**: see suvand on saadaval opsüsteemis Windows 10 RS3 (versioon 1709, järk 10.0.16299) ja uuemates versioonides. Stsenaarium ei esine tõenäoliselt Enterprise Devices. Kui aga OS-i vaikekonto on Microsofti konto, logib Microsoft Edge kasutaja automaatselt sisse Microsofti kontoga.
 
 
