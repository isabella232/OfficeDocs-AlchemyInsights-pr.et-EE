---
title: Miks on nupp Lisa eelarve minu jaoks keelatud?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954662"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Miks on nupp Lisa eelarve minu jaoks keelatud?

Eelarve loomiseks on vaja ühte järgmistest õigustest.

- Haldusrühm, tellimus, ressursirühma ulatused
- Kulude halduse kaasautor
- Omanik
- Kaasautor
- Ainult enterprise customer: Enrollment, Department, Account Scopes
- Registreerumise administraator (eelarve määramine registreerimise ulatuse juures)
- Osakonna administraator (eelarve määramine osakonna ulatuses)
- Konto omanik (määra eelarve konto ulatuse järgi)
- Ainult modernne kliendileping: arvelduskonto, arveldusprofiil, arvejao ulatus
- Azure'i tellimuse looja

**Lõin eelarve, kui minu praeguse kuu maksumus oli juba üleeelarve. Miks ma teatist ei saanud?**  
Kui olete juba ületanud määratud kululäve, kui loote eelarve, mis ei tule. Kui algab uus tsükkel, kui ületate läve, siis hoiatusteade käivitatakse.

**Millal peaks eeldama teatise saamist pärast seda, kui olen ületanud ühe määratud eelarveteatise läve?**  
Eelarveid hinnatakse iga 4 tunni järel. Eelarvesüsteemini jõudmiseks kulub kasutusandmete jaoks vähemalt 8 tundi. Seda arvesse võttes võib hoiatuste arv pärast läve ületamist võtta kuni 12 tundi.

**Miks on nupp Alguskuupäev keelatud, kui valin kuu või arvelduskuu lähtestamisperioodi?**  
Eelarved joondatud praeguse kalendrikuu või praeguse arveldusperioodiga (juhul, kui valitud on arvelduskuu). Seetõttu eelasustame selle väärtuse teie eest.

**Miks ma ei näe eelarve loomises kulude graafikut?**  
Vajame minimaalselt 2 kuud kuluandmeid, enne kui saame renderdada graafiku, mis aitab teil eelarvet luua.

**Miks ei saa äsja loodud tellimusele eelarvet määrata?**  
Pärast tellimuse loomist kulub andmete töötlemiseks 24–48 tundi, enne kui eelarve selle vastu seatakse.

**Eelarve API ressursid**

- [Eelarved API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)pakub toiminguid eelarvete loomiseks ja värskendamiseks. Eelarvete API abil saate määrata eelarveläve ja konfigureerida mitu hoiatusteadet tulele, kui lähenete sellele lävele. Teatised võivad automatiseerimiseks käivitada meili või Azure'i toimingurühma. Märkus. Selle API filtreerimine ei ühti päringu API filtreerimise /mõõtmetega.
- [Eelarved API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)saate luua eelarveid, mille kulude filtreerimise võimalused on suuremad kui v1. Filtreerimine joondatud lepingule, mida kasutatakse meie päringu- ja dimensiooni api-des. See on soovitatav eelarvete API edasi liikumiseks.
- [Mõõtmed.](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Pakub toiminguid, mille kaudu saate oma kasutuse jaoks toetatud mõõtmeid kasutada mitmesugustes ulatuses. Dimensioonide API abil saate tuua dimensioonide loendi, mida saab päringu API-ga päringute loomiseks kasutada sisendina.
- [Päring.](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Pakub toiminguid, mille abil saate kogukulu- ja kasutusandmeid teie esitatud päringu põhjal. Päringu API abil saate määrata soovitud filtreerimise, sortimise ja rühmitamise kõigi saadaolevate dimensioonide alusel (millele pääseb juurde dimensioonide API kaudu).

**Prognoositud kulud**

**Miks ei näe kulude prognoosid kuluanalüüsis?**  
On mitu põhjust, miks prognoosi projektsioon võib teie jaoks kuluanalüüsis puududa, mõned neist on järgmised.

1. Kui teie kuluandmed on vähem kui 10 päeva vanad, siis prognoosidiagrammi ei laadita. Täpsete prognooside jaoks on mudeli jaoks vaja vähemalt 10 päeva hiljutisi kuluandmeid.
2. Kui olete valinud ajaloolised kuupäevad, siis prognoosidiagramm ei ole nähtav. Valige prognoosiskeemi kuvamiseks kuupäevavahemik koos tulevaste kuupäevadega.
3. Kui teie kontol on mitu valuutat, on prognoosidiagrammil ainult projektikulud "Kõik kulud USA dollarites".

**Miks ei muutu prognoos ressursside muutmisel?**  
Prognoosimudel nõuab konto muudatuste arvesse miseks paar päeva ega tee ressursside muutumisel põhinevaid kohesi prognoose.  
Ressursside suurendamise või vähendamise suuremate etappide korral võtab mudel nende muudatustega kohandamiseks anomaaliate arvesse suurendamiseks veidi rohkem aega.

**Miks kasvab minu prognoos pärast reserveeringu tegemist või Turuplatsi ostmist?**  
Prognoosimudelis võetakse arvesse teie tegelikku maksumust ning see ei arvesta kasutamist ega ostmist eraldi. Ühe ostu korral vähendab mudel prognooside arvu 10 päeva pärast, et võtta arvesse kulude järsku suurenemist.

**Soovin näha ühe dimensiooni prognoose (nt. Arvesti)**  
Prognoos toetab praegu kulude prognooside kogusummat, mitte üksikute arvestite puhul. Seega, kui dimensioon on rühmitatud, on prognoosid dimensiooni kõigi üksuste koguarvu kohta.

**Soovitatud dokumendid**

- [Mis on Azure'i kulude haldus?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure'i kulude halduse head tavad](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kulude ja kulutuste analüüsimine](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kulude analüüsimine ja analüüsimine](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure'i kulude haldus: hinnad](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kulude läbivaatamine kuluanalüüsis](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videoõpetus: Eelarve loomine Azure'i portaalis](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Eelarvete vaatamise ja kohandamise eeltingimused](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Eelarvete loomine ja haldamine](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatiseerimise konfigureerimine Azure'i tegevusrühmade ja eelarvete API abil](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Kuluteadete kasutamine kasutuse ja kulutuste jälgimiseks](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kuluhalduse head tavad](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Õppevideod**

- [Azure'i portaalis eelarve loomine](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Kulude haldamine eelarvete API ja tegevusrühmade abil](https://go.microsoft.com/fwlink/?linkid=2147038)