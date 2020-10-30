---
title: Asutusesisese konnektori Intune ' i häälestamine
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807645"
---
# <a name="intune-exchange-on-premise-connector"></a>Asutusesisese konnektori Intune ' i häälestamine

Lisateavet kohapeal majutatud Intune ' i ja Exchange ' i vahelise konnektori häälestamise kohta leiate järgmistest dokumentidest.

[Microsoft Intune Azure ' i häälestamine asutusesisese Exchange ' i konnektori häälestamiseks](https://docs.microsoft.com/intune/exchange-connector-install)

**KKK**

K: Exchange Connectori häälestamise katsel kuvatakse tõrketeade "Exchange Connectori versiooni pole toetatud". Mis võiks olla põhjus?

V: konto, mida kasutate, on litsentsitud asjakohaselt – sellel peab olema aktiivne Intune ' i litsents.

K: Kas on võimalik kasutada mitut Exchange ' i konnektorit?

V: saate häälestada ühe Exchange ' i konnektori ühe Exchange ' i asutuse rentniku kohta. Konnektori saab installida ainult ühte serverisse mitme serveri Exchange ' i organisatsioonis.

Samuti ei saa teil olla ühendatud samasse rentniku jaoks konfigureeritud nii Exchange ' i kohapealsete kui ka Exchange Online ' i jaoks.

K: kas konnektor kasutab Exchange ' iga ühendust CAS-massiivina?

V: CAS-massiivi määramine pole konnektori häälestamisel toetatud konfiguratsioon. Ainult üks server tuleks määrata ja see peaks olema kõva konnektori konfiguratsioonifaili, mida võib leida

programmi data\microsoft\microsoft Intune for Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Otsige üles järgmine kirje ```<ExchangeWebServiceURL />``` ja asendage URL Exchange ' i serveriga.

**Nt**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Lisateavet leiate järgmistest dokumentidest: [asutusesisese Exchange Connectori Intune ' i tõrkeotsing](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Exchange Connectori verbose logimise lubamine**

1. Avage redigeerimise jaoks Exchange Connectori jälgimise konfiguratsioonifail.  
See toimik asub aadressil:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Nt**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Leidke TraceSourceLine, millel on järgmine võti: OnPremisesExchangeConnectorService  
  
3. SourceLevel muutmine ActivityTracing (vaikeväärtus) väärtuseks verbose ActivityTracing  

**Nt**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Microsoft Intune ' i Exchange ' i teenuse taaskäivitamine  
5. Täielik sünkroonimine Intune ' i portaalis, kuni see on lõpule jõudnud, ja seejärel muutke XML tagasi "teabe ActivityTracing" ja taaskäivitage Microsoft Intune Exchange ' i teenus.  
6. Logide asukoht: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`