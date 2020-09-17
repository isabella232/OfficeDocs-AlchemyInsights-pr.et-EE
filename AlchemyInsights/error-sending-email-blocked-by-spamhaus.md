---
title: Tõrge SpamHaus poolt blokeeritud meilisõnumite saatmisel
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783799"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="514c4-102">Tõrge meilisõnumi saatmisel: kliendi host on SpamHaus abil blokeeritud</span><span class="sxs-lookup"><span data-stu-id="514c4-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="514c4-103">Sõnumi saatnud IP-aadress on [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245)-i omanikule kuuluval ploki loendis.</span><span class="sxs-lookup"><span data-stu-id="514c4-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="514c4-104">Põhjused, miks SpamHaus on blokeeritud, hõlmavad ka ohustatud kontosid, avaliku IP-aadressi ühiskasutusse antud ohustatud seadmeid ja Interneti-teenuse pakkuja (ISP) poliitikaid.</span><span class="sxs-lookup"><span data-stu-id="514c4-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="514c4-105">Võimalikud parandused on järgmised.</span><span class="sxs-lookup"><span data-stu-id="514c4-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="514c4-106">Blokeeritud sissetulevatele sõnumitele, kus saate määrata allika meiliserveri, peate tuvastama põhjuse ja eemaldama ploki SpamHaus veebisaidilt.</span><span class="sxs-lookup"><span data-stu-id="514c4-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="514c4-107">Blokeeritud sissetulevatele sõnumitele, kus allika IP-aadress kuulub kellelegi teisele, peab aadressi omanik eemaldama ploki SpamHaus veebisaidilt.</span><span class="sxs-lookup"><span data-stu-id="514c4-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="514c4-108">Kui IP-aadress asub poliitikate blokeerimise loendis (PBL), saab omanik määrata teistsuguse staatilise IP-aadressi või eemaldada aadressi PBL.</span><span class="sxs-lookup"><span data-stu-id="514c4-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="514c4-109">Microsoftiga ühendatud domeeni blokeeritud Väljaminevatele sõnumitele saate selle tõrketeate, kui sõnumeid marsruuditakse kolmanda osapoole teenuse kaudu.</span><span class="sxs-lookup"><span data-stu-id="514c4-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="514c4-110">Saate kasutada WHOIS-otsingu tööriista, et leida blokeeritud IP-aadressi omanik.</span><span class="sxs-lookup"><span data-stu-id="514c4-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
