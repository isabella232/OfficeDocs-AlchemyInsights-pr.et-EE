---
title: Ühiskaustadele ei pääse juurde
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959491"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei saa ühiskaustadega ühendust luua

Kui ühiskausta juurdepääs ei tööta vähe kasutajaid, proovige järgmist.

Ühendage EXO PowerShelli ja konfigureerige DefaultPublicFolderMailbox probleemi kasutajakonto sobitada ühe töö kasutaja konto.

Näide:

Get-postkasti WorkingUser | FT DefaultPublicFolderMailbox, Efektivepublicfoldermailbox

Set-postkasti ProblemUser-DefaultPublicFolderMailbox \<väärtus eelmise käsu>

Muudatuse jõustumiseks oodake vähemalt üks tund.