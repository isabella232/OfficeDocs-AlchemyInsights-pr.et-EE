---
title: Klassikalise saidi vahetamine moodsa saidiga
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691175"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Klassikalise saidi vahetamine moodsa saidiga

Kui teie keskkond oli häälestatud enne 2019 aprillini, saate Microsoft PowerShelli abil muuta oma juure modernseks saidiks.

- Kui teil on mõni muu sait, mida soovite kasutada oma juure saidina, saate selle [saidi asendada (swap)](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Kasutage [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , et vahetada saidi asukoht teise saidiga, arhiivides algse saidi. Saadaval nii meeskonnatöö saidi jaoks (pole rühmaga ühendatud) kui ka kommunikatsiooni saidil. 

- Lisavõimalused võetakse kasutusele varsti, mis võimaldab teil saidil olevat sisu kasutada, kuid olemasoleva saidi saidiks teisendada. 
>[!Important]
>Need võimalused on järk-järgult rullitud. Jätkake värskenduste otsimist. 

## <a name="known-issues-with-swapping-sites"></a>Saidid vahetamise teadaolevad probleemid

- Sihtkaust võib tagastada lühikese aja jooksul tõrketeate "ei leitud" (HTTP 404).
- Otsingu indeksi värskendamiseks tuleb sisu uuesti analüüsida. Käsitsi tehtavaid juhiseid pole vaja – seda tehakse automaatselt.
- Midagi, mis sõltub staatilisest lingist (nt failide sünkroonimine ja OneNote ' i failid), tuleb käsitsi parandada.
- Kui lähteteksti sait oli ettevõtte uudiste sait, värskendage URL-i.Hankige kõigi organisatsiooniliste uudiste saitide loend.
- Võimalik, et Project Serveri saidid peavad olema valideeritud, et veenduda, et need on endiselt õigesti seotud.
