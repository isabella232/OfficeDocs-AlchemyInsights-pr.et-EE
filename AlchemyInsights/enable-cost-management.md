---
title: Luba kuluhaldus
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
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003565"
---
# <a name="enable-cost-management"></a>Luba kuluhaldus

**Mida tähendab "kulud on teie asutuse jaoks keelatud"?**

Ettevõtted, Enterprise Agreement (EA) või Microsofti kliendilepingu (MCA) kontosid kasutavad asutused saavad keelata juurdepääsu kuluteabele ja hinnateabele.

Pärast Azure'i portaali sisselogimist saavad nad kasutada arvelduse API-sid, et saada programmiliselt arveid (kui see on valitud) ja kasutusteavet.

**Kuidas lubada lisakasutajatel arvetele juurde pääseda?**

1. Avage **Azure'i portaalis leht** Tellimused.
2. Valige **Arved** ja seejärel **Juurdepääs arvetele.**
3. Lülitage sisse juurdepääs, millele järgneb muudatuste salvestamine, et tellimuse ulatusega rollide kasutajad saavad arveid alla laadida.

> [!NOTE]
> Kontoadministraator saab konfigureerida ka nii, et arved saadetakse meiliga. Lisateavet leiate teemast [Arve toomine meilisõnumiga.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Kasutajate lisamine arvelduslugeja rolli**

1. Avage **Azure'i portaalis leht** Tellimused.
2. Valige **Accessi juhtelement (IAM) ja** seejärel klõpsake **nuppu Lisa.**
3. Valige **lehel Rolli** valimine valik **Arveldusluger.**
4. Tippige selle kasutaja meiliaadress, mille soovite kutsuda, ja klõpsake kutse saatmiseks nuppu **OK.**
5. Arvelduslugejana sisselogimiseks järgige kutse meilisõnumis toodud juhiseid. Lisateavet leiate teemast [Arvelduse juurdepääsu andmine.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**Soovitatud dokumendid**

- [DA- ja AO-vaadete lubamine EA portaali kaudu](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kuluhaldusse kaasatud kulud](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Toetatud Microsoft Azure'i pakkumised](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Kulude läbivaatamine kuluanalüüsis](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Arveldusteabele juurdepääsu tagab](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Microsofti kliendilepingule juurdepääsu kontrollimine](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






