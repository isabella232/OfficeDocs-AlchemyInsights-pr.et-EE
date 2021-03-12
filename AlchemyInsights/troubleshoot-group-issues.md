---
title: Rühma probleemide tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713648"
---
# <a name="troubleshoot-group-issues"></a>Rühma probleemide tõrkeotsing

**Mul on vaja määrata rühma Azure AD rollile**

Azure Active Directory (AD) rühma määramiseks Azure AD rollile tehke järgmist.

1. Uue rühma loomine – uue rühma loomiseks tehke järgmist.

    loomine. Logige sisse Azure AD halduskeskus, millel on priviligeeritud rollide administraator või üldadministraatori õigused. 
    b. Valige Azure Active Directory > rühmad > kõik rühmad > uus rühm. 
    c. Looge rühm.

2. Määrake rühmale roll rühma loomise ajal või pärast rühma loomist.

    loomine. Rühmale rolli määramiseks rühma loomise ajal lülitage sisse lüliti Azure AD rollid, mida saab rühmale määrata ja rühma luua.
    b. Kui soovite rühmale rolli määrata pärast selle loomist, liikuge vastloodud rühma jaoks menüüsse määratud rollid ja määrake roll rühmale.

**Mul on vaja hallata Azure AD rollile määratud rühma liikmestaatust**

