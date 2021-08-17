---
title: Koopiakomplekt
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110676"
---
# <a name="replica-set"></a>Koopiakomplekt

AADDS-i nimetatakse ka hallatavaks domeeniks. See on tegelikult kaks domeenikontrollerit, mida käitab ja haldab tagaprogramm. Kaks DCS-i sisaldavad ühte peamist DC-d ja ühte tiražeerimise DC-d. AADDS-i (hallatava domeeni) varukoopiad on Azure'i platvormi hallatav automaatne protsess. Hallatava domeeniga seotud probleemi korral aitab Azure'i tugi teil varukoopiast taastada.

Iga koopiakomplekti saate luua virtuaalvõrgus. Iga virtuaalvõrk peab olema võrdõigusvõrguga igas teises virtuaalvõrgus, mis majutab hallatava domeeni koopiakomplekti. Selle konfiguratsiooniga luuakse võrgu topoloogia, mis toetab kataloogi paljundust. Virtuaalvõrk saab toetada mitut koopiakomplekti, eeldusel et iga koopiakomplekt asub teises virtuaalses alamvõrgus.

Lisateavet koopiakomplekti kohta leiate teemast [Mõistete koopiakomplektid.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
