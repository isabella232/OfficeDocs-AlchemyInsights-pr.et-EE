---
title: MDATP tõrkeotsing Mac-arvutis
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746299"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP tõrkeotsing Mac-arvutis

Kui käsitsi installimine nurjub, kuvatakse installiviisardi lehel **Kokkuvõte** järgmine tõrketeade:

"Installimisel ilmnes tõrge. Installeril ilmnes tõrge, mis põhjustas installi nurjumise. Abi saamiseks pöörduge tarkvara tootja poole. "

MDM-i juurutuste korral kuvatakse lehel üldine installi tõrge.

Kuigi me ei kuva lõppkasutajatele täpseid vigu, hoiame logifaili installimisega **/Library/Logs/Microsoft/mdatp/install.log**. Iga installimise seanss lisatakse sellele logifaili. Ainult viimase installimise seansi väljundiks kasutage `sed` .

Lisateavet leiate teemast [Microsoft DEFENDERI ATP for Maci installimisega seotud probleemide tõrkeotsing](https://go.microsoft.com/fwlink/?linkid=2144615).
