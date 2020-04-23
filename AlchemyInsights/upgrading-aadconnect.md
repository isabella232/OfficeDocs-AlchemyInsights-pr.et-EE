---
title: 932 täiendamine AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766489"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD ühenduse täiendamine

Vaikimisi on automaatne täiendamine lubatud Azure AD ühenduse jaoks, mis aitab tagada uusima versiooni käitamise. Kontrollige automaatse versiooniuuenduse installimise sätted, kasutage Azure AD PowerShelli cmdlet **-käsu Get-ADSyncAutoUpgrade** . Cmdlet-käsk tagastab ühe järgmistest väärtustest:

- **Lubatud**: automaatne täiendamine on lubatud.

- **Keelatud**: automaatne täiendamine on keelatud.

- **Peatatud**: süsteem ei vasta enam automaatvärskendusteenuse saamise tingimustele. Seda väärtust ei saa konfigureerida; See on süsteemi poolt määratud.

Lisateabe saamiseks vaadake [automaatset täiendamist](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Azure AD ühenduse uusima versiooni allalaadimiseks [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
