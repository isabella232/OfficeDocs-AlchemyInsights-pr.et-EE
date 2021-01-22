---
title: Sujuv SSO kasutaja sisselogimise probleemid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935121"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Sujuv SSO kasutaja sisselogimise probleemid

Kui kasutaja on autenditud, salvestab brauser kasutaja mandaadi, nii et samale brauserile logib rakendus automaatselt sisse sama kontoga. See võib raskendada, et teine kasutaja või üks kasutaja saab ühes seadmes mitmesse kontosse sisse logida. Selle probleemi lahendamiseks tehke järgmist. Proovige mõnes muus brauseris sisse logida. 2. Tühjendage brauseri vahemälu ja/või küpsised ning proovige uuesti sisse logida.

Kui teil on endiselt probleeme sisselogimise probleemidega, soovitame teil lahendamise juhised diagnoosida ja automatiseerida järgmiselt.

1. Azure ' i portaalis testimise kogemuse kasutamisel saate installida [minu rakenduste turvalise brauseri laienduse](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) , et aidata Azure Active Directory (Azure AD) abil paremini diagnoosida ja kasutada lahendusi.
2. Reprodutseerige tõrge, kasutades Azure ' i portaalis rakenduse konfiguratsiooni lehe funktsioonide testimise kogemust. Lisateavet leiate teemast [SAML põhinevate ühekordse sisselogimise rakenduste silumiseks](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Kui kasutate Azure ' i portaalis testimise kogemust minu rakenduste turvalise brauseri laiendiga, võite **sammu 4 vahele jätta**.
4. SAML-põhise ühekordse sisselogimise konfigureerimise lehe avamiseks tehke järgmist.
    - Avage [Azure ' i portaal](https://portal.azure.com/) ja logige sisse **globaalse administraatorina** või **Coadmin**.
    - Avage **Azure Active Directory laiend** , valides vasakpoolse navigeerimispaani ülaosas **kõik teenused** .
    - Tippige väljale filtri otsing tekst "Azure Active Directory" ja valige **Azure Active Directory** üksus.
    - Valige **Enterprise Applications** Azure Active Directory vasakpoolses menüüs.
    - Kõigi rakenduste loendi kuvamiseks valige **Kõik rakendused** . Kui te ei näe seda rakendust, mida soovite siin kuvada, kasutage **loendi Kõik rakendused** ülaosas olevat **filtri** juhtelementi ja seadke suvand **Kuva** **kõigile rakendustele**.
    - Valige rakendus, mille soovite konfigureerida ühekordse sisselogimise jaoks.
    - Pärast rakenduse laadimist valige rakenduse Vasakpoolsel navigeerimispaanil suvand **Ühekordne sisselogimine** .
    - Valige **SAML põhinev SSO**.
5. Tõrke põhjal leiate lisateavet soovitatavate juhiste kohta leiate teemast [SAML sisselogimisega seotud rakenduste](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)sisselogimine.
6. Muude kasutaja sisselogimise probleemide tõrkeotsinguks vaadake järgmisi juhiseid.
    - [Ühe Sign-On SAML protokoll](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Kuidas: Azure Active Directory aruannete abil sisselogimise tõrgete tõrkeotsing](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Ootamatu nõusoleku viip](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Kasutaja nõusoleku tõrge](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Minu rakendustes sisselogimisega seotud probleemid](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Tõrge rakenduse sisselogimise lehel](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Probleem Microsofti rakendusse sisselogimisel](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
