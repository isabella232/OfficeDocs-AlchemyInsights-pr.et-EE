---
title: 1065 EOP väljamineva IP-aadressi rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806791"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Väljamineva IP-aadresside vahemike EOP

Oleme tuvastanud teie asutusega võimaliku probleemi, mis (kui seda ei parandatud 26. oktoobril, 2018), võib katkestada meilivoo teie kohapealsetele või välistesse sihtkohtadesse. Nagu varem edastatud, on IP-aadresside vahemiku haldamise lihtsustamiseks koondatud Exchange Online ' i Protection (EOP) IP-aadresside vahemikud, mida kasutatakse meilisõnumite saatmiseks ja vastuvõtmiseks väljaspool Microsoft 365. Meie analüüs näitab, et ühe või mitme välise e-posti allikat või sihtkohta, mille olete konfigureerinud meilivoo konnektorid, ei aktsepteeri [siin](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)esitatud IP-aadresside vahemikke.

Toimige enne 26. oktoobril, et need allikad ja sihtkohad aktsepteerivad ühendusi kõigi [avaldatud EOP IP-aadressidega](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Lisateavet selle muudatuse kohta leiate teemast sõnumikeskuse postitused [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)või [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Märkus**: kui olete varem kasutanud IP-või URL-i avaldamist HTML-, XML-i ja RSS-i lõpp-punktide värskenduste kaudu, peaksite ka migreerima uued veebiteenused, et automatiseerida seda tüüpi värskendusi. Lisateavet leiate teemast [microsoft 365 lõpp-punkti kategooriad ja microsoft 365 IP-aadress ja URL-i veebiteenus](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
