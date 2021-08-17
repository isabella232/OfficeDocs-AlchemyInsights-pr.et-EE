---
title: Enterprise'i rakenduste loendi toomine
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116724"
---
# <a name="get-a-list-of-enterprise-applications"></a>Enterprise'i rakenduste loendi toomine

1. **PowerShelli käsu kaudu** ettevõtterakenduste loendi (kõik rakendused või filtreeritud kuvatava nime, ID, identifikaatori URL-ide jne järgi) leiate teemast [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. PowerShelli käsu kaudu teenusesubjektiobjektide (kõik objektid või ID-ga filtreeritud) loendi leiate teemast [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Kui soovite saada **LOENDIT SAML-i konfigureeritud rakendustest, võivad teid aidata järgmised PowerShelli** skriptid.

    Igal rakendusel on OAuthi rakendus või SAML-i rakendus (nii galerii- kui ka mittegaleriirakendused), kui nende registreerimine toimub, luuakse AAD-s kaks objekti. Ühte nimetatakse rakendusobjektiks ja teine on teenusesubjekti objekt. PowerShelli abil teenusesubjektobjekti atribuutide talletamisel leiate, et igal rakendusel on sellega seotud teatud arv silte, näiteks:

    - OAuthi rakendustel oleks silt nimega "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Galerii SAML-i rakendustel oleks silt nimega "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Mittegalerii saml-rakendustel oleks silt nimega "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication " ("WindowsAzureActiveDirectoryCustomSingleSignOnApplication" ("WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**).

    Seega saate neid silte kasutada ja teada saada, mis tüüpi rakendus see on. Silt "**WindowsAzureActiveDirectoryIntegratedApp**" on levinud igat tüüpi rakenduste jaoks. Kõigi SAML-i rakenduste (nii galerii kui ka mittegalerii) loetlemiseks saate kasutada järgmist koodilõiku.

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Lisateavet leiate teemast [SAML-i toega rakenduste tuvastamine Azure AD-s.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Ainult veebirakenduste portaal** ja loend. Kasutage allolevat käsku, et saada kõik Azure AD rakendused, mille rakenduse tüüp on "Veebirakendus/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Otsige üles ja loetlege ainult kohalikud** rakendused. Kõigi kohalike klientrakenduste (lauaarvuti/mobiilsideseadme) rakenduste toomiseks käivitage järgmine käsk.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Ekspordi kõik registreeritud Azure AD rakenduse üksikasjad** CSV-i. Alloleva käsuga eksporditakse kõik Azure AD rakendused, mille üksikasjad on nõutavad, CSV-faili.

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Kasutamata Azure'i rakenduste loendi eksportimine** – auditiaruanne

    Azure AD saab kuvada rakenduselogisid ainult kuni 30 päeva, kui teil on Azure AD Premium litsents.
    Teil on kaks võimalust andmete säilitamiseks kauemaks kui 30 päevaks. Azure AD aruandluse [API-sid](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) saate kasutada andmete toomiseks programmiliselt ja talletada need andmebaasis. Teise võimalusena saate integreerida auditilogid kolmanda osapoole SIEM-süsteemi.

    Rakenduseloendi saate alla laadida ka kõigi rakenduste ja omatud rakenduste jaoks jaotises Azure Active directory>App Registrations>Download>All applications/Owned applications (Kõik rakendused/omanikule määratud rakendused).

    Ms Graph kaudu rakenduste loendi leiate teemast [Rakenduste loend – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) ja [rakenduse ressursitüüp – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
