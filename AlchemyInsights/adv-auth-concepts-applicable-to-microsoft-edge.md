---
title: Microsoft Edge ' i suhtes kohaldatavad täiustatud autentimise põhimõtted
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573394"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="cb8a4-102">Microsoft Edge ' i suhtes kohaldatavad täiustatud autentimise põhimõtted</span><span class="sxs-lookup"><span data-stu-id="cb8a4-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="cb8a4-103">Järgmised on Microsoft Edge ' i jaoks kohaldatavad täiustatud autentimise kontseptsioonid.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="cb8a4-104">**Proaktiivne autentimine**</span><span class="sxs-lookup"><span data-stu-id="cb8a4-104">**Proactive Authentication**</span></span>

<span data-ttu-id="cb8a4-105">Kui lubate [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) poliitika, proovib Microsoft Edge autentida sisselogitud kasutajaid Microsofti teenuste kaudu.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="cb8a4-106">Regulaarsete ajavahemike järel kasutab ta veebiteenust, et kontrollida värskendatud manifesti, mis sisaldab ennetavat autentimist reguleerivat konfiguratsiooni.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="cb8a4-107">Eelised: proaktiivne autentimine võimaldab autentida põhiteenuseid (nt Office ' i uue vahekaardi leht).</span><span class="sxs-lookup"><span data-stu-id="cb8a4-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="cb8a4-108">Kui otsingumootorina kasutatakse ka Bingi, parandab proaktiivne autentimine aadressiriba jõudlust ja aitab luua teie ärirakenduse vajadustele vastavaid otsingutulemusi.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="cb8a4-109">**Windows Hello CredUI NTLM-autentimise jaoks**</span><span class="sxs-lookup"><span data-stu-id="cb8a4-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="cb8a4-110">Kui üksik sisselogimine (SSO) pole saadaval, kui veebisait proovib sisse logida kasutaja kaudu NTLM-või läbirääkimiste mehhanismi kaudu, võimaldab see funktsioon kasutajal jagada selle saidiga OS-i mandaati ja rahuldada autentimise väljakutse Windows Hello-i-süsteemi KASUTAJALIIDESE abil.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="cb8a4-111">See sisselogimine kuvatakse ainult opsüsteemis Windows 10 ja ainult nende kasutajate jaoks, kes ei saa kasutada SSO-või läbirääkimiste väljakutset.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="cb8a4-112">**Automaatselt sisselogimiseks salvestatud paroolide kasutamine**</span><span class="sxs-lookup"><span data-stu-id="cb8a4-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="cb8a4-113">Microsoft Edge ' is paroolid salvestavad kasutajad saavad lubada automaatse sisselogimise veebisaitidele, kus nad on salvestanud mandaadi.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="cb8a4-114">Kasutajad saavad selle funktsiooni edge://settings/passwords sisse või välja lülitada ja seda saab konfigureerida [parooli halduri](https://go.microsoft.com/fwlink/?linkid=2134622) poliitikas.</span><span class="sxs-lookup"><span data-stu-id="cb8a4-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
