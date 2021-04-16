---
title: Rämpspostihausi blokeeritud meilisõnumite saatmisel ilmnes tõrge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813720"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="0b759-102">Meilisõnumite saatmisel ilmnes tõrge: Rämpspostihausi abil blokeeritud klientarvuti host</span><span class="sxs-lookup"><span data-stu-id="0b759-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="0b759-103">Sõnumi saatnud IP-aadress asub rämpspostisaatjale omases [blokeerimisloendis.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="0b759-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="0b759-104">Rämpspostihausi blokeerimise põhjused on näiteks ohustatud kontod, avaliku IP-aadressiga ohustatud masinad ja Interneti-teenuse pakkuja (ISP) poliitikad.</span><span class="sxs-lookup"><span data-stu-id="0b759-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="0b759-105">Võimalikud parandused on järgmised.</span><span class="sxs-lookup"><span data-stu-id="0b759-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="0b759-106">Blokeeritud sissetulevate sõnumite korral, kus saate lähtemeiliserverit juhtida, peate määrama põhjuse ja eemaldama blokeerimise Rämpspostikeskuse veebisaidilt.</span><span class="sxs-lookup"><span data-stu-id="0b759-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="0b759-107">Blokeeritud sissetulevate sõnumite korral, mille lähte-IP-aadress kuulub kellelegi teisele, peab aadressi omanik blokeerima Rämpspostihausi veebisaidilt.</span><span class="sxs-lookup"><span data-stu-id="0b759-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="0b759-108">Kui IP-aadress on poliitikaplokkide loendis (PBL), saab omanik määrata muu staatilise IP-aadressi või eemaldada aadressi PBL-ist.</span><span class="sxs-lookup"><span data-stu-id="0b759-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="0b759-109">Microsoftiga ühendatud blokeeritud väljaminevate sõnumite korral saate selle tõrketeate, kui sõnumid marsruuditakse kolmanda osapoole teenuse kaudu.</span><span class="sxs-lookup"><span data-stu-id="0b759-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="0b759-110">Blokeeritud IP-aadressi omaniku leidmiseks saate kasutada WHOIS-otsingutööriista.</span><span class="sxs-lookup"><span data-stu-id="0b759-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
