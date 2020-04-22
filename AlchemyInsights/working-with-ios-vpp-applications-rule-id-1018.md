---
title: Töötamine iOS VPP rakendused reegel ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719953"
---
# <a name="working-with-ios-vpp-applications"></a>Töötamine iOS VPP rakendused

Lugege, [Kuidas hallata iOS-i rakendusi, mis on ostetud Microsoft Intune ' i hulgitost-programmi kaudu](https://docs.microsoft.com/intune/vpp-apps-ios) , et saada teavet funktsioonide, piirangute ja toimingute kohta, et kasutada Apple ' i helitugevuse ostuprogrammi ja seda Microsofti Intune-i toe kaudu.
  
 **Levinud probleemid:** "Ma määratud iOS VPP rakendus minu kasutajatele, kuid paigaldamine nurjus."
  
- See võib juhtuda, kui ühe VPP luba kasutatakse mitme mobiilsideseadme haldusteenuse pakkujad. Apple ' i VPP märke võib kasutada ainult koos ühe pakkujaga. Kui kasutasite VPP luba mitme pakkujad, peate uuesti üles laadida luba Intune.

- Installimine võib nurjuda ka siis, kui seadmete koguarv ületab litsentside arvu. Litsentside kasutusaruande vaatamiseks jaotisse **Intune Mobile ' i rakenduste** \> **rakenduse litsentsid** leht. Lisateavet kasutuslitsentside kasutamise kohta leiate [käesolevast artiklist.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
