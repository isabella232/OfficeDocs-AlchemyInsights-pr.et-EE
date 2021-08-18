---
title: MDATP installiprobleemide tõrkeotsing Mac-arvutis
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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090997"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP installiprobleemide tõrkeotsing Mac-arvutis

Kui käsitsi installimine **nurjub,** kuvatakse installiviisardi lehel Kokkuvõte järgmine tõrketeade.

"Installimisel ilmnes tõrge. Installeril ilmnes tõrge, mis põhjustas installi nurjumise. Abi saamiseks pöörduge tarkvara tootja poole."

MDM-i juurutuste korral kuvatakse lehel ka üldine installitõrge.

Kuigi me ei kuva lõppkasutajatele täpseid tõrkeid, säilitame installi edenemisega logifaili , mis on saadaval rakenduses **/Library/Logs/Microsoft/mdatp/install.log.** Iga installiseanss lisatakse sellele logifailile. Ainult viimase installiseansi väljundiks kasutage funktsiooni `sed` .

Lisateavet leiate teemast [Microsoft Defenderi ATP for Maci installiprobleemide tõrkeotsing.](https://go.microsoft.com/fwlink/?linkid=2144615)
