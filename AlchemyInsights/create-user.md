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
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896711"
---
# <a name="create-user"></a>Kasutaja loomine

**TEADAANNE:**

- Teenuse WebView sisselogimistoe väljaarvamine [Google'is alates 4. jaanuarist 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Kontrollige, kas ühilduvuse testimise juhised [võivad mõjutada](https://go.microsoft.com/fwlink/?linkid=2157323) teie rakendusi.
- Veenduge, et kasutate kasutajate sisse logimisel Google'i tarbijakontoga süsteemi veebivaadet või süsteemibrauseri. Lisateavet leiate teemast Ainult [Chrome'i brauseri abil rakendus(te)sse sisselogimisega seotud probleemid.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Azure AD kataloogis ei saa uut kasutajat luua**

1. Veenduge, et teil oleks õigus luua uus tavakasutaja. Uue tavakasutaja saab luua ainult Azure Active Directory (AD) üldadministraatori või kasutajaadministraatori rolli. Kui te pole üheski neist rollidest, paluge administraatoril lisada teid ühte neist rollidest või luua uus kasutajakonto.
1. Veenduge, et kasutajanimi oleks teie Azure AD-s kinnitatud domeenis. Kui teil pole Azure AD-s kinnitatud kohandatud domeeninimesid, saate kasutada azure AD algdomeeni, mille lõpus on *.onmicrosoft.com.
1. Veenduge, et kasutajanimi oleks domeenis, mis pole ühendatud teie asutusesisesest AD-st Azure AD-ga. Pilveteenusesse ei saa kasutajaid lisada domeeninimedega, mis on ühendatud asutusesisesest domeenist.
1. Veenduge, et ükski teine kasutaja ega kontakt ei oleks juba loonud kasutajanime, mille soovite uuele kasutajale määrata. Kasutajanimed peavad olema azure AD-s kordumatud.
1. Azure [AD rollide ja administraatorite kohta leiate](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) lisateavet teemast Azure AD rollid ja administraatorid.
1. Vaadake [oma](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD domeeninimesid.
1. Vaadake [läbi auditilogid,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) et näha üksikasjalikumat teavet hiljuti loodud või kustutatud kasutaja kohta(nt toimingu sooritanud ja millal).
1. Lisateavet uute kasutajate lisamise kohta leiate teemast [Azure'i portaali kasutamine azure AD-s uue kasutaja loomiseks.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD haldusrollid:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)administraatori rolliõigused Azure Active Directory
1. Uue kasutaja [loomiseks saate kasutada ka Azure AD PowerShelli.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
