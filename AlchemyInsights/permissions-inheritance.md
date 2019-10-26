---
title: Õiguste pärimine
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 6322ca12902be2612f65b6388a650300b257a95e
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36554941"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="ed7cb-102">Kuidas õiguste pärand töötab SharePoint</span><span class="sxs-lookup"><span data-stu-id="ed7cb-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="ed7cb-103">Vaikimisi on SharePointi õigused päritud hierarhias kõrgemale.</span><span class="sxs-lookup"><span data-stu-id="ed7cb-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="ed7cb-104">Seega päriab fail oma õigused kaustast, mis päriab oma load teegist, mis päriab oma õigused saidilt, mis päriab oma õigused saidikogumis.</span><span class="sxs-lookup"><span data-stu-id="ed7cb-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="ed7cb-105">Teavet kordumatute õiguste eemaldamise ja päranduse taastamise kohta vaadake teemast [loendi või teegi õiguste redigeerimine ja haldamine](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="ed7cb-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

