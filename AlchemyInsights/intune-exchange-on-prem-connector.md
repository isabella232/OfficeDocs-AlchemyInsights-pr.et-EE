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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="c7edc-102">Asutusesisese konnektori Intune ' i häälestamine</span><span class="sxs-lookup"><span data-stu-id="c7edc-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="c7edc-103">Lisateavet kohapeal majutatud Intune ' i ja Exchange ' i vahelise konnektori häälestamise kohta leiate järgmistest dokumentidest.</span><span class="sxs-lookup"><span data-stu-id="c7edc-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="c7edc-104">Microsoft Intune Azure ' i häälestamine asutusesisese Exchange ' i konnektori häälestamiseks</span><span class="sxs-lookup"><span data-stu-id="c7edc-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="c7edc-105">**KKK**</span><span class="sxs-lookup"><span data-stu-id="c7edc-105">**FAQ:**</span></span>

<span data-ttu-id="c7edc-106">K: Exchange Connectori häälestamise katsel kuvatakse tõrketeade "Exchange Connectori versiooni pole toetatud".</span><span class="sxs-lookup"><span data-stu-id="c7edc-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="c7edc-107">Mis võiks olla põhjus?</span><span class="sxs-lookup"><span data-stu-id="c7edc-107">What could be the cause?</span></span>

<span data-ttu-id="c7edc-108">V: konto, mida kasutate, on litsentsitud asjakohaselt – sellel peab olema aktiivne Intune ' i litsents.</span><span class="sxs-lookup"><span data-stu-id="c7edc-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="c7edc-109">K: Kas on võimalik kasutada mitut Exchange ' i konnektorit?</span><span class="sxs-lookup"><span data-stu-id="c7edc-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="c7edc-110">V: saate häälestada ühe Exchange ' i konnektori ühe Exchange ' i asutuse rentniku kohta.</span><span class="sxs-lookup"><span data-stu-id="c7edc-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="c7edc-111">Konnektori saab installida ainult ühte serverisse mitme serveri Exchange ' i organisatsioonis.</span><span class="sxs-lookup"><span data-stu-id="c7edc-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="c7edc-112">Samuti ei saa teil olla ühendatud samasse rentniku jaoks konfigureeritud nii Exchange ' i kohapealsete kui ka Exchange Online ' i jaoks.</span><span class="sxs-lookup"><span data-stu-id="c7edc-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="c7edc-113">K: kas konnektor kasutab Exchange ' iga ühendust CAS-massiivina?</span><span class="sxs-lookup"><span data-stu-id="c7edc-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="c7edc-114">V: CAS-massiivi määramine pole konnektori häälestamisel toetatud konfiguratsioon.</span><span class="sxs-lookup"><span data-stu-id="c7edc-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="c7edc-115">Ainult üks server tuleks määrata ja see peaks olema kõva konnektori konfiguratsioonifaili, mida võib leida</span><span class="sxs-lookup"><span data-stu-id="c7edc-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="c7edc-116">programmi data\microsoft\microsoft Intune for Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="c7edc-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="c7edc-117">Otsige üles järgmine kirje ```<ExchangeWebServiceURL />``` ja asendage URL Exchange ' i serveriga.</span><span class="sxs-lookup"><span data-stu-id="c7edc-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="c7edc-118">**Nt**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="c7edc-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="c7edc-119">Lisateavet leiate järgmistest dokumentidest: [asutusesisese Exchange Connectori Intune ' i tõrkeotsing](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="c7edc-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="c7edc-120">**Exchange Connectori verbose logimise lubamine**</span><span class="sxs-lookup"><span data-stu-id="c7edc-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="c7edc-121">Avage redigeerimise jaoks Exchange Connectori jälgimise konfiguratsioonifail.</span><span class="sxs-lookup"><span data-stu-id="c7edc-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="c7edc-122">See toimik asub aadressil:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="c7edc-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="c7edc-123">**Nt**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="c7edc-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="c7edc-124">Leidke TraceSourceLine, millel on järgmine võti: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="c7edc-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="c7edc-125">SourceLevel muutmine ActivityTracing (vaikeväärtus) väärtuseks verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="c7edc-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="c7edc-126">**Nt**</span><span class="sxs-lookup"><span data-stu-id="c7edc-126">**Example:**</span></span>
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
4. <span data-ttu-id="c7edc-127">Microsoft Intune ' i Exchange ' i teenuse taaskäivitamine</span><span class="sxs-lookup"><span data-stu-id="c7edc-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="c7edc-128">Täielik sünkroonimine Intune ' i portaalis, kuni see on lõpule jõudnud, ja seejärel muutke XML tagasi "teabe ActivityTracing" ja taaskäivitage Microsoft Intune Exchange ' i teenus.</span><span class="sxs-lookup"><span data-stu-id="c7edc-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="c7edc-129">Logide asukoht: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="c7edc-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>