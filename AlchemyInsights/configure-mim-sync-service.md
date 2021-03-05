---
title: MIM sünkroonimise teenuse konfigureerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481353"
---
# <a name="configure-mim-sync-service"></a>MIM sünkroonimise teenuse konfigureerimine

Microsoft Identity Manageri (MIM) sünkroonimise teenus on MIM komponent. See on tsentraliseeritud kohapealne teenus, mis talletab ja integreerib teabe organisatsioonidele, millel on mitu kohapealset kataloogi ja andmebaasi. Võimalik, et saate probleemi lahendada MIM sünkroonimisega, kui probleem on lahendatud hiljutises värskenduses MIM või on mõnest muust jaotisest, mida on kirjeldatud allpool.

**Soovitatavad toimingud**

1. Veenduge, et kasutate MIM sünkroonimise hiljutist värskendust ja kontrollite, kas probleem on värskenduses lahendatud, [MIM sünkroonimisel](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) .
2. Kui probleem on üldise LDAP-i, Generic SQL-i, Lotus Domino või Web Services Connectori abil, veenduge, et kasutate [geneeriliste konnektorite](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)hiljutist värskendamist.
3. Kui MIM sünkroonimisel ilmneb tõrge, lugege võimalike põhjuste määratlemiseks tabelit [käitamise](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) tõrkekoodidest.
4. Kui Run peatub **laiendiga dll-erand**, klõpsake neid sõnu, et avada aken **konnektori ruumi objekti atribuudid** , ja klõpsake nuppu **pinu jälg...** lisateabe saamiseks algpõhjuse kohta, nagu on kirjeldatud jaotises [laiend-DLL-erand](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Kui parool muutmise teatise teenus (PCNS) Component lahendid **tõrge 6025** parooli sünkroonimise ajal sündmuselogi, vaadake [PCNS aruandluse tõrge 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)juhiseid.
6. Kui FIM-i teenuse haldusteguri täielik sünkroonimine on aeglane, märkige jaotises tõrkeotsing säte **Automaatne Grow** for tempdb, nagu on kirjeldatud jaotises [tõrkeotsing aeglase või täieliku sünkroonimise](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)korral.
7. Kui teil on FIM-i teenuse haldamise agendi abil peatatud-server, kus on ebaõnnestunud loomine-kaudu-veebiteenused, lugege teemat [tugiteenused – teave: ebaõnnestunud-loomine-Via-Web-teenused](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) põhjuste ülevaate saamiseks.

