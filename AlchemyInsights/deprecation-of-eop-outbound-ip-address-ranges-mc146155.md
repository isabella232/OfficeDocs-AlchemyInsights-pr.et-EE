---
title: 1065 EOP väljamineva IP-aadressi rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806791"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="607e3-102">Väljamineva IP-aadresside vahemike EOP</span><span class="sxs-lookup"><span data-stu-id="607e3-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="607e3-103">Oleme tuvastanud teie asutusega võimaliku probleemi, mis (kui seda ei parandatud 26. oktoobril, 2018), võib katkestada meilivoo teie kohapealsetele või välistesse sihtkohtadesse.</span><span class="sxs-lookup"><span data-stu-id="607e3-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="607e3-104">Nagu varem edastatud, on IP-aadresside vahemiku haldamise lihtsustamiseks koondatud Exchange Online ' i Protection (EOP) IP-aadresside vahemikud, mida kasutatakse meilisõnumite saatmiseks ja vastuvõtmiseks väljaspool Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="607e3-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="607e3-105">Meie analüüs näitab, et ühe või mitme välise e-posti allikat või sihtkohta, mille olete konfigureerinud meilivoo konnektorid, ei aktsepteeri [siin](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)esitatud IP-aadresside vahemikke.</span><span class="sxs-lookup"><span data-stu-id="607e3-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="607e3-106">Toimige enne 26. oktoobril, et need allikad ja sihtkohad aktsepteerivad ühendusi kõigi [avaldatud EOP IP-aadressidega](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="607e3-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="607e3-107">Lisateavet selle muudatuse kohta leiate teemast sõnumikeskuse postitused [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)või [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="607e3-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="607e3-108">**Märkus**: kui olete varem kasutanud IP-või URL-i avaldamist HTML-, XML-i ja RSS-i lõpp-punktide värskenduste kaudu, peaksite ka migreerima uued veebiteenused, et automatiseerida seda tüüpi värskendusi.</span><span class="sxs-lookup"><span data-stu-id="607e3-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="607e3-109">Lisateavet leiate teemast [microsoft 365 lõpp-punkti kategooriad ja microsoft 365 IP-aadress ja URL-i veebiteenus](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="607e3-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
