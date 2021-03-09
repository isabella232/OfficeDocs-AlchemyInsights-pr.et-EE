---
title: Puhverserveri aadressi tõrge ühiskasutatava postkasti loomisel
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568286"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Puhverserveri aadressi tõrge postkasti või muu meili lubatud objekti loomisel

Kui proovisite luua e-posti loaga objekti (postkast, ühiskasutuses postkast jne) ja sai tõrketeate "puhverserveri aadress" SMTP:alias@domain.com "on juba kasutusel...", on teie valitud meiliaadress juba mõne muu teie asutuse jaoks loodud e-posti toega objekt.
  
Peate leidma kasutaja, rühma, ühiskasutatava postkasti või ühiskausta, millel on see meiliaadress, ja kustutama või muutma selle meiliaadressi. Siis saad luua uue e-posti toega objekti koos vabanenud meiliaadressiga. Selle leidmiseks kasutage avalehel otsingut. Selle otsimiseks saate kasutada ka järgmist Exchange Online PowerShelli käsku.

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Kui te ei soovi olemasolevat meiliaadressi kustutada, valige loodava uue objekti jaoks uus meiliaadress.
  