---
title: Port Google Chrome ' i laiendused Microsoft Edge ' i (kroom)
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
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677286"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="5b80d-102">Port Google Chrome ' i laiendused Microsoft Edge ' i (kroom)</span><span class="sxs-lookup"><span data-stu-id="5b80d-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="5b80d-103">Google Chrome ' i [laiendusi saab hõlpsalt saata Microsoft Edge ' i (kroom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="5b80d-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="5b80d-104">Enamikul juhtudel on nende laiendite Microsoft Edge ' i käitamiseks vaja teha ainult minimaalseid muudatusi.</span><span class="sxs-lookup"><span data-stu-id="5b80d-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="5b80d-105">Google Chrome ' i toetatud laiendiga API-d ja manifesti võtmed on ühilduvad Microsoft Edge ' i koodiga.</span><span class="sxs-lookup"><span data-stu-id="5b80d-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="5b80d-106">Microsoft Edge ei toeta siiski laiendi APIs Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken ja Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="5b80d-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>