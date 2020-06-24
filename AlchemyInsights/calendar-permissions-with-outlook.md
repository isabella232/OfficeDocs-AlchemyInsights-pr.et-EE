---
title: Kalendri õigused
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862057"
---
# <a name="calendar-permissions"></a>Kalendri õigused

Kasutajad saavad muuta oma kalendriõigusi Outlooki veebirakenduse või muude klientidega, kuid administraatorina peate võib-olla uurima ka.  
Exchange PowerShelli cmdlet-käsuga kuvatakse kasutaja kalendris olev õigus.

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Lisateabe saamiseks vaadake järgmist.

- [Get-MailboxFolderPermission (Get-MailboxFolderPermission)](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission (Set-MailboxFolderPermission)](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission (Add-MailboxFolderPermission)](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendriõigusi kasutatakse kalendrite ühiskasutuses, et näha lisateavet Outlooki kalendri ühiskasutuse kohta, lugege järgmisi artikleid.

- [Outlooki kalendri ühiskasutus](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalendri ühiskasutusse andmine Outlooki veebirakenduses ettevõttejaoks](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Kalendriõiguste tõrkeotsinguks saate kasutada [tugi- ja taasteabimehe](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tööriista.