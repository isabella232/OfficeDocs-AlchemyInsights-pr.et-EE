---
title: Puhverserveri aadressi tõrge ühispostkasti loomisel
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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062904"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Puhverserveri aadressi tõrge postkasti või muu meilis lubatud objekti loomisel

Kui proovisite luua meiliga toega objekti (postkast, ühispostkast jne) ja saite tõrketeate "Puhveraadress "SMTP:alias@domain.com" on juba kasutusel...", on teie valitud meiliaadress juba võetud teie ettevõttes mõne muu meiliga toega objekti poolt.
  
Peate selle meiliaadressiga kasutaja, rühma, ühispostkasti või avaliku kausta üles otsima ja selle kustutama või selle meiliaadressi muutma. Seejärel saate vaba meiliaadressiga luua uue meiliga toega objekti. Kasutage selle leidmiseks avalehel otsingut. Selle otsimiseks saate Exchange Online powerShelli käsu abil.

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Kui te ei soovi olemasolevat meiliaadressi kustutada, valige uue objekti jaoks uus meiliaadress.
  