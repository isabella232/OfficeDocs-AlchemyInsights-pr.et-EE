---
title: Privileged Identity Management roll
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973225"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) roll

**Õigusi ei anta pärast rolli aktiveerimist**

Azure AD Privileged Identity Management (PIM) rolli aktiveerimisel ei pruugi aktiveerimine kohe levida kõigile portaalidele, mis nõuavad õigustega rolli. Mõnikord võib veebi vahemällu salvestamine portaalis isegi juhul, kui muudatust levitatakse, kohe muutuda.

Kui aktiveerimine viibib, tehke järgmist.

1. Logige Azure'i portaalist välja ja seejärel logige uuesti sisse. Azure AD-rolli või Azure'i ressursirolli aktiveerimisel kuvatakse aktiveerimise etapid. Kui kõik etapid on lõpule jõudnud, kuvatakse link "Logi välja". Selle lingi abil saate välja logida. See lahendab enamikel juhtudel aktiveerimise viivituse.
2. Veenduge, et olete PIM-i loendis rolli liige.
3. Kui aktiveerite administraatorirolli Exchange, logige kindlasti välja ja logige uuesti sisse. Kui probleem ei lahene, avage tugiteenuste pilet ja tõstke see probleemina esile. Kui kasutate turbe- ja Exchange turbe- ja vastavuskeskusele juurdepääsuks oma administraatorirolli, lugege järgmist juhist.
4. Kui aktiveerite turbe- ja vastavuskeskusele juurdepääsuks rolli või aktiveerite SharePoint administraatori rolli, ilmneb aktiveerimisviivitus mõne minuti kuni mõne tunni pärast. See on teadaolev probleem ja töötame aktiivselt nende töörühmadega, et see probleem võimalikult kiiresti lahendada.

Lisateavet leiate järgmistest teemadest.

- [Azure AD rollide aktiveerimine PIM-is](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Azure'i ressursirollide aktiveerimine PIM-is](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Õigusi ei eemaldata pärast rolli inaktiveerimist või rolli aktiveerimine aegub**

Kui inaktiveerite rolli Azure AD-Privileged Identity Management või kui rolli aktiveerimisperiood aegub, võib juurdepääsu jätkumisel olla viivitus.

Kui inaktiveerimine viibib, tehke järgmist.

1. Kui inaktiveerite Exchange administraatori rolli või rolli aktiveerimise periood aegub ja märkate enne õiguste eemaldamist märkimisväärset viivitust, avage tugiteenuste pilet ja teavitage oma tugiteenuste tehnikut, et aidata teil selle probleemi kohta esitada pilet Office-sse privilegeeritud juurdepääsuhalduse (PAM) töörühma.
2. Kui aktiveerimisperiood on aegunud, kuid brauseri seanss on endiselt avatud, sulgege brauser. Saate seda rolli edasi kasutada, kuni selle seansi sulgete. See on teadaolev probleem ja me otsime võimalikku parandust iga seansi aktiivseks tühistamiseks, kui aktiveerimine on aegunud.

Kui teie viivitus erineb nendest kahest stsenaariumist, avage tugiteenuste pilet.