1. Õiguste suurendamise takistamiseks saab vaikimisi kasutada ainult privilegeeritud rolli administraator ja globaalne administraator. Nad saavad siiski määrata sellise rühma omaniku ja selle ülesande delegeerida. Lisateavet leiate teemast [pilve rühmade kasutamine rolli ülesannete haldamiseks Azure ' i Active Directorys](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Levinumad küsimused ja tõrkeotsingu näpunäited Azure AD rühmadesse rollide määramiseks leiate teemast [pilve rühmade jaoks määratud rollide tõrkeotsing](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dünaamilised rühmad**

1. Kui te ei leia sisseehitatud kasutaja atribuute, veenduge, et atribuut oleks toetatud atribuutide loendis.
2. Kui otsite sisseehitatud seadme atribuute, veenduge, et atribuut oleks seadme atribuutide loendis. 
3. Lisaks sisseehitatud kasutaja ja seadme atribuutidele võite kasutada ka [laienduse atribuute](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Pärast laienduse atribuutide sünkroonimist kohapealsest Windows Server AD või ühendatud SaaS-rakendusest peaks atribuudid olema reegli ehitaja ripploendis nähtavad. Kohandatud atribuudi nime leiate kataloogist, kui päringute kasutaja atribuut PowerShelli abil ja otsitakse atribuudi nime. Neid võib kasutada ka reegli süntaksis reeglite koostamiseks.
4. Veenduge, et teie Rentnik on sobiv litsents. Dünaamilised rühmad nõuavad, et rentnik saaks Azure AD P1 Premiumi litsentsi. Azure AD litsentside lepingute loendit saab kasutada [siin](https://azure.microsoft.com/pricing/details/active-directory/). Enterprise mobiilsus + turvalisuse litsentside lepingud pääseb [siia](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)juurde.
5. Veenduge, et dünaamilise rühma loomise kasutaja roll oleks globaalne administraator, Intune Administrator, rühma administraator või kasutaja administraator.
6. Palun lubage rühmal aeg asustada. Olenevalt teie rentniku suurusest võib rühm võtta aega kuni 24 tundi, et asustada esimest korda või pärast reegli muutmist.
7. Lisateavet leiate teemast [atribuudi-põhiste reeglite loomine dünaamilise rühma liikmestaatuse jaoks](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Ma pean rühma kustutama**

1. Rühmi saab kustutada kataloogist, kasutades Azure AD PowerShelli moodulis Remove-AzureADGroup cmdlet-käsku.
2. Enne kui proovite Azure AD sünkroonitud rühma kustutada, veenduge, et olete kustutanud kõik määratud litsentsid tõrgete vältimiseks.
3. Lisateavet rühmade kustutamise kohta leiate teemast [rühma kustutamine määratud litsentsiga](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Kustutatud rühma taastamine**

1. Kui Office 365 rühm on kustutatud, saab seda taastada ainult kuni 30 päeva enne jäädavalt kustutamist. Kui olete jäädavalt kustutanud, ei saa rühma enam taastada. Lisateavet rühmade taastamise kohta leiate [siit](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. See funktsioon ei toeta turbe-ja levirühma.
3. Veenduge, et teil on Office 365 rühma taastamine lubatud. Globaalsed administraatorid, rühma administraatorid, kasutajakonto administraatorid, Intune ' i teenuse administraatorid, partneri TIER1 või tier2 tugi ja rühma omanik saab taastada rühma.
4. Kui dünaamiline rühm kustutatakse ja taastatakse, kuvatakse see uue rühmana ja asustatakse uuesti vastavalt reeglile. See protsess võib kuluda kuni 24 tundi.
5. Lisateavet kustutatud rühma taastamise kohta leiate teemast [Kustutatud Office 365 rühma taastamine Azure ' i Active Directorys](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Rühma aegumise poliitika konfiguratsioon**

1. See funktsioon on toetatud ainult Office 365 rühmade jaoks, kuid mitte turbe-ja levirühmade puhul, mida ei toetata.
2. Office 365 rühmade aegumise poliitika konfigureerimine ja kasutamine nõuab Azure AD Premiumi litsentsi.
3. Praegu saab rentniku jaoks konfigureerida Office 365 rühmade jaoks vaid ühe aegumise poliitika.
4. Rühma saab uuendada ainult globaalsed administraatorid, rühma administraatorid, kasutaja administraatorid ja rühma omanik.
5. Kui Office 365 rühm on aegunud, siis see kustutatakse ja seda saab taastada ainult kuni 30 päeva enne jäädavalt kustutamist. Kui olete jäädavalt kustutanud, ei saa rühma enam taastada. Lisateavet rühmade taastamise kohta leiate [siit](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Tegevusel põhinev automaatne pikendamine**

SharePointi, Outlooki ja meeskondade kasutaja tegevused võivad vallandada rühma automaatse pikendamise. Tegevusi kontrollitakse 35 päeva enne, kui rühm aegub. Kui praeguse rühma elutsükli ajal on tegevust, pikendatakse rühma automaatselt ja meilisõnumeid ei saadeta rühma omanikele.

**Aegunud rühmade teatiste ajastus**

1. Meilisõnumite teatised saadetakse Office 365 rühma omanikele 30 päeva, 15 päeva ja 1 päev enne rühma aegumist.
2. Kui te esimest korda häälestate, on kõik rühmad, mis on vanemad kui aegumise intervall, seatud kuni 35 päevani.
3. Grupi aegumiskuupäev arvutatakse grupi uuendamise kuupäeva põhjal, mis ei põhine poliitika värskendatud kuupäeval. Kui aegumise poliitika on värskendatud, siis aegumistähtaega ei muudeta.
4. Lisateavet leiate teemast [rühma aegumise poliitika ja pikendatud meilisõnumid](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) ning [taastada kustutatud Office 365 rühma Azure Active Directorys](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Rühma loomise õigus**

Veenduge, et teil on õigus luua uus rühm. Globaalsed administraatorid saavad rühma loomise keelata Azure ' i portaalis või Accessi paanil. Teil võib olla vaja administraatorit, et luua uus rühm või anda teile vastavad õigused.

1. [Uue rühma loomine ja liikmete lisamine Azure ' i portaalis](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Rühmade loomine PowerShelli MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Rühmade loomise keelamine PowerShellis](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Saate hallata, kes saavad Office 365 rühmi luua](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Office 365 tervituse keelamine PowerShelli kaudu](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD administratiivsed rollid](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Rühma loomise õiguse haldamine**

1. Globaalsed administraatorid saavad hallata Azure ' i portaalis või Accessi paneelis loodud turbe-või Office 365 rühmade loomise õiguseid, seades **kasutajate jaoks Azure** ' i portaalis turberühma või **kasutajad saavad luua Office 365 rühmi Azure** ' i portaalide sätetes **kõigis rühmades > General (sätted**
2. Kui teil on Azure AD P1 Premiumi litsents, saate rühma loomist piirata ka kasutajate rühma valimiseks.

**Office 365 rühma uute liikmete tervituste teatise keelamine**

Office 365 rühmadesse lisatud kasutajatele, kes on lisatud Office rühmadesse, saab keelata, kui säte on `UnifiedGroupWelcomeMessageEnabled` PowerShellis **FALSE** . [Siit](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)saate teada, kuidas see säte käib.













