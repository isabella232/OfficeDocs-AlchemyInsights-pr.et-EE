---
title: Andmete Microsoft Edge muutmiseks saate kasutada andmekataloogi muutujaid, mitte hardcoded paths
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113412"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Andmete Microsoft Edge muutmiseks saate kasutada andmekataloogi muutujaid, mitte hardcoded paths

Kui soovite näiteks Windows salvestada profiiliandmed kasutaja kohaliku rakenduse andmete all, mitte vaikeasukohas, määrake **poliitika UserDataDir** väärtuseks **${local_app_data}\Edge\Profile**. 

Lisateavet leiate teemast [Kasutajaandmete Microsoft Edge loomine.](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)