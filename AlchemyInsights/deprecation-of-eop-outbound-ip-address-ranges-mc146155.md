---
title: 1065 EOP taunimine väljaminev IP aadress rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858092"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="0eff1-102">Taunimine EOP väljaminev IP-aadressid</span><span class="sxs-lookup"><span data-stu-id="0eff1-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="0eff1-103">Tuvastatud võimalike probleemi teie organisatsiooniga (kui ei kõrvaldata 26. oktoobril 2018) võib murda meilivoogu kohapeal või välistesse sihtkohtadesse.</span><span class="sxs-lookup"><span data-stu-id="0eff1-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="0eff1-104">Kui varem edastatud IP aadress vahemikus haldamise lihtsustamiseks meil on konsolideerimine kasutatavad saata ja vastu võtta e-posti väljaspool Office 365 Exchange Online kaitse (EOP) IP-aadressid.</span><span class="sxs-lookup"><span data-stu-id="0eff1-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="0eff1-105">Meie analüüs näitab, et ühe või mitme välise e-posti puhul või sihtkohtade, mille olete konfigureerinud posti voolu ühendused ei ole vastu ühendusi on IP aadress vahemikud näidatud [siin](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0eff1-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="0eff1-106">Tegutsema enne 26 oktoober tagada nende allikad ja sihtkohtade aktsepteerib lennuühendusi kõik [avaldatud EOP IP-aadressid](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0eff1-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="0eff1-107">Selle muudatuse kohta lisateabe saamiseks lugege keskus Ametikohad, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)või [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="0eff1-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="0eff1-108">**Märkus**: kui varem kasutanud IP või URL kirjastamine, HTML, XML ja RSS värskendusi lõpp-punkti, samuti tuleks siirdamist uute veebiteenuste automatiseerimiseks seda tüüpi värskendusi.</span><span class="sxs-lookup"><span data-stu-id="0eff1-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="0eff1-109">Lisateabe saamiseks vt [Office 365 lõpp-punkti kategooriad ja Office 365 IP-aadress ja URL-i veebiteenuse](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="0eff1-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>