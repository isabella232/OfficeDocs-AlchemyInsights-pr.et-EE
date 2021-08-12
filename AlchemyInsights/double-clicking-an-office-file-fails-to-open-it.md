---
title: Topeltklõpsake faili, Office faili ei avane
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965097"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Topeltklõpsake faili, Office faili ei avane

Pärast faili topeltklõpsamist Office võib programm olla avatud, kuid fail ise ei avane. Samuti võidakse kuvada tõrketeade "Ilmnes probleem käsu programmile saatmisega". Selleks on mitu põhjust, kuid kaks kõige levinuimat lahendust on järgmised.

- Veenduge Excel, et suvand DDE oleks märkimata. Suvandi leiate, kui loote uue töövihiku ja valite seejärel käsu Fail **> Suvandid > Täpsemalt**. Tühjendage **jaotises Üldist** ruut Ignoreeri muid rakendusi, mis kasutavad dünaamilisi Exchange **(DDE).**

- Käivitage vaikesätete taastamiseks veebitaaste. Klõpsake nuppu Windows Start ja otsige sõna "Control Panel" (Juhtpaneel). Avage **juhtpaneel ja valige** Programmid **> Programmid ja funktsioonid**. Seejärel paremklõpsake käsku **Microsoft Office [Versioon]** ja valige **Muuda > Paranda** võrgus.

Kui kumbki neist lahendustest ei toimi, leiate tugiteenuste artiklist täielikuma lahenduste loendi, kui faili Office ei [avane.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
