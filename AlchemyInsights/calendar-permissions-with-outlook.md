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
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819904"
---
# <a name="calendar-permissions"></a>Kalendriõigused

Kasutajad saavad outlooki veebirakenduses või muudes klientklientides muuta oma kalendriõigusi, kuid administraatorina peate võib-olla ka uurima.  
Exchange PowerShelli cmdlet-käsuga kuvatakse teile kasutaja kalendris olevad õigused.

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Lisateabe saamiseks vaadake järgmist.

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendriõigusi kasutatakse kalendrite ühiskasutuses, et saada lisateavet Outlooki kalendri ühiskasutuse kohta, leiate järgmisest artiklist.

- [Outlooki kalendri ühiskasutus](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalendri ühiskasutus Outlooki veebirakenduse ettevõtterakenduses](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Kalendriõiguse tõrkeotsinguks saate kasutada [tugi- ja taasteteenuste abilise](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tööriista.