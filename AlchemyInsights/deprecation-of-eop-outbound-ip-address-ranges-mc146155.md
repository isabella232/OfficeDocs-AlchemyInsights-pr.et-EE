---
title: 1065 EOP väljaminev IP-aadressi deprecation rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704593"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="ecc6b-102">EOP väljaminevate IP-aadresside vahemike keelamine</span><span class="sxs-lookup"><span data-stu-id="ecc6b-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="ecc6b-103">Oleme tuvastanud potentsiaalse probleemi teie organisatsioonis, et (kui ei korrigeerita oktoober 26th, 2018) võib murda meilivoog asutusesisese või väliste sihtkohtade.</span><span class="sxs-lookup"><span data-stu-id="ecc6b-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="ecc6b-104">Nagu varem edastatud, lihtsustada IP-aadresside vahemiku haldamine, me konsolideeritakse Exchange Online Protection (EOP) IP aadressi vahemikud, mida kasutatakse saata ja vastu võtta e-posti väljaspool Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ecc6b-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="ecc6b-105">Meie analüüs näitab, et üks või mitu välist e-posti allikad või sihtkohad, mis on konfigureeritud e-posti voog konnektorid ei aktsepteeri ühendusi [siin](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)näidatud IP-aadresside vahemikud.</span><span class="sxs-lookup"><span data-stu-id="ecc6b-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="ecc6b-106">Seaduse enne oktoober 26th tagada nende allikate ja sihtkohtade aktsepteerivad ühendusi ja kõik [avaldatud EOP IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="ecc6b-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="ecc6b-107">Selle muudatuse kohta lisateabe saamiseks lugege Message Center postitusi [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)või [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="ecc6b-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="ecc6b-108">**Märkus**: kui KASUTASITE varem IP või URL-i avaldamine HTML-i, XML-i ja RSS-i lõpp-punkti värskenduste jaoks, peaksite ka uude veebiteenusse seda tüüpi värskenduste automatiseerimiseks rändama.</span><span class="sxs-lookup"><span data-stu-id="ecc6b-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="ecc6b-109">Lisateabe saamiseks vaadake [microsoft 365 lõpp-punkti kategooriad ja microsoft 365 IP-aadress ja URL-i veebiteenus](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="ecc6b-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
