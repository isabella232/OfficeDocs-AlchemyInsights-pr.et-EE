---
title: 932 versioonitäienduse Aadconnecti
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806035"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connecti värskendamine

Vaikimisi on Azure AD Connecti jaoks lubatud automaatne täiendamine, mis aitab tagada, et kasutate uusimat versiooni. Automaatse ülemineku sätete kinnitamiseks kasutage Azure AD PowerShelli cmdlet **-käsku Get-ADSyncAutoUpgrade** . Cmdlet-käsk tagastab ühe järgmistest väärtustest.

- **Lubatud**: automaatne uuendamine on lubatud.

- **Keelatud**: automaatne uuendamine on keelatud.

- **Peatatud**: süsteem ei vasta enam automaatsete versioonitäienduste saamise tingimustele. Seda väärtust ei saa konfigureerida; See on määratud süsteemis.

Lisateavet leiate teemast [Automaatne täiendus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Azure AD Connecti uusima versiooni allalaadimiseks avage [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
