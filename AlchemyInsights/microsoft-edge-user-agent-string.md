---
title: Microsoft Edge ' i kasutajaagendi string (töölaud)
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
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677376"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="4ff61-102">Microsoft Edge ' i kasutajaagendi string (töölaud)</span><span class="sxs-lookup"><span data-stu-id="4ff61-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="4ff61-103">Kasutajaagendi (UA) stringe saab kasutada selleks, et tuvastada, millist kindlat brauseri versiooni kasutatakse teatud operatsioonisüsteemis.</span><span class="sxs-lookup"><span data-stu-id="4ff61-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="4ff61-104">Sarnaselt muude brauseritega lisab Microsoft Edge selle teabe ka "kasutajaagendi" HTTP päisesse iga kord, kui see saidilt taotluse esitab.</span><span class="sxs-lookup"><span data-stu-id="4ff61-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="4ff61-105">Brauseri versiooni teavet saab kasutada ka JavaScripti kaudu, kui päring "Navigator. User Agent" väärtus.</span><span class="sxs-lookup"><span data-stu-id="4ff61-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="4ff61-106">Soovitame, et veebiarendajad kasutaksid võimaluse korral funktsiooni tuvastamist, et parandada koodi säilitamist, vähendada koodi ebakindlust ja välistada koodi purunemise riski tulevaste UA stringi värskenduste korral.</span><span class="sxs-lookup"><span data-stu-id="4ff61-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="4ff61-107">Lisateavet leiate artiklist [Microsoft Edge User Agent String (töölaud)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="4ff61-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>