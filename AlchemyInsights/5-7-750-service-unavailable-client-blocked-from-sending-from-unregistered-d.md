---
title: 1048 5.7.750 teenus pole saadaval. Kliendi blokeeritud saatmine registreerimata domeenid
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 06be6babc524ae0d8065355218426c695f49be66
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856616"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="106a2-103">5.7.750 kliendi blokeeritud saatmine registreerimata Domeen</span><span class="sxs-lookup"><span data-stu-id="106a2-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="106a2-104">Viga tekib siis, kui suurel hulgal sõnumeid saadetakse valdkondades, mis ei ole ette nähtud Office 365 (on aktsepteeritud domeenidena ja kinnitatud).</span><span class="sxs-lookup"><span data-stu-id="106a2-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>

<span data-ttu-id="106a2-105">Selle tõrke vältimiseks kasutage serdipõhist posti voolu konnektori kui sertifikaadi domeen on ettevalmistatud domeeni või valmistate saatva domeenides.</span><span class="sxs-lookup"><span data-stu-id="106a2-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>