---
title: Dynamics 365 Formsi ärireeglid – vormi ärireegel ei tööta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947295"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Sündmust OnChange ei toimu, kui välja muudetakse programmiliselt

Sündmust *OnChange* ei toimu, kui välja muudetakse atribuudi abil programmiliselt.  [setValue-meetod.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Kui soovite sündmuseohjureid sündmuse *OnChange* jaoks käivitada pärast väärtuse seadmist, peate koodis kasutama *atribuuti formContext.data.entity* [fireOnchange.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
