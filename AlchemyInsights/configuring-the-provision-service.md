---
title: Ettevalmistamise teenuse konfigureerimine
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
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033274"
---
# <a name="configuring-the-provision-service"></a>Ettevalmistamise teenuse konfigureerimine

Kasutajate automaatseks ettevalmistamiseks tööks on Azure AD-l vaja kehtivat identimisteavet, mis võimaldavad tal luua ühenduse tööpäev veebiteenuste API-ga. Lisaks valideerib rakendus Workday to AD User Provisioning (Testi ühendust) nupp Test Connection (Testi ühendust) ka siis, kui see saab luua ühenduse AD Ühendus domeeniga seotud Azure AD-ettevalmistamise agendiga.

Kui Azure'i portaal tagastab identimisteabe salvestamisel tõrke, järgige alltoodud juhiseid.

1. Veenduge, et olete konfigureerinud tööpäevaintegratsiooni süsteemi kasutajakonto, nagu on märgitud jaotises [Integratsioonisüsteemi kasutaja konfigureerimine tööpäeval.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Veenduge, et Azure AD Ühendus ettevalmistamise agenditeenus on teie teenuste halduskonsooli abil teie Windows serveris töötav. Agendi oleku vaatamiseks Azure'i portaalis klõpsake nuppu Kuva kohapealsed agendid.
3. Veenduge, et sisestate välja "Tööpäev kasutajanimi" väärtuse, kasutades username@workday-rentniku-nime. Kui tööpäev-rentniku-nimi puudub, siis tööpäeva autentimine nurjub.
4. Kui konfigureerite integreerimist workday'i rakenduse rentnikuga, pange tähele oma tööpäeva rentniku ajastatud töötunnid. Workday on kavandanud oma rakendus rentnike jaoks nädalavahetuse (tavaliselt reede õhtult laupäeva hommikuni) aega ja ühenduvustõrked selle ajal on teadaolev probleem, mis automaatselt lahendatakse kohe, kui rakendus rentnikud on taas võrgus.
5. Harvadel juhtudel võidakse see tõrge kuvada ka juhul, kui integratsioonisüsteemi kasutaja parool on rentniku värskendamise tõttu muutunud või kui konto on lukustatud või aegunud. Kontrollige oma tööpäeva administraatoriga integreerimissüsteemi kasutaja olekut.

Lisateavet automaatseks ettevalmistamiseks tööpäevade konfigureerimise kohta leiate teemast [Õpetus: Tööpäeva konfigureerimine automaatseks kasutajate ettevalmistamiseks.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
