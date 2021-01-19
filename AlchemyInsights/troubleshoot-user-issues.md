---
title: Kasutajate probleemide tõrkeotsing
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900878"
---
# <a name="announcements"></a>Teadaanded

Järgige ühilduvuse testimiseks Google ' i juhiseid, et kontrollida, kas teie rakendused on mõjutatud. Google ' i juhised on saadaval https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Veenduge, et kasutate oma kasutajatele Google ' i kontoga sisselogimisel süsteemi WebView või süsteemi brauserit. Lisateavet leiate teemast [rakendusse (desse) sisselogimise probleemid, mis kasutavad ainult Chrome ' i brauserit](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Ma ei saa luua uut kasutajat Azure AD Directorys**

Azure AD uue kasutaja loomise probleemi tõrkeotsingu sooritamiseks tehke järgmist.

1. Veenduge, et teil on õigus luua uus tavakasutaja. Uue tavakasutaja saab luua ainult rakenduses Azure Active Directory (AD) ainult globaalne administraator või kasutaja administraatori roll. Kui te ei ole mõnes sellises rollis, paluge administraatoril lisada teid ühte neist rollidest või luua uus kasutajakonto.
2. Veenduge, et kasutajanimi oleks domeenis, mis on teie Azure AD-s kinnitatud. Kui teil pole Azure ' i REKLAAMIs kinnitatud kohandatud domeeninimesid, saate kasutada oma Azure AD algset domeeni, mis lõpeb *. onmicrosoft.com.
3. Veenduge, et kasutajanimi oleks domeenis, mis pole ühendatud Azure AD-ga teie kohapealsest REKLAAMIst. Kasutajad ei saa pilve lisada kohapealsest välisest domeenist pärit domeeninimega.
4. Veenduge, et ühelgi teisel kasutajal või kontaktil pole juba kasutaja nime, mille soovite uuele kasutajale määrata. Kasutajanimed peavad olema kordumatud Azure ' i REKLAAMIs.
5. Lugege Azure AD [rollide ja administraatorite](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
6. Vaadake oma Azure AD [domeeninimesid](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) .
7. Vaadake üle [auditi logid](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , et näha täpsemat teavet hiljuti loodud või kustutatud kasutaja kohta, kes on toimingu sooritanud ja millal.
8. Uute kasutajate lisamise kohta leiate lisateavet artiklist Azure ' i [reklaamis uue kasutaja loomiseks Azure ' i portaali kasutamine](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Lisateavet administraatori rolli õigused Azure AD, vt [AZURE ad administratiivsed rollid](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Lisateavet Azure AD PowerShelli abil kasutaja loomise kohta leiate teemast [AZURE ad PowerShell uue kasutaja loomiseks](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Probleem iseteeninduse logimisega**

Iseteeninduse logimisega seotud probleemide lahendamiseks tehke järgmist.

1. Oma rakendustes iseteenindusega sisselogimise kasutamiseks luba kõigepealt rentniku jaoks endale registreerumine. 
2. Kui soovite, et rakendus toetaks iseteenindusega registreerumist, lisage see oma kasutaja voo juurde. Järgmine kord, kui lähete selle rakenduse sisselogimise lehele, kuvatakse võimalus **_kontot pole? Loo see!_* _. See käivitab iseallkirjastatud sisselogimise protsessi.
3. Lisateavet selle kohta, kuidas kasutada teenuse kasutajaks registreerumist Azure AD ' is, leiate teemast [teenuse AZURE ad sisselogimine](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Kui seostate kasutaja voolu ühe või mitme rakendusega, saavad kasutajad, kes seda rakendust külastavad, sisse logida ja hankida külaliskonto, kasutades kasutaja voolus konfigureeritud suvandeid. Lisateavet külaliskonto registreerumise ja saamise kohta leiate teemast kasutajate [iseteeninduskeskuse sisselogimine](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

*Probleem välise kasutaja kutsumisega**

Välise kasutaja kutsumisega seotud probleemide lahendamiseks tehke järgmist.

Veenduge, et saadate kasutaja kutse e-posti aadressile, mis vastab selle nimele, milles kasutaja sisse logib. Kui saadate kutse kasutaja puhverserveri meiliaadressile, ei saa kasutaja seda lunastada. Lisateavet leiate teemast [AZURE ad B2B dokumentatsioon](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Kasutajale ei saa litsentse määrata**

Kasutajale litsentside määramisega seotud probleemide lahendamiseks tehke järgmist.

1. Kasutajate litsentside haldamiseks veenduge, et kasutate mõnda nõutud administraatori rollidest kontot: globaalne administraator, litsentsi administraator või kasutaja administraator. Kasutaja rolli saate kontrollida kasutaja Blade ' i vahekaardil **rollid** .
2. Kui kasutate Azure ' i portaali ja litsentsi määramine nurjub, klõpsake paremas ülanurgas olevat teadet. See avab laba, kus on üksikasjad valesti läinud. Enamikul juhtudel piisab probleemi mõistmiseks ja lahendamiseks.
3. Enne kui kasutaja saab litsentsi määrata, veenduge, et kasutajale oleks määratud atribuut **kasutuse asukoht** . Veenduge, et kasutaja on selle atribuudi määranud, kuvades kasutaja laba vahekaardil **profiil** .
4. Veenduge, et selle toote jaoks, mida proovite määrata, oleks piisavalt saadaolevaid litsentse. Azure ' i portaalis saadaolevate litsentside arvu leiate [Azure Active Directory > litsentsidega > kõik tooted](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Kasutajal võib juba olla mõni muu litsents, mille teenused on vastuolus selle uue litsentsiga, mida proovite määrata. Kui kasutajal on näiteks Exchange Online (leping 1) lubatud, siis ei saa te Exchange Online ' iga (leping 2) litsentsi määrata. Keelake mõni teenus, et lubada uue litsentsi määramine. Kui kasutate Azure ' i portaali või PowerShelli cmdlet-käske, loetletakse **probleemi üksikasjade** lehel konkreetsed teenused, mis põhjustavad konflikti.
6. Kui proovite eemaldada litsentsi ja see nurjub, võib kasutajal olla muid litsentse teenustega, mis sõltuvad teenustest, mida proovite eemaldada. Kui kasutate Azure ' i portaali või PowerShelli cmdlet-käske, kuvatakse tõrketeadete loend, mis sisaldab sõltuvustega seotud teenuseid.
7. Kui soovite teada saada, miks kasutaja (nt kes veel teie asutuses teie asutuses) on litsentsi lisanud/eemaldanud, kontrollige auditilogi. Seadke filtriks **litsentsi tegevused** , et kuvada kõik muudatused (sh nende teostatud "näitleja").
8. Kui kasutate Exchange Online ' i, võivad mõned rentniku kasutajad olla valesti konfigureeritud sama puhvri aadressi väärtusega. Sellistel juhtudel võidakse kuvada tõrketeade, kui litsentsi toiming nurjub. [See artikkel](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) sisaldab lisateavet selle probleemi kohta, sh teavet selle kohta, [Kuidas Exchange Online ' iga ühenduse loomine Remote PowerShelli abil](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Kui soovite kindlaks teha, millised teie rentniku kasutajad sisaldavad sama puhverserveri aadressi, käivitage see Exchange Online ' i cmdlet-käsk.

Käivita

Get-Recipient | kus {$ _. EmailAddresses-Match <user principal name> } | fL-i nimi, RecipientType, EmailAddresses





