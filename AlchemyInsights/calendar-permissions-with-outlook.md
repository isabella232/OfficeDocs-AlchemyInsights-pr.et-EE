---
title: Kalendriõigused
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046100"
---
# <a name="calendar-permissions"></a>Kalendriõigused

Kasutajad saavad oma kalendriõigusi muuta Outlook või muude klientidega, kuid administraatorina peate võib-olla ka uurima.  
PowerShelli Exchange korral kuvatakse teile kasutaja kalendris õigused.

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Lisateabe saamiseks vaadake järgmist.

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendriõigusi kasutatakse kalendrite ühiskasutuses, et saada lisateavet kalendri ühiskasutusse Outlook kohta leiate järgmisest artiklist.

- [Outlooki kalendri ühiskasutus](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalendri ühiskasutusse Outlooki veebirakendus ettevõtterakenduses](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Kalendriõiguse tõrkeotsinguks saate kasutada [tugi- ja taasteteenuste abiline](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tööriista.