---
title: Microsoft Edge ' i tugi Microsoft Defenderi rakenduse Guard jaoks
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583579"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge ' i tugi Microsoft Defenderi rakenduse Guard jaoks

Windows 10 ja Microsoft Edge ' i jaoks loodud rakendus valvur kasutab riistvara-isolatsiooni lähenemist, mis võimaldab kasutajal liikuda ebausaldusväärsel saidil isoleeritud Hyper-V-toega konteineri seest, mis eraldatakse hosti operatsioonisüsteemist.

Ettevõtte administraator määratleb usaldusväärsete veebisaitide, pilve ressursside ja sisemiste võrkude loendi. Kui kasutaja külastab saiti, mida loendis pole, avab Microsoft Edge saidi ümbrises. See tähendab, et kui sait osutub pahatahtlikuks, jääb vastuvõttev arvuti kaitstud ja ründaja ei pääse ettevõtte andmetele juurde.

Pakendis olevate laienduste installimist toetatakse Microsoft Edge ' i versiooni 81 ja seda saab reguleerida poliitika kaudu. UpdateURL-aadress, mida kasutatakse ExtensionInstallForcelist poliitikas, tuleks lisada neutraalse ressursina rakenduse Guard kasutatavas võrgu isolatsiooni poliitikas.

Lisateavet leiate teemast Microsoft Edge ' i [tugi Microsoft Defenderi rakenduse Guard jaoks](https://go.microsoft.com/fwlink/?linkid=2134229).
