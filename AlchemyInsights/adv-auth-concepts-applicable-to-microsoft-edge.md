---
title: Microsoft Edge'i täiustatud autentimispõhimõtted
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398554"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="51cf1-102">Microsoft Edge'i täiustatud autentimispõhimõtted</span><span class="sxs-lookup"><span data-stu-id="51cf1-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="51cf1-103">Microsoft Edge'ile kehtivad täpsemad autentimismõisted on järgmised.</span><span class="sxs-lookup"><span data-stu-id="51cf1-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="51cf1-104">**Ennetav autentimine**</span><span class="sxs-lookup"><span data-stu-id="51cf1-104">**Proactive Authentication**</span></span>

<span data-ttu-id="51cf1-105">Kui lubate [poliitika ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) proovib Microsoft Edge ennetavalt autentida sisse logitud kasutajaid Microsofti teenuste kaudu.</span><span class="sxs-lookup"><span data-stu-id="51cf1-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="51cf1-106">Regulaarsete intervallide järel kontrollib see veebiteenuse abil värskendatud manifesti, mis sisaldab proaktiivset autentimist reguleerivat konfiguratsiooni.</span><span class="sxs-lookup"><span data-stu-id="51cf1-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="51cf1-107">Eelised. Ennetav autentimine võimaldab autentimist võtmeteenustele (nt Office'i uue vahekaardi lehele).</span><span class="sxs-lookup"><span data-stu-id="51cf1-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="51cf1-108">Kui Bingi kasutatakse otsingumootorina, parandab proaktiivne autentimine aadressiriba jõudlust ja aitab luua teie ettevõtte vajadustele kohandatud otsingutulemeid.</span><span class="sxs-lookup"><span data-stu-id="51cf1-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="51cf1-109">**Windows Hello CredUI NTLM-autentimise jaoks**</span><span class="sxs-lookup"><span data-stu-id="51cf1-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="51cf1-110">Kui ühekordne sisselogimine (SSO) pole saadaval, kui veebisait proovib kasutajat NTLM-i või Negotiatei mehhanismi kaudu sisse logida, võimaldab see funktsioon kasutajal operatsioonisüsteemi identimisteavet veebisaidiga jagada ja windows Hello Credi kasutajaliidese abil autentimisfunktsiooni abil rahuldada.</span><span class="sxs-lookup"><span data-stu-id="51cf1-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="51cf1-111">See sisselogimisvoog kuvatakse ainult opsüsteemis Windows 10 ja ainult kasutajatele, kes ei saa SSO-d NTLM-i või Negotiatei väljakutse ajal.</span><span class="sxs-lookup"><span data-stu-id="51cf1-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="51cf1-112">**Salvestatud paroolide kasutamine automaatseks sisselogimiseks**</span><span class="sxs-lookup"><span data-stu-id="51cf1-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="51cf1-113">Microsoft Edge'is paroole salvestavad kasutajad saavad lubada automaatse sisselogimise veebisaitidele, kus nad on identimisteabe salvestanud.</span><span class="sxs-lookup"><span data-stu-id="51cf1-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="51cf1-114">Kasutajad saavad selle funktsiooni sisse või välja edge://settings/passwords ja saate selle konfigureerida [paroolihalduri poliitikates.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="51cf1-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
