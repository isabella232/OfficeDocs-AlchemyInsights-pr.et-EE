---
title: Rakenduse registreerimise lõikekettast puuduvate rakenduste registreerimine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404415"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Rakenduse registreerimise lõikekettast puuduvate rakenduste registreerimine

1. Rakenduste registreerimine portaalis ei leia rakendusi.

    Kui rakendus on mitme rentnikuga rakendus ja see on registreeritud mõnes muus rentnikus, ei kuvata seda jaotises Rakenduse registreerimine. Siiski võite selle leida ettevõtterakenduste lõiketera all, kui sellele on juurde pääsetud (pärast nõusoleku saamist) ja teenusesubjekt on teie rentnikus loodud. Lisateavet leiate teemast Rakendused, [& teenusesubjektid Azure AD-s – Microsofti identiteediplatvormis.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Rakendusi ei saa kuvada rakenduse registreerimise labas isegi siis, kui olete administraator.

    Veenduge, et olekste Azure'i portaalis õiges kataloogis.
3. Minu rakendus pole loendis Enterprise Applications blade, kuid see kuvatakse, kui ma powerShelli käsu päringut teen.

    Mõnikord ei ilmu rakendus pärast Azure'i portaalist kustutamist portaalis, kuid see ei pruugi olla täielikult kustutatud. Lisateavet leiate järgmistest teemadest:
    - Saate varem kustutatud rakenduste loendi tuua ja vaadata, kas rakendus kuvatakse loendis PowerShelli **käsuGa Get-AzureADDeletedApplication**. Lisateavet leiate teemast [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Kui soovite rakenduse täielikult eemaldada, proovige PowerShellis järgmist: **Remove-AzureADApplication -ObjectId**. Lisateavet leiate teemast [Eemalda AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Teise võimalusena võite proovida kustutatud rakenduse taastamiseks kasutada järgmist PowerShelli käsku: **AzureADDeletedApplication -ObjectId taastamine.** Lisateavet leiate teemast [AzureADDeletedApplicationi (AzureAD) taastamine.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Ei leia oma uues Azure'i rentnikus kõigi eelinstallitud ettevõtterakenduste loendit.

    Azure AD-s pole vaikimisi eelinstallitud ettevõtterakendusi. Selle peate lisama käsitsi suvandi "Uus rakendus" kaudu, sirvides seda Azure AD galeriist või lisades mittegaleriirakenduse. Lisateavet leiate teemast [Quickstart: Rakenduse lisamine Azure Active Directory (Azure AD) rentnikule.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Kui olete üldadministraator, pääsete oma rakendustele hõlpsalt juurde [Microsoft 365 rakendusekäiviti abil.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Minu rakendusi ei leia portaalist Minu rakendused.

    Veenduge, et rakendused pole lehel Minu rakendused peidetud. Lisateavet leiate teemast [Kogud (eelvaade) portaalis Minu rakendused – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Rakenduste käivitamiseks portaalist Minu rakendused lugege teemat Rakenduste [& portaalis Minu rakendused – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Moveri rakendust ei kuvata pärast installimist Enterprise Applicationsi teral.

    Rakendus "Office 365 Mover" on mitmeotstarbeline rakendus, mida ei pea AAD-sse lisama jaotise Ettevõtterakenduse registreerimine jaotises Galeriirakendused. Office 365 Moveri rakendusele juurdepääsemiseks logige lihtsalt rakendusse sisse ja küsiks kasutaja nõusolekut õiguste kohta. Kui kasutaja on andnud nõusoleku, lisatakse see rakendus automaatselt rentnikule koos teie sisse logitud meili ID-ga.

    Pärast rakendusesse sisselogimist peaksite saama AAD-s leida selle rakenduse kirje ettevõtterakenduste tera all. Selle rakenduse otsimiseks tuleb tippida täisnimi ehk "Office 365 Mover" või lihtsalt otsida sõna "office" ja see peaks rakenduse loetlema. Lisateavet leiate teemast [Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)ütleb, et see on juba installitud, kuid seda pole ettevõtterakenduse galeriis loetletud.
8. [Kiirülevaade. Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) rentnikku identiteedihalduse jaoks kasutava rakenduste loendi abil saate vaadata rakendusi ehk rakendusi, mis on juba häälestatud kasutama teie Azure AD rentnikku oma identiteedipakkujana (IdP).
9. [Azure Active Directorysse rakenduse lisamise või eemaldamise](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) levinud probleemi tõrkeotsing aitab teil mõista levinumaid probleeme, millega inimesed Azure Active Directory rakenduste vaatamisel kokku seisavad.
