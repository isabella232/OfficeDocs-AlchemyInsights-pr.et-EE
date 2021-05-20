---
title: Kasutaja loomine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569717"
---
# <a name="create-user"></a>Kasutaja loomine

**TEADAANNE:**

- Teenuse WebView sisselogimistoe väljaarvamine [Google'is alates 4. jaanuarist 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Kontrollige, kas ühilduvuse testimise juhised [võivad mõjutada](https://go.microsoft.com/fwlink/?linkid=2157323) teie rakendusi.
- Veenduge, et kasutate kasutajate sisse logimisel Google'i tarbijakontodega süsteemi veebivaadet või süsteemibrauseri. Lisateavet leiate teemast Ainult [Chrome'i brauseri abil rakendus(te)sse sisselogimisega seotud probleemid.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Azure AD kataloogis ei saa uut kasutajat luua**

1. Veenduge, et teil oleks õigus luua uus tavakasutaja. Uue tavakasutaja saab luua ainult Azure Active Directory (AD) üldadministraatori või kasutajaadministraatori rolli. Kui te pole üheski neist rollidest, paluge administraatoril lisada teid ühte neist rollidest või luua uus kasutajakonto.
1. Veenduge, et kasutajanimi oleks teie Azure AD-s kinnitatud domeenis. Kui teil pole Azure AD-s kinnitatud kohandatud domeeninimesid, saate kasutada Azure AD algdomeeni, mille lõpus on *.onmicrosoft.com.
1. Veenduge, et kasutajanimi oleks domeenis, mis pole ühendatud teie asutusesisesest AD-st Azure AD-ga. Pilveteenusesse ei saa kasutajaid lisada domeeninimedega, mis on ühendatud asutusesisesest domeenist.
1. Veenduge, et ükski teine kasutaja ega kontakt ei oleks juba loonud kasutajanime, mille soovite uuele kasutajale määrata. Kasutajanimed peavad olema azure AD-s kordumatud.
1. Azure [AD rollide ja administraatorite kohta leiate](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) lisateavet teemast Azure AD rollid ja administraatorid.
1. Vaadake [oma](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD domeeninimesid.
1. Vaadake [läbi auditilogid,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) et näha üksikasjalikumat teavet hiljuti loodud või kustutatud kasutaja kohta(nt toimingu sooritanud ja millal).
1. Lisateavet uute kasutajate lisamise kohta leiate teemast [Azure'i portaali abil azure AD-s uue kasutaja loomine.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD haldusrollid:](/azure/active-directory/active-directory-assign-admin-roles)administraatori rolliõigused Azure Active Directory
1. Uue kasutaja [loomiseks saate kasutada ka Azure AD PowerShelli.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
