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
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057098"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Rakenduse registreerimise lõikekettast puuduvate rakenduste registreerimine

1. Rakenduste registreerimine portaalis ei leia rakendusi.

    Kui rakendus on mitme rentnikuga rakendus ja see on registreeritud mõnes muus rentnikus, ei kuvata seda jaotises Rakenduse registreerimine. Siiski võite selle leida ettevõtterakenduste lõiketera all, kui sellele on juurde pääsetud (pärast nõusoleku saamist) ja teenusesubjekt on teie rentnikus loodud. Lisateavet leiate teemast Azure [AD & teenusesubjektid – Microsofti identimisplatvorm.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Rakendusi ei saa kuvada rakenduse registreerimise labas isegi siis, kui olete administraator.

    Veenduge, et olekste Azure'i portaalis õiges kataloogis.
3. Minu rakendus pole loendis Enterprise Applications blade, kuid see kuvatakse, kui ma powerShelli käsu päringut teen.

    Mõnikord ei ilmu rakendus pärast Azure'i portaalist kustutamist portaalis, kuid see ei pruugi olla täielikult kustutatud. Lisateavet leiate järgmistest teemadest.
    - Saate varem kustutatud rakenduste loendi tuua ja vaadata, kas rakendus kuvatakse loendis PowerShelli **käsuGa Get-AzureADDeletedApplication**. Lisateavet leiate teemast [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Kui soovite rakenduse täielikult eemaldada, proovige PowerShellis järgmist: **Remove-AzureADApplication -ObjectId**. Lisateavet leiate teemast [Eemalda AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Teise võimalusena võite proovida kustutatud rakenduse taastamiseks kasutada järgmist PowerShelli käsku: **AzureADDeletedApplication -ObjectId taastamine.** Lisateavet leiate teemast [AzureADDeletedApplicationi (AzureAD) taastamine.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Ei leia oma uues Azure'i rentnikus kõigi eelinstallitud ettevõtterakenduste loendit.

    Azure AD-s pole vaikimisi eelinstallitud ettevõtterakendusi. Selle peate lisama käsitsi suvandi "Uus rakendus" kaudu, sirvides seda Azure AD galeriist või lisades mittegaleriirakenduse. Lisateavet leiate teemast [Quickstart: Add an application to your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal).
    Kui olete üldadministraator, pääsete rakendustele hõlpsalt juurde [rakendusekäiviti Microsoft 365 kaudu.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Minu rakendusi ei leia portaalist Minu rakendused.

    Veenduge, et rakendused pole lehel Minu rakendused peidetud. Lisateavet leiate teemast [Kogud (eelvaade) portaalis Minu rakendused – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Rakenduste käivitamiseks portaalist Minu rakendused lugege teemat Rakenduste [& portaalis Minu rakendused – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Pärast installimist ei kuvata üleminekurakendust Enterprise Applicationsi teral.

    Rakendus "Office 365 Mover" on mitmeotstarbeline rakendus, mida ei pea AAD-sse lisama jaotise Ettevõtterakenduse registreerimine jaotises Galeriirakendused. Office 365 rakendusele juurdepääsemiseks logige lihtsalt rakendusse sisse ja küsite kasutaja nõusolekut õiguste kohta. Kui kasutaja on andnud nõusoleku, lisatakse see rakendus automaatselt rentnikule koos teie sisse logitud meili ID-ga.

    Pärast rakendusesse sisselogimist peaksite saama AAD-s leida selle rakenduse kirje ettevõtterakenduste tera all. Selle rakenduse otsimiseks tippige täisnimi ehk "Office 365 Mover" või otsige lihtsalt sõna "office". Lisateavet leiate teemast Office 365 Mover ütleb, et see on juba installitud, kuid seda pole [ettevõtterakenduse galeriis loetletud.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. [Kiirülevaade.](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) Kuva nende rakenduste loend, mis kasutavad teie Azure Active Directory (Azure AD) rentnikku identiteedihalduse jaoks, näitab teile, kuidas vaadata rakendusi ehk rakendusi, mis on juba häälestatud kasutama teie Azure AD rentnikku oma identiteedipakkujana (IdP).
9. [Levinud probleemide tõrkeotsing rakenduse lisamisel või eemaldamisel Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) aitab teil mõista levinumaid probleeme, millega inimesed rakenduste vaatamisel Azure Active Directory.
