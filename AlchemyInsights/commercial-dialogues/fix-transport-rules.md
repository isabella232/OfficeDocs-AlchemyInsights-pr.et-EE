---
title: Transpordireeglite parandus
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034750"
---
# <a name="fix-transport-rules"></a>Transpordireeglite parandus

Seda sõnumit mõjutas kohandatud meilivoo reegel. Täpse reegli vaatamiseks tehke järgmist.

1. Märkige edastustulemite **jaotises Lisateave** üles **GUID** või **poliitika nimi.**
2. Käivitage Exchange Management Shell. Lisateavet leiate teemast [Halduskesta Exchange avamine.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Käivitage see käsk (kasutades oma edastuse GUID-i):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Vaadake kirjeldus läbi, et näha konfigureeritud tingimusi, mis sõnumit mõjutasid.

Lisateavet leiate teemast [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
