---
title: SpamHaus blokeeritud e-posti saatmise tõrge
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714254"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="c84ad-102">Tõrge meili saatmisel: kliendi hosti blokeeritud kasutades SpamHaus</span><span class="sxs-lookup"><span data-stu-id="c84ad-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="c84ad-103">Sõnumi saatnud IP-aadress on blokeeriloendis, mille omanik on [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="c84ad-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="c84ad-104">SpamHaus blokeeritavate põhjuste hulka kuuluvad ohustav konto, rikutud masinad, mis jagavad avalikku IP-aadressi ja Interneti-teenuse pakkuja (ISP) poliitikaid.</span><span class="sxs-lookup"><span data-stu-id="c84ad-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="c84ad-105">Võimalikud parandused on:</span><span class="sxs-lookup"><span data-stu-id="c84ad-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="c84ad-106">Blokeeritud sissetulevad sõnumid, kus te kontrolli allika meiliserverit, peate kindlaks tegema põhjuse ja eemaldama Block SpamHaus veebisaidilt.</span><span class="sxs-lookup"><span data-stu-id="c84ad-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="c84ad-107">Blokeeritud sissetulevate sõnumite puhul, kus allika IP-aadress kuulub kellelegi teisele, peab aadressi omanik eemaldama SpamHaus veebisaidilt ploki.</span><span class="sxs-lookup"><span data-stu-id="c84ad-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="c84ad-108">Kui IP-aadress on poliitika Block List (PBL), omanik saab määrata teise staatilise IP-aadressi või eemaldada aadress PBL.</span><span class="sxs-lookup"><span data-stu-id="c84ad-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="c84ad-109">Blokeeritud väljaminevate sõnumite domeenist, mis on ühendatud Microsofti, saate selle tõrke, kui sõnumid on marsruutitud kaudu 3rd Party teenust.</span><span class="sxs-lookup"><span data-stu-id="c84ad-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="c84ad-110">WHOIS otsinguriista abil saate leida blokeeritud IP-aadressi omanik.</span><span class="sxs-lookup"><span data-stu-id="c84ad-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
