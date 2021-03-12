---
title: Koopia komplekt
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713747"
---
# <a name="replica-set"></a>Koopia komplekt

AADDS nimetatakse ka hallatavaks domeeniks. See on tegelikult kaks domeenikontrollerit, mida tagaserveris käitab ja hooldab. Kaks DCs sisaldavad ühte peamist DC-d ja ühte replikatsiooni DC-d. Varundid AADDS (hallatav Domeen) on Azure ' i platvormi hallatav automatiseeritud protsess. Kui probleem on teie hallatavas domeenis, aitab Azure ' i tugi teil taastada varukoopia põhjal.

Loote iga koopia virtuaalses võrgus. Iga virtuaalne võrk peab olema ühendatud kõigi muude virtuaalsete võrkudega, mis majutavad hallatava domeeni koopia komplekti. Selle konfiguratsiooniga luuakse võrgusilma võrgu topoloogia, mis toetab kataloogi replikatsiooni. Virtual Network saab toetada mitut koopia komplekti, kui iga koopia komplekt on mõnes muus virtuaalses alamvõrgus.

Lisateavet koopiakomplekti kohta leiate teemast [Concepts replica komplektid](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
