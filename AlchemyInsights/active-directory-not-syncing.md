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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937097"
---
# <a name="active-directory-not-syncing"></a>Active Directoryt ei sünkroonita

Kui saate sünkroonimistõrkeid (nt "viimatist sünkroonimist pole" või märkate kataloogisünkroonimise olekut Office haldusportaalis, ütleb "Viimati sünkroonitud rohkem kui 3 päeva tagasi", võib olla see, et AADConnectil on valed sätted või sünkroonimiseks pole piisavalt õigusi.  

AADConnecti uuesti installimine kiirsätete abil võib probleemi kiiresti lahendada.

1. [Laadige alla AADConnecti uusim versioon.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Järgige kiirinstalli juhiseid.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect peab olema opsüsteemis Windows Server 2012 või uuemas versioonis installitud. See server peab olema domeeniga ühendatud ja võib olla domeenikontroller või liikmest server. Azure AD Ühendus eeltingimuste täieliku loendi vaatamiseks vaadake [läbi Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)Ühendus.

Lisateavet AADConnecti teenusekontode kohta leiate teemast [Azure AD Ühendus: Kontod ja õigused](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
