---
title: Port Google Chrome ' i laiendused Microsoft Edge ' i (kroom)
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
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677286"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Port Google Chrome ' i laiendused Microsoft Edge ' i (kroom)

Google Chrome ' i [laiendusi saab hõlpsalt saata Microsoft Edge ' i (kroom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). Enamikul juhtudel on nende laiendite Microsoft Edge ' i käitamiseks vaja teha ainult minimaalseid muudatusi.

Google Chrome ' i toetatud laiendiga API-d ja manifesti võtmed on ühilduvad Microsoft Edge ' i koodiga. Microsoft Edge ei toeta siiski laiendi APIs Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken ja Chrome. instanceID.