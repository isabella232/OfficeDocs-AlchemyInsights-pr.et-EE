---
title: Active Directoryt ei sünkroonita
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889214"
---
# <a name="active-directory-not-syncing"></a>Active Directoryt ei sünkroonita

Kui saate sünkroonimistõrkeid (nt "viimatist sünkroonimist pole" või märkate kataloogisünkroonimise olekut Office haldusportaalis, ütleb "Viimati sünkroonitud rohkem kui 3 päeva tagasi", võib olla see, et AADConnectil on valed sätted või sünkroonimiseks pole piisavalt õigusi.  

AADConnecti uuesti installimine kiirsätete abil võib probleemi kiiresti lahendada.

1. [Laadige alla AADConnecti uusim versioon.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Järgige kiirinstalli juhiseid.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect peab olema opsüsteemis Windows Server 2012 või uuemas versioonis installitud. See server peab olema domeeniga ühendatud ja võib olla domeenikontroller või liikmest server. Azure AD Ühendus eeltingimuste täieliku loendi vaatamiseks vaadake [läbi Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Ühendus.

Lisateavet AADConnecti teenusekontode kohta leiate teemast [Azure AD Ühendus: Kontod ja õigused](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
