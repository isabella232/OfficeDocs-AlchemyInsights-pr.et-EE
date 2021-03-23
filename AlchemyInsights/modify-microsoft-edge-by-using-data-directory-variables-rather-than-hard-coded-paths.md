---
title: Microsoft Edge ' i muutmine, kasutades andmete kataloogi muutujaid, mitte kõva koodiga teed
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035283"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Microsoft Edge ' i muutmine, kasutades andmete kataloogi muutujaid, mitte kõva koodiga teed

Kui soovite näiteks Windowsis talletada andmed kasutajate kohaliku rakenduse andmete alusel, mitte vaikeasukohta, määrake *UserDataDir* poliitikaks **$ {local_app_data} \Edge\Profile**.

Lisateavet leiate teemast [Microsoft Edge ' i kasutajate andmete kataloogi muutujate loomine](https://docs.microsoft.com/deployedge/microsoft-edge-policies).