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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743950"
---
# <a name="create-user"></a>Kasutaja loomine

**TEADAANNE**

- [Google ' i WebView väljalogimine alates jaanuarist 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Kontrollige, kas teie rakendused võivad mõjutada, järgides [Google ' i juhiseid](https://go.microsoft.com/fwlink/?linkid=2157323) ühilduvuse testimise kohta.
- Veenduge, et kasutate oma kasutajatele Google ' i kontoga sisselogimisel süsteemi WebView või süsteemi brauserit. Lisateavet leiate teemast [rakendusse (desse) sisselogimise probleemid, mis kasutavad ainult Chrome ' i brauserit](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Ma ei saa luua uut kasutajat Azure AD Directorys**

1. Veenduge, et teil on õigus luua uus tavakasutaja. Uue tavakasutaja saab luua ainult rakenduses Azure Active Directory (AD) ainult globaalne administraator või kasutaja administraatori roll. Kui te ei ole mõnes sellises rollis, paluge administraatoril lisada teid ühte neist rollidest või luua uus kasutajakonto.
1. Veenduge, et kasutajanimi oleks domeenis, mis on teie Azure AD-s kinnitatud. Kui teil pole Azure ' i REKLAAMIs kinnitatud kohandatud domeeninimesid, saate kasutada oma Azure AD algset domeeni, mis lõpeb *. onmicrosoft.com.
1. Veenduge, et kasutajanimi oleks domeenis, mis pole ühendatud Azure AD-ga teie kohapealsest REKLAAMIst. Kasutajad ei saa pilve lisada kohapealsest välisest domeenist pärit domeeninimega.
1. Veenduge, et ühelgi teisel kasutajal või kontaktil pole juba kasutaja nime, mille soovite uuele kasutajale määrata. Kasutajanimed peavad olema kordumatud Azure ' i REKLAAMIs.
1. Lugege Azure AD [rollide ja administraatorite](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
1. Vaadake oma Azure AD [domeeninimesid](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) .
1. Vaadake üle [auditi logid](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) , et näha täpsemat teavet hiljuti loodud või kustutatud kasutaja kohta, kes on toimingu sooritanud ja millal.
1. Uute kasutajate lisamise kohta leiate lisateavet artiklist Azure ' i [reklaamis uue kasutaja loomiseks Azure ' i portaali kasutamine](/azure/active-directory/active-directory-users-create-azure-portal).
1. [AZURE ad administratiivsed rollid](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): administraatori rolli õigused Azure Active Directorys
1. [Uue kasutaja loomiseks saate kasutada ka rakendust AZURE ad PowerShell](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
