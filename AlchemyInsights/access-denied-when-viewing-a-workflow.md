---
title: Töövoo vaatamisel on juurdepääs keelatud
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955197"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Töövoo vaatamisel on juurdepääs keelatud

SharePoint 2013 töövood, mis proovivad saata meilisõnumeid SharePoint rühmale, võivad nurjuda tõrketeatega "Juurdepääs keelatud", kui rühma SharePoint liikmelisus pole seatud väärtusele Kõik.
  
 **Selle probleemi lahendamiseks tehke järgmist.**
  
 1. Lubage kõigil vaadata rühma SharePoint.
  
 2. Eemaldage SharePoint meilisõnumi realt Adressaat või Koopia.
  
 3. Lisage kasutajad selgesõnaliselt reale Adressaat või Koopia, kui liikmesuse nähtavust ei saa SharePoint muuta.
  
Lisateabe kuvamiseks lugege http-aadressi [/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  