---
title: 1332 OWA-sisendkausta reegel (ID) ei Käivita postkasti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721587"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Sisendkausta reegel ei tööta ootuspäraselt

Kontrollige Outlooki veebirakenduses järgmisi sätteid.

- Sõnumi saab ümber suunata, edasi saata või vastatud automaatselt sisendkausta reeglite alusel ainult üks kord. Ümbersuunamise reegel (sisendkausta reegel või meilivoo reegel, mida tuntakse ka transpordiviisina) saab sõnumile lisada kuni kümme adressaati. Lisateavet leiate teemast [töölehe, transpordi ja sisendkausta reegli piirangud](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Sisendkausta reeglid ei tööta alternatiivsel Journali postkastil. Lisateavet alternatiivse Journali postkasti kohta leiate teemast [postkasti alternatiivne päevik](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Nende probleemide lahendamiseks lugege teemat [KB 2829319](https://support.microsoft.com/kb/2829319).

Kui varasemaid probleeme ei rakendata, käivitage enne probleemi lahendamist Microsofti toega sisendkausta reegel diagnostiline ülevaade.

1. Avage postkast Outlooki veebirakenduses ja klõpsake nuppu <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Sätted**  >  **Kõigi Outlooki sätete kuvamine**  >  **Meil**  >  **Reeglid**.

2. Klõpsake lehe allservas, **kui teie reeglid ei tööta, klõpsake siin, et luua diagnostiline ettekanne**.
