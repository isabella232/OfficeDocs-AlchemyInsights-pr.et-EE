---
title: Kulude halduse lubamine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677219"
---
# <a name="enable-cost-management"></a>Kulude halduse lubamine

**Mida tähendab "kulud on teie ettevõtte jaoks keelatud"?**

Ettevõtted, kes kasutavad Enterprise Agreement (EA) või Microsoft Customer Agreement (MCA) kontosid, võivad keelata juurdepääsu kulude teabele ja hinnakujunduse teabele.

Pärast Azure ' i portaali sisselogimist saavad nad arveldamise API-sid kasutada programmiliselt arvete hankimiseks (kui olete valinud) ja kasutuse üksikasjad.

**Kuidas lubada täiendavate kasutajate juurdepääsu arvetele?**

1. Avage Azure ' i portaalis **tellimuste labad** .
2. Valige **arved** ja seejärel **juurdepääs arvetele**.
3. Juurdepääsu sisselülitamine, millele järgneb muudatuste salvestamine, et kasutajad saaksid arved alla laadida tellimuse ulatusega.

> [!NOTE]
> Konto administraator saab konfigureerida ka meili teel saadetud arved. Lisateavet leiate teemast [arve saamine meili teel](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Kasutajate lisamine arvelduse lugeja rollile**

1. Avage Azure ' i portaalis **tellimuste labad** .
2. Valige **Access Control (iam)** ja seejärel klõpsake nuppu **Lisa**.
3. Valige lehel **rolli valimine** valik **arvelduse lugeja** .
4. Tippige selle kasutaja meiliaadress, keda soovite kutsuda, ja seejärel klõpsake kutse saatmiseks nuppu **OK** .
5. Kui soovite logida sisse arvelduse lugejana, järgige juhiseid, mis on toodud teemas Kutsu meilisõnum. Lisateavet leiate teemast [Arveldusele juurdepääsu andmine](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Soovitatavad dokumendid**

- [Luba DA ja AO vaateid EA portaali kaudu](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kulude haldusse kaasatud kulud](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Toetatud Microsoft Azure ' i pakkumised](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Kulude ülevaade kulude analüüsis](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Juurdepääsu andmine arvelduse teabele](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Microsofti kliendi lepingule juurdepääsu kontrollimine](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






