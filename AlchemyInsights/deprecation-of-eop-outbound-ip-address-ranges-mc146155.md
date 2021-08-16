---
title: 1065 EOP väljamineva IP-aadressi vahemike deprecation of EOP outbound IP address rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031258"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP väljaminevaTE IP-aadresside vahemike amortiseerumine

Oleme tuvastanud teie ettevõttes võimaliku probleemi, mis (kui seda pole 26. oktoobril 2018 parandamata) võib meilivoog teie kohapeal või välistesse sihtkohtadesse katkeda. Nagu eespool mainitud, konsolideerime IP-aadresside vahemiku haldamise lihtsustamiseks Exchange Online'i kaitseteenus (EOP) IP-aadresside vahemikke, mida kasutatakse meilisõnumite saatmiseks ja vastuvõtuks väljaspool Microsoft 365. Meie analüüs näitab, et üks või mitu meilivoo konnektorites konfigureeritud välist meiliallikat või -sihtkohta ei aktsepteeri siin kuvatud IP-aadresside vahemike [ühendusi.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Tegutsege enne 26. oktoobrit, et tagada, et need allikad ja sihtkohad aktsepteerivad ühendusi kõigi avaldatud [EOP IP-aadressidega ja nendelt.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Lisateavet selle muudatuse kohta leiate teemast Sõnumikeskuse postitused [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)või [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Märkus.** Kui kasutasite lõpp-punktide värskenduste jaoks VAREM IP- või URL-i avaldamist HTML-i, XML-i ja RSS-i kaudu, peaksite seda tüüpi värskenduste automatiseerimiseks migreerima ka uutele veebiteenustele. Lisateavet leiate teemast [lõpp-Microsoft 365 kategooriad ja Microsoft 365 IP-aadressi ja URL-i veebiteenus.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
