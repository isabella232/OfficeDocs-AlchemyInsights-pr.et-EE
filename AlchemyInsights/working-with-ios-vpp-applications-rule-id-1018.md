---
title: IOS-i VPP-rakenduste reegli Id 1018 abil töötamine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083010"
---
# <a name="working-with-ios-vpp-applications"></a>IOS-i VPP-rakendustega töötamine

Siit [saate teada, kuidas hallata iOS-i](https://docs.microsoft.com/intune/vpp-apps-ios) rakendusi, mis Microsoft Intune ostetud hulgiostuprogrammi kaudu, et saada teavet Apple'i hulgiostuprogrammi kasutamise funktsioonide, piirangute ja juhiste kohta ning selle Microsoft Intune.
  
 **Levinumad probleemid** "I assigned an iOS VPP app to my users, but the installation failed" (I assigned an iOS VPP app to my users, but the installation failed" (I assigned an iOS VPP app to my users, but the installation failed) (I assigned an i
  
- See võib juhtuda siis, kui ühte VPP-luba kasutatakse mitmes mobiilsideseadme haldusteenuse pakkujas. Apple'i VPP-tõendeid saab kasutada ainult ühe teenusepakkujaga. Kui kasutasite mitme teenusepakkujaga VPP-tõend, peate selle uuesti Intune'i üles laadima.

- Installimine võib nurjuda ka siis, kui installide koguarv ületab litsentside arvu. Litsentside kasutusaruande vaatamiseks avage **intune'i mobiilirakenduste** \> **rakenduselitsentside** leht. Teavet selle kohta, kuidas kasutuses litsentse tagasi võtta, leiate [sellest artiklist.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
