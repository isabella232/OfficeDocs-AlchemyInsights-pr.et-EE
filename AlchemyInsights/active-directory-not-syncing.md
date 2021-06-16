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
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930971"
---
# <a name="active-directory-not-syncing"></a>Active Directoryt ei sünkroonita

Kui saate sünkroonimistõrkeid (nt "viimatist sünkroonimist pole" või märkate kataloogisünkroonimise olekut Office haldusportaalis, ütleb "Viimati sünkroonitud rohkem kui 3 päeva tagasi", võib olla see, et AADConnectil on valed sätted või sünkroonimiseks pole piisavalt õigusi.  

AADConnecti uuesti installimine kiirsätete abil võib probleemi kiiresti lahendada.

1. [Laadige alla AADConnecti uusim versioon.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Järgige kiirinstalli juhiseid.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect peab olema opsüsteemis Windows Server 2012 või uuemas versioonis installitud. See server peab olema domeeniga ühendatud ja võib olla domeenikontroller või liikmest server. Azure AD Ühendus eeltingimuste täieliku loendi vaatamiseks vaadake [läbi Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Ühendus.

Lisateavet AADConnecti teenusekontode kohta leiate teemast [Azure AD Ühendus: Kontod ja õigused](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
