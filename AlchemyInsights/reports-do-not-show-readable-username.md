---
title: Microsoft 365 halduskeskuse aruanded ei kuva loetavat kasutajanime
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327810"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Microsoft 365 halduskeskuse aruanded ei kuva loetavat kasutajanime

Microsoft 365 halduskeskuse aruanded ei kuva kasutajanime, vaid kuvavad selle asemel tähtnumbrilisi väärtusi, nagu B2BC6C15BB9FCDEA71E5CD302D228CC8.

Selline käitumine on ootuspärane ja sellest on teatatud sõnumikeskuses (MC275344, avaldatud 3. augustil 2021). 

Üldadministraatorid saavad selle muudatuse oma rentniku jaoks tagasi pöörata ja kuvada tuvastatavat kasutajateavet, kui nende organisatsiooni privaatsustavad seda lubavad. Rentniku muudatuse tagasipööramiseks tehke järgmist.

1. Avage halduskeskuses **Sätted** > **Organisatsiooni sätted** > [**Teenused**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) ja valige suvand **Aruanded**. 
1. Jaotises **Kasutajateabe kuvamisviisi valimine** valige **Kuva aruannetes tuvastatav kasutajateave** ja käivitage aruanne uuesti.