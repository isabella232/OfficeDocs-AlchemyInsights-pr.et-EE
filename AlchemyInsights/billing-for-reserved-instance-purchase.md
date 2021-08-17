---
title: Broneeritud eksemplari ostude eest arve esitamine
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
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104016"
---
# <a name="billing-for-reserved-instance-purchase"></a>Broneeritud eksemplari ostude eest arve esitamine

Broneeritud eksemplari ostu eest esitatakse arve maksemeetodile, mis on seotud ostmise ajal valitud tellimusega. Tellimuse tüüp peab olema Enterprise Agreement (pakkumine nr MS-AZR-0017P), kasutuspõhine (pakkumine nr MS-AZR-0003P), Microsofti kliendileping või Microsofti pilvlahenduste pakkuja.

- Suurettevõtte tellimuse korral lahutatakse tasud registreerumise rahalise kohustuse saldolt või esitatakse arve ülejäägina
- Kasutuspõhise tellimuse korral esitatakse tasude eest arve tellimuse krediitkaardile või arve makseviisile.

**Reserveeringu tühistamine**

- **Iseteenindus:** Reserveeritud eksemplari saate azure'i portaali kaudu ise tühistada [või vahetada.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Valige broneering ja klõpsake tagasimakset või vahetust. Võtke arvesse, et teil peab olema omaniku juurdepääs broneerimiskorraldusele, et seda vahetada või tagasi maksta. Juurdepääs ainult broneeringule ei luba teil tagasimakset või vahetust jätkata. Paluge reserveerimistellimuse omanikul anda teile omanikule juurdepääs reserveerimiskorraldusele.
- **Exchange poliitika:** Saate vahetada reserveeringut mõne muu sama tüüpi reserveeringu vastu – broneeringu vahetamisel **ei ole** mingeid karistusi. Uue reserveeringuga kogukohustus peaks olema suurem kui vahetatud broneeringu tagasimakse summa ja tulevased igakuised maksed (kui see on asjakohane)
- **Tagasimaksepoliitika:** Tagasimaksesumma ja tühistatud tulevased maksed ei tohi ületada 50 000 USA dollarit 12-st kuust jooksvas aknas. Me ei **pea praegu tagasimaksete eest mingit** karistust, kuid võime selle tulevaste tagasimaksete eest tasuda.

**Erandid:** Iseteeninduslik vahetus ja tühistamisvõimalus pole SAADAVAL USA Enterprise Agreement klientidele

- **API / PS / CLI** tugi ei ole saadaval tühistamiseks ja tagasimaksete makstes Azure'i broneeringute iseteeninduse [vahetused ja tagasimaksed](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Iseteeninduslik vahetus ja tühistamisvõimalus pole SAADAVAL USA Enterprise Agreement klientidele. Toetatakse muid USA valitsuse tellimuse tüüpe, sh Pay-As-You-Go ja CSP

Lisateave: [Tagastus- ja vahetustehingute](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) töötlemine Lisateave: [Exchange ja tagasimaksepoliitikad](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Muud küsimused: Külasta [reserveeritud eksemplari dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange reserveeritud eksemplari (iseteenindus)**

Saate vahetada reserveeringut mõne muu sama tüüpi reserveeringu vastu. Kui te seda enam ei vaja, saate broneeringu tagasi maksta kuni 50 000 USA dollarit aastas. Iseteeninduslik vahetus ja tühistamisvõimalus pole SAADAVAL USA Enterprise Agreement klientidele. Toetatakse muid USA valitsuse tellimuse tüüpe, sh Pay-As-You-Go ja CSP. Olemasoleva broneeringu vahetamiseks või tagastamiseks peab teil olema omaniku juurdepääs broneerimiskorraldusele.

Tehingu lõpuleviimiseks tehke järgmist.

1.Logige sisse [Azure'i portaali.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Valige broneeringud, mille soovite tagasi maksta, ja **klõpsake Exchange** 2.Valige VM-toode, mida soovite osta, ja tippige kogus. Veenduge, et uue ostu kogusumma oleks suurem kui tagastussumma. Määrake enne [ostmist õige suurus.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Tehingu läbivaatamine ja lõpule viimine

**Reserveeritud eksemplari tagasimakse**

Broneeringu tagastamiseks minge valikusse Broneeringu üksikasjad **ja** klõpsake nuppu **Tagasimakse.**

**Pro tagasimakse:**

**Pro ja minimaalsete** nõuete näited raha tagastamise ja vahetamise kohta Ettetellimise näide:

- Ostate 1. jaanuaril 120-ga üheaastase tähtajaga RI
- 7. aprillil soovite selle broneeringu tagasi maksta või vahetada
- Kuna broneering on 97 päeva jooksul reaalajas olnud, saate (1-97/365) * 120 $ tagasi. (st 88,1 $ ). Tagasimaksete eest praegu karistust ei määrata
- Vahetamise korral peaks teie uus ost olema suurem kui 88,1 $
- Praegu tagasimaksete eest karistust ei määrata

**Arveldusplaani reserveerimise näide:**

- Ostate üheaastase tähtajaga RIT-d 10 $ kuus
- 7. aprillil soovite selle broneeringu tagasi maksta või vahetada
- Kuna viimane makse on tehtud 7 päeva, saate (1-7/31) * 10 $ tagasi. (st 7,74 $)
- Tühistatud tulevased maksed on 80 $. Tagasimaksete eest praegu karistust ei määrata
- Tühistamine lahutab teie 50 000 $ tagasimakselimiidist 87,74 $
- Vahetamise korral peaks uue ostu koguväärtus olema suurem kui 87,74 $

**Viimase arveldusperioodi arvet ei saa vaadata**

Mõned võimalikud põhjused, miks arvet ei pruugita kuvada.

- Teil on oma tellimusega igakuine krediidisumma, mida te ei ületanud või teil on tasuta prooviversioon. Arve luuakse ainult siis, kui olete raha võlgu
- Azure'i tellimise päevast on vähem kui 30 päeva.
- Arvet pole veel genereeritud. Oodake, kuni arveldusperioodi lõpuni
- Kui te pole kontoadministraator, ei pruugi vanemad arved teile saadaval olla.

**Arve allalaadimine Azure'i portaalist (.pdf)**

- Valige oma tellimus [Azure'i portaali lehel](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Tellimused, kui [kasutajal on juurdepääs arvetele.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Valige **Arved**
- **PDF-arve** koopia kuvamiseks klõpsake nuppu Laadi arve alla. Kui seal **on kirjas Pole** saadaval, lugege teemat Miks ma ei näe viimase [arveldusperioodi arvet?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Arve saatmine meilisõnumiga (.pdf)**

- Valige oma tellimus lehelt [Tellimused.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Klõpsake **valikut Arved ja** seejärel saatke arve meiliga
- Klõpsake **nuppu Loobu ja** nõustuge tingimustega. Teil tuleb valida iga tellimus, mille olete endale sidunud

Märkus. Kui te ei saa pärast juhiste järgimist meilisõnumit, veenduge, et teie meiliaadress on profiili [suhtluseelistustes õige.](https://account.windowsazure.com/profile)

**Kasutusandmete allalaadimine Azure'i portaalist**

- Logige [sisse Azure'i kontokeskusesse](https://account.windowsazure.com/Subscriptions) konto [administraatorina](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Valige tellimus, mille kohta soovite arve- ja kasutusteavet.
- Valige **Arveldamise ajalugu**
- Hinnangu **genereerimise ajal** kulude hinnangu kuvamiseks valige Kuva praegune lause.
- **Igapäevaste kasutusandmete** allalaadimiseks CSV-failina valige Laadi kasutus alla. Kui teile on saadaval kaks versiooni, laadige alla versioon 2

Muud küsimused: [külastage reserveeritud eksemplariga dokumente](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Soovitatud dokumendid**

- [Arvelduse põhitõed](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserveeritud eksemplari allahindluse rakendamist](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure'i arveldusarve ja igapäevaste kasutusandmete allalaadimine või vaatamiseks](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserveeritud eksemplari allahindluse rakendamist](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tellimuse Pay-As-You-Go reserveeritud eksemplarikasutuse mõistmine](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Enterprise'i registreerumise reserveeritud eksemplarikasutuse mõistmine](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows ei sisalda reserveeritud eksemplare](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserveeritud eksemplarid partneri Pilvlahenduste pakkuja (CSP) programmis](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)