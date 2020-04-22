---
title: 1065 EOP väljaminev IP-aadressi deprecation rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704593"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP väljaminevate IP-aadresside vahemike keelamine

Oleme tuvastanud potentsiaalse probleemi teie organisatsioonis, et (kui ei korrigeerita oktoober 26th, 2018) võib murda meilivoog asutusesisese või väliste sihtkohtade. Nagu varem edastatud, lihtsustada IP-aadresside vahemiku haldamine, me konsolideeritakse Exchange Online Protection (EOP) IP aadressi vahemikud, mida kasutatakse saata ja vastu võtta e-posti väljaspool Microsoft 365. Meie analüüs näitab, et üks või mitu välist e-posti allikad või sihtkohad, mis on konfigureeritud e-posti voog konnektorid ei aktsepteeri ühendusi [siin](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)näidatud IP-aadresside vahemikud.

Seaduse enne oktoober 26th tagada nende allikate ja sihtkohtade aktsepteerivad ühendusi ja kõik [avaldatud EOP IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Selle muudatuse kohta lisateabe saamiseks lugege Message Center postitusi [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)või [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Märkus**: kui KASUTASITE varem IP või URL-i avaldamine HTML-i, XML-i ja RSS-i lõpp-punkti värskenduste jaoks, peaksite ka uude veebiteenusse seda tüüpi värskenduste automatiseerimiseks rändama. Lisateabe saamiseks vaadake [microsoft 365 lõpp-punkti kategooriad ja microsoft 365 IP-aadress ja URL-i veebiteenus](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
