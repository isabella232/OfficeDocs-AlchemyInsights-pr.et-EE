---
title: Täiustatud jahipidamispäringute heade tavade kasutamine
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930129"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Täiustatud jahipidamispäringute heade tavade kasutamine

Tulemuste kiiremaks saamiseks ja keerukate päringute ajal ajalõpu vältimiseks tehke järgmist.

- Uute päringute proovimisel kasutage alati limiiti, et vältida äärmiselt suurte tulemikomplektide saamist. Samuti saate `count` kasutada tulemikomplekti suuruse esialgseks hindamiseks.
- Kasutage esmalt ajafiltreid. Ideaaljuhul saate päringuid piirata seitsme päevaga.
- Lisage päringu alguses kohe pärast ajafiltrit filtrid, mis eeldavad enamiku andmete kustutamist.
- Täielike märkide otsimisel kasutage pigem `has` tehtemärki kui `contains` .
- Käivitage otsing kindlas veerus, mitte kõigis veergudes.
- Tabelite ühendamisel määrake esmalt tabel, kus on vähem ridu.
- `project` ainult ühendatud tabelite vajalikud veerud.

Lisateavet leiate teemast Täpsemad [jahipäringute head tavad.](https://go.microsoft.com/fwlink/?linkid=2144812)
