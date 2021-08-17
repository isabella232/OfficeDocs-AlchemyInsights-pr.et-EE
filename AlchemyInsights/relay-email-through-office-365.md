---
title: Meilisõnumite edastamine Microsoft 365 kaudu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 8f8b0780ebec2911b6698deee25e0fabe83bd9afef5fb3a6ef4c51cccd67fc7c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898544"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Mitmeotstarbelise seadme või rakenduse häälestamine meili saatma

Teavet variantide kohta ja juhised leiate artiklist [Mitmeotstarbelise seadme või rakenduse häälestamine Microsoft 365 kaudu meili saatma](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Kui teil on seade või rakendus, mis on hiljuti lõpetanud töötamise, on kõige levinumad probleemid järgmised.

- **Autentimistõrked SMTP-autentimisrakenduse edastuse kasutamisel** Oleme hiljuti teinud mõned muudatused seoses SMTP-autentimise tööga. Probleemide lahendamise kohta leiate lisateavet teemast Printerite, skannerite ja LOB-rakendustega seotud probleemide [lahendamine,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)mis saadavad meilisõnumeid Microsoft 365 või Office 365 .
- Aktsepteerime turvalise ühenduse loomise ajal ainult **TLS 1.2 Office 365** Kui kasutate turvalist ühendust (TLS), veenduge, et teie rakendusseade toetab TLS 1.2. Lisateavet leiate teemast [TLS 1.2 ettevalmistamine Office 365 ja Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Muude probleemide ja lahenduste kohta leiate teavet teemast Probleemide lahendamine printerite, skannerite ja [LOB-rakendustega,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)mis saadavad meilisõnumeid Microsoft 365 või Office 365 .

Mõjutatud seadmete kuvamiseks avage [SMTP autentimise kliendi aruanne](https://protection.office.com/mailflow/dashboard).

**Märkus.** Exchange Online ei mahu hulgipostitusstsenaariumidesse. Hulgimeilisõnumite (nt klientide teabelehtede) saatmiseks peaksite kasutama nendele teenustele spetsialiseerunud kolmanda osapoole teenusepakkujaid.
