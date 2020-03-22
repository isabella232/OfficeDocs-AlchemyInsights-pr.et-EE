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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891745"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei saa ühiskaustadega ühendust luua

Kui ühiskausta juurdepääs ei tööta mõned kasutajad, proovige järgmist.

Ühendage EXO PowerShelli ja konfigureerige DefaultPublicFolderMailbox parameeter probleemi kasutajakonto sobitada parameeter töö kasutajakonto.

Näide:

Get-postkasti WorkingUser | FT DefaultPublicFolderMailbox, Efektivepublicfoldermailbox

Set-postkasti ProblemUser-DefaultPublicFolderMailbox \<väärtus eelmise käsu>

Muudatuse jõustumiseks oodake vähemalt üks tund.

Kui probleem ei ole, Palun järgige [seda toimingut](https://aka.ms/pfcte) ühiskausta juurdepääsu probleemide tõrkeotsinguks Outlooki abil.