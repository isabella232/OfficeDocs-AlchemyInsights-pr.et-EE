---
title: Luba postkasti auditeerimine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736249"
---
# <a name="enable-mailbox-auditing"></a>Luba postkasti auditeerimine

Postkasti auditeerimine lubamiseks kas ühe kasutaja või kogu organisatsiooni järgmised cmdlet-käsud tuleb käivitada kaugtöölaua Power Shell:
  
 **Üksik kasutaja**
  
Set-Mailbox-identiteedi "Jane Dow"-AuditEnabled $true
  
 **Organisatsiooni**
  
Get-Mailbox-ResultSize piiramatu-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true
  
[Lisateave](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

