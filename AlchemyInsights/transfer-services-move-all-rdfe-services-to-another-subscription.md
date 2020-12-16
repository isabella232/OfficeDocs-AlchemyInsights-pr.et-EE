---
title: Teenuste edastamine – kõigi RDFE teenuste teisaldamine teise tellimusse
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692041"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Teenuste edastamine – kõigi RDFE teenuste teisaldamine teise tellimusse

**Ressursside ümberpaigutamine**

Azure ' i ressursse saab teisaldada kas mõnele muule Azure ' i tellimusele või ressursirühma samale tellimusele, kasutades Azure ' i portaali, Azure PowerShelli, Azure ' i või REST API-d.

Enne ressursside liikumist vaadake järgmisi teemasid:

- [Kontroll-loend enne ressursside teisaldamist](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Teenused, mida saab teisaldada](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Liikumise kinnitamine](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Teenuste juhendamine](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Olemasolevate ressursside teise ressursirühma või tellimusele liikumiseks saate kasutada järgmist.

- [Azure ' i portaal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Õpetus: [Azure ' i ressursside teise ressursirühma või tellimusele minek](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Tõrkeotsing tõrgete korral Azure Resource Manageri abil**

Lisateavet levinud Azure ' i juurutamise tõrgete kohta leiate allpool olevatest artiklitest ja nende lahendamiseks saada teavet. Kui te ei leia oma juurutamise tõrke tõrkekoodi, lugege teemat [tõrkekoodi otsimine](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Juurutamise tõrgete tõrkeotsing](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure ' i ressursside uuele ressursirühma või tellimusele teisaldamise tõrkeotsing](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Pange tähele, et kui soovite oma Azure ' i tellimust täiendada (nt minna tasuta tasulisele tellimusele), peate tellimuse muutma.

- Tasuta prooviversiooni värskendamiseks lugege artiklit [tasuta prooviversiooni uuendamine või Microsoft Imagine Azure ' i tellimuse maksmine-AS-You-Mine](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Tasuliste kontode vahetamise kohta leiate lisateavet teemast [Azure ' i tasuliste pakettide muutmine teise pakkumise jaoks](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Azure ' i tellimuse lisamiseks või seostamiseks Azure Active Directory rentniku jaoks tehke järgmist.**

1. Logige sisse ja valige pakett, mida soovite [Azure ' i portaalis tellimuste lehel](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)kasutada.
2. Valige **Muuda kataloogi**.
3. Vaadake üle kõik kuvatud hoiatused ja seejärel valige **Muuda**.
4. Kataloogi muudetakse tellimuse jaoks ja teile kuvatakse edukas sõnum.
5. Kasutage *kataloogi* vahetaja, et minna uude kataloogi. See võib võtta kuni 10 minutit, et kõik kuvataks õigesti.

**Soovitatavad dokumendid**

- [Azure ' i tellimuse omandiõiguse üleandmine](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Ressursside uude ressursirühma või tellimusesse paigutamine](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Ressursside haldamine Azure ' i portaali abil](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
