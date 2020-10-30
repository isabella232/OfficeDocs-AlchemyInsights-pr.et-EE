---
title: Miks on nupp Lisa eelarve minu jaoks keelatud?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807281"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Miks on nupp Lisa eelarve minu jaoks keelatud?

Eelarve loomiseks on vaja ühte järgmistest õigustest.

- Jaotis juhtimine, tellimus, ressursirühma ulatused
- Kulude halduse toetaja
- Omanik
- Kaasautor
- Ainult Enterprise ' i klient: registreerimine, osakond, konto ulatus
- Registreerimise administraator (eelarve seadmine liitumise ulatuses)
- Osakonna administraator (eelarve seadmine osakonna ulatuses)
- Konto omanik (eelarve seadmine konto ulatuses)
- Ainult tänapäevane kliendikonto: arvelduse konto, arvelduse profiil, arvete jaotise ulatus
- Azure ' i tellimuse looja

**Ma lõin eelarve, kui praeguse kuu hind oli juba eelarvest väljas. Miks ma ei saanud teatist?**  
Kui olete juba ületanud antud kulude künnise, kui loote eelarve, et teatis ei tule. Kui uus tsükkel algab, kui rikud künnist, siis teatis süttib.

**Millal peaks eeldama teatise kättesaamist pärast seda, kui olen ületanud ühe oma määratletud eelarveliste teatiste künnisest?**  
Eelarveid hinnatakse iga 4 tunni tagant. Andmete kasutamise kohta eelarvete süsteemile kulub vähemalt 8 tundi. Seda arvestades võivad teatised kesta kuni 12 tundi pärast künnise ületamist.

**Miks on nupp alguskuupäev kuu või arvelduse kuu lähtestamise perioodi valimisel keelatud?**  
Eelarved joondatakse praeguse kalendrikuu või praeguse arvelduse perioodiga (juhul, kui valitud on arveldamise kuu). Seetõttu peame selle väärtuse teie eest eelnevalt asustama.

**Miks ei kuvata eelarve loomise kogemustes minu kulude graafikut?**  
Meil on vaja vähemalt 2 kuud kulu andmeid, enne kui saame muuta graafikut, mis aitab teil eelarvet luua.

**Miks ei saa eelarvet määrata äsja loodud tellimuse vastu?**  
Pärast tellimuse loomist kulub andmete töötlemiseks 24-48 tundi enne eelarve määramist.

**Eelarve API ressursid**

- [Eelarvete API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): eelarvete loomiseks ja uuendamiseks pakutakse toiminguid. Eelarvete API abil saate määrata eelarve künnise ja konfigureerida mitu teatist, et seda künnist kasutada. Teatised võivad automatiseerimise sooritamiseks käivitada meili või Azure ' i tegevuste rühma. Märkus: selle API filtreerimine ei Joonda päringu API filtreerimise/dimensioonidega.
- [Eelarvete API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): eelarvete loomine suurema kulude filtreerimise võimalustega kui v1. Filtreerimine joondatakse meie päringus ja dimensioonide API-s kasutatava lepinguni. See on soovitatav eelarvete API kasutamiseks edasi liikuda.
- [Mõõtmed](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): pakub toiminguid, mille abil saate kasutada toetatud dimensioone teie kasutuseks mitmes ulatuses. Dimensioonide API abil saate hankida loendi dimensioonidest, mida saab kasutada päringu API päringute loomiseks sisendina.
- [Päring](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): pakub toiminguid, mille abil saate koondatud kulude ja kasutusandmed hankida teie tarnitava päringu põhjal. Päringu API abil saate määrata soovitud filtreerimise, sortimise ja rühmitamise kõigi saadaolevate dimensioonide jaoks (millele on juurdepääs dimensioonide API kaudu).

**Prognoositud kulud**

**Miks ei kuvata kulude analüüsi kulude prognoose?**  
On mitu põhjust, miks prognoositav projektsioon võib olla teie jaoks kulude analüüsis puudu, mõned neist on järgmised.

1. Kui teie kulude andmed on vähem kui 10 päeva vanad, siis ei laadita eelarveplaani. Mudel nõuab vähemalt 10 päeva viimaste kulude andmeid täpsete prognooside kohta.
2. Kui olete valinud ajaloolised kuupäevad, siis prognoositud diagramm pole nähtav. Valige kuupäevavahemik, kus on kuvatud eelarveplaani tulevased kuupäevad
3. Kui teie kontol on mitu valuutat, siis prognoositakse, et eelarvemudel hindab ainult "kõik kulud USA dollarites".

**Miks ei muutu prognoos minu ressursside muudatuste tegemisel?**  
Eelarvemudel nõuab konto muudatuste arvessevõtmiseks paari päeva jooksul ja ei tee kohe prognoose, võttes aluseks ressursside muutuse.  
Suuremate sammudena ressursside suurendamiseks või vähendamiseks võtab mudel veidi kauem aega nende muudatuste kohandamiseks kõrvalekallete arvessevõtmiseks.

**Miks prognoosimine pärast broneeringu või turuplatsi ostu sooritamist suureneb?**  
Eelarvemudel arvestab teie tegelike kuludega ning ei kasuta eraldi kasutus-ja ostu. Ühekordse ostuna vähendab mudel prognoose 10 päeva pärast, et arvestada kulude järsu tõusuga.

**Soovin vaadata ühe dimensiooni prognoose (nt. Arvesti**  
Prognoos toetab praegu kogukulude prognoose, mitte üksikute arvestite puhul. Seega, kui "rühmitatud" dimensiooni alusel, on prognoosid kõigi dimensiooni üksuste jaoks.

**Soovitatavad dokumendid**

- [Mis on Azure ' i kulude haldus?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure ' i kulude halduse head tavad](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kulude ja kulutuste analüüsimine](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kulude analüüsimisega seotud kulude uurimine ja analüüsimine](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure ' i kulude haldus: hinnakujundus](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kulude ülevaade kulude analüüsis](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video õpetus: Azure ' i portaalis eelarve loomine](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Eeltingimused eelarvete vaatamiseks ja kohandamiseks](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Eelarvete loomine ja haldamine](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatiseerimise konfigureerimine Azure ' i tegevuste rühmade ja eelarvete API-ga](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Kulude teatiste kasutamine kasutuse ja kulutuste jälgimiseks](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kulude halduse head tavad](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Õpetuse videod**

- [Eelarve loomine Azure ' i portaalis](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Kulude haldamine eelarvete API ja tegevuste rühmadega](https://go.microsoft.com/fwlink/?linkid=2147038)