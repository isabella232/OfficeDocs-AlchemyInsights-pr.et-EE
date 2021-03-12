---
title: Ei saa saata/vastu võtta meilisõnumeid teenusest Office 365 TLS 1,0 ja TLS 1,1 keelamise tõttu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743969"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="01099-102">Ei saa saata/vastu võtta meilisõnumeid teenusest Office 365 TLS 1,0 ja TLS 1,1 keelamise tõttu</span><span class="sxs-lookup"><span data-stu-id="01099-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="01099-103">Nagu kinnitas sõnumikeskuse postituse MC229914, TLS 1,0 ja TLS 1,1, hakkas jõustamine Exchange Online ' i meilivoo lõpp-punktide korral.</span><span class="sxs-lookup"><span data-stu-id="01099-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="01099-104">Varsti Office 365 ei nõustu enam TLS 1,0 ja TLS 1,1 väliste allikate kaudu.</span><span class="sxs-lookup"><span data-stu-id="01099-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="01099-105">Samuti ei kasuta Exchange Online kunagi TLS 1,0 või 1,1 Väljamineva meili saatmiseks.</span><span class="sxs-lookup"><span data-stu-id="01099-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="01099-106">Kui teil on probleeme TLS 1,0 või 1,1 keelamise tõttu, võib ilmneda üks järgmistest tõrketeadetest.</span><span class="sxs-lookup"><span data-stu-id="01099-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="01099-107">Saatja saab NDR-i tagasipõrkamise tagasi-' 421 4.4.2 Connection langes tõttu SocketError '</span><span class="sxs-lookup"><span data-stu-id="01099-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="01099-108">Tõrge asutusesisese serveri järjekorra vaaturis, mis saadab meilisõnumeid ametnikule 365-' 421 4.4.2 Connection langes SocketError tõttu</span><span class="sxs-lookup"><span data-stu-id="01099-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="01099-109">Tõrge rakenduses saada konnektor [protokolli logimine](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) serveris, mis saadab meilisõnumid Office 365-TLS-i läbirääkimistele nurjus tõrkega SocketError</span><span class="sxs-lookup"><span data-stu-id="01099-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="01099-110">Viga saatmisel või vastuvõtmisel konnektori protokolli log-"451 5.7.3 peab esmalt välja andma STARTTLS käsu"</span><span class="sxs-lookup"><span data-stu-id="01099-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="01099-111">Kui teil ilmneb mõni eespool kirjeldatud tõrgetest, veenduge, et meili saatmiseks või vastuvõtmiseks loodud serveris on TLS 1,2 lubatud, kontrollides järgmisi registrivõtmed.</span><span class="sxs-lookup"><span data-stu-id="01099-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="01099-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ klient] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="01099-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="01099-113">Kui muudate ülaltoodud registrivõtmed, et lubada TLS 1,2, taaskäivitage server muudatuste jõustumiseks.</span><span class="sxs-lookup"><span data-stu-id="01099-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="01099-114">Veenduge ka, et teil oleks installitud uusimad Windowsi ja Exchange ' i värskendused.</span><span class="sxs-lookup"><span data-stu-id="01099-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="01099-115">Lisateavet leiate järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="01099-115">For more information, see:</span></span>

- [<span data-ttu-id="01099-116">Exchange Serveri TLS-i juhised, osa 1: TLS 1,2-i ettevalmistamine – Microsoft Techi kogukond</span><span class="sxs-lookup"><span data-stu-id="01099-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="01099-117">Exchange Serveri TLS-i juhised osa 2: TLS 1,2 lubamine ja klientide tuvastamine, kes seda ei kasuta-Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="01099-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="01099-118">E-posti stsenaariumite mõistmine, kui TLS-versioone ei saa Exchange Online ' iga kokku leppida – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="01099-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
