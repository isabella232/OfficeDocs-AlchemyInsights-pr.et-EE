---
title: Transfer Services - Move all RDFE services to another subscription
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940034"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services - Move all RDFE services to another subscription

**Ressursside teisaldamine**

Azure'i ressursse saab ressursside teisaldamiseks azure'i portaali, Azure PowerShelli, Azure CLI või REST API abil teisaldada sama tellimuse alusel teise Azure'i tellimusse või ressursirühma.

Enne ressursside teisaldamist lugege teemat

- [Kontroll-loend enne ressursside teisaldamist](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Teenused, mida saab teisaldada](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Käigu valideerimine](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Teenuste juhiste teisaldamine](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Olemasolevate ressursside teisaldamiseks mõnda muusse ressursirühma või tellimusse saate kasutada:

- [Azure'i portaal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Õpetus: [Azure'i ressursside teisaldamine teise ressursirühma või tellimusse](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure Resource Manageri tõrgete tõrkeotsing**

Lisateavet levinud Azure'i juurutustõrgete kohta leiate allpool toodud artiklitest ja saate nende lahendamiseks teavet. Kui te ei leia juurutamisvea tõrkekoodi, lugege teemat [Tõrkekoodi otsige.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Juurutamistõrgete tõrkeotsing](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure'i ressursside uuele ressursirühmale või tellimusele teisaldamise tõrkeotsing](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Võtke arvesse, et kui soovite oma Azure'i tellimust täiendada (nt minna üle tasuta tellimuselt tasule), peate tellimuse teisendama.

- Tasuta prooviversiooni täiendamiseks lugege teemat [Tasuta prooviversiooni või Microsoft Imagine Azure'i tellimuse täiendamine teenuseks Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Vaadake teemat [Azure Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)tellimuse muutmine muuks pakkumiseks.

**Azure'i tellimuse lisamiseks või seostamiseks oma Azure Active Directory rentnikuga.**

1. Logige sisse ja valige Azure'i portaali lehel Tellimused soovitud [tellimus.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Valige **Muuda kataloogi**.
3. Vaadake kuvatavad hoiatused üle ja valige **Muuda**.
4. Tellimust muudetakse ja teile kuvatakse eduteade.
5. Uue *kataloogi* minemiseks kasutage kataloogilülitit. Kõige õigeks näitamine võib võtta kuni 10 minutit.

**Soovitatud dokumendid**

- [Azure'i tellimuse omandiõiguse üleminek](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Ressursside teisaldamine uude ressursirühma või tellimusse](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Ressursside haldamine Azure'i portaali abil](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
