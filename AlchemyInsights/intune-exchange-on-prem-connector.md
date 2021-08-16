---
title: Intune Exchange on-premise Connector
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013960"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange on-premise Connector

Lisateavet intune'i ja Exchange vahel konnektori häälestamise kohta leiate järgmistest dokumentidest.

[Intune'i asutusesisese Exchange konfiguratsiooni Microsoft Intune Azure'is](https://docs.microsoft.com/intune/exchange-connector-install)

**KKK:**

K. Kuvatakse tõrketeade "Exchange Konnektori versiooni ei toetata", kui proovite häälestada Exchange konnektorit. Mis võib olla põhjuseks?

A. Konto, mida kasutate, on litsentsitud sobival viisil – sellel peab olema aktiivne Intune'i litsents

Küsimus. Kas mitme konnektori Exchange?

A. Saate häälestada ainult ühe Exchange intune'i rentniku kohta ühe Exchange kohta. Konnektori saab installida ainult ühte serverisse mitme serveriga exchange'i organisatsioonis.

Samuti ei saa konnektorid konfigureerida nii Exchange kui ka Exchange Online rentniku jaoks.

K. Kas konnektor saab kasutada CAS-massiivi selle ühendamiseks Exchange?

V. CAS-massiivi määramine pole konnektori häälestuses toetatud konfiguratsioon. Määrata tuleks ainult üks server, mis peaks olema konnektori konfiguratsioonifailis raske kodeerida, mille leiate

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Otsige üles järgmine kirje ```<ExchangeWebServiceURL />``` ja asendage URL exchange'i serveriga.

**Näide:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Lisateavet leiate järgmisest dokumentatsioonist: [Intune'i asutusesisese](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) Exchange tõrkeotsing

**Verbose logimise lubamine Exchange konnektori jaoks**

1. Avage Exchange konnektori jälgimise konfiguratsioonifail.  
Faili asukoht on : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Näide:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Leidke traceSourceLine järgmise võtmega: OnPremisesExchangeConnectorService  
  
3. Muutke lähtetaseme sõlme väärtus väärtuseks Information ActivityTracing (vaikesäte) väärtuseks Verbose ActivityTracing (Tegevuse jälgimine)  

**Näide:**
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
4. Taaskäivitage Microsoft Intune Exchange teenus  
5. Täielik sünkroonimine Intune'i portaalis, kuni see lõpetatakse, ja seejärel muutke XML-iks "Teabetegevuse jälgimine" ja taaskäivitage Microsoft Intune Exchange teenus.  
6. Logide asukoht on: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`