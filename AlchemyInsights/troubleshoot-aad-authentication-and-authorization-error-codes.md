---
title: Azure AD Authenticationi ja autoriseerimise (AADSTS) tõrkekoodid tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035637"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="74abf-102">Azure AD Authenticationi ja autoriseerimise (AADSTS) tõrkekoodid tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="74abf-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="74abf-103">AAD autentimise ja autoriseerimise tõrkekoodid (AADSTS) lahendamiseks tehke järgmised Soovitatavad toimingud.</span><span class="sxs-lookup"><span data-stu-id="74abf-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="74abf-104">**Rakenduse tõrkekoodid käitlemine**</span><span class="sxs-lookup"><span data-stu-id="74abf-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="74abf-105">**OAuthi 2.0 spec**, annab juhiseid selle kohta, kuidas tõrke korral tõrkeid tõrkeid https://tools.ietf.org/html/rfc6749#section-5.2 kasutades autentida.</span><span class="sxs-lookup"><span data-stu-id="74abf-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="74abf-106">**tõrge**: tõrkekood string, mida saab kasutada ilmnevate tõrgete tüüpide klassifitseerimiseks, ning seda tuleks kasutada tõrgete korral reageerimiseks.</span><span class="sxs-lookup"><span data-stu-id="74abf-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="74abf-107">Väljal **viga** on mitu võimalikku väärtust – vaadake üle protokolli dokumentatsiooni lingid ja OAuthi 2,0 specs, et saada lisateavet konkreetsete tõrgete ja neile reageerimise kohta.</span><span class="sxs-lookup"><span data-stu-id="74abf-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="74abf-108">Siin on proovi tõrge vastus:</span><span class="sxs-lookup"><span data-stu-id="74abf-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="74abf-109">**Praeguse tõrke koodi teabe otsing**</span><span class="sxs-lookup"><span data-stu-id="74abf-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="74abf-110">Tõrkekoodid ja sõnumid võivad muutuda.</span><span class="sxs-lookup"><span data-stu-id="74abf-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="74abf-111">Uusimat teavet leiate https://login.microsoftonline.com/error lehelt AADSTS vigade kirjeldused, parandused ja Soovitatavad lahendused.</span><span class="sxs-lookup"><span data-stu-id="74abf-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="74abf-112">Samuti saate otsida ja sooritada artiklis [AZURE ad autentimine ja autoriseerimise](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)tõrkekoodid loetletud [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) .</span><span class="sxs-lookup"><span data-stu-id="74abf-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="74abf-113">**Abi saamine**</span><span class="sxs-lookup"><span data-stu-id="74abf-113">**Get Help**</span></span>

- <span data-ttu-id="74abf-114">[Arendajate tugi-ja tugikeskused](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – kui vajate vastust küsimusele või abi, mis lahendab probleemi, mida meie dokumentatsioon ei hõlma, võib olla aeg saada abi ekspertidele.</span><span class="sxs-lookup"><span data-stu-id="74abf-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="74abf-115">Selles artiklis on esitatud mitu soovitust, kuidas saada oma küsimustele vastuseid, kui arendate rakendusi, mis integreeritakse Microsoft Identity platformiga.</span><span class="sxs-lookup"><span data-stu-id="74abf-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








