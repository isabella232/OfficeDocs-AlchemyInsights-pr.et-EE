---
title: Teamsi halduskeskus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826375"
---
# <a name="teams-admin-center"></a><span data-ttu-id="04f28-102">Teamsi halduskeskus</span><span class="sxs-lookup"><span data-stu-id="04f28-102">Teams Admin Center</span></span>

<span data-ttu-id="04f28-103">Vaadake teavet Teamsi haldamise kohta [Teamsi halduskeskusega](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="04f28-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="04f28-104">Kui te ei pääse Teamsi halduskeskusele ligi, kontrollige järgnevat.</span><span class="sxs-lookup"><span data-stu-id="04f28-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="04f28-105">Veenduge, et oleksite lubanud õige [Office 365 IP-aadressid ja URL-id](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kõikidel perimeetriseadmetel (tulemüür jne) või tulemüüri reeglid teie kohalikus masinas.</span><span class="sxs-lookup"><span data-stu-id="04f28-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="04f28-106">Veenduge, et Teamsi halduskeskuse portaali juurdepääsuks kasutatav sisselogimisteave ühtiks [Microsoft 365 haldusportaalis](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) loetletud kasutajanimega.</span><span class="sxs-lookup"><span data-stu-id="04f28-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="04f28-107">Kui kasutajad ei ilmu Teamsi halduskeskuses, kontrollige järgnevat.</span><span class="sxs-lookup"><span data-stu-id="04f28-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="04f28-108">Kas olete kasutajad loonud või määranud itsentsid viimase 24 tunni jooksul?</span><span class="sxs-lookup"><span data-stu-id="04f28-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="04f28-109">Veenduge, et ootaksite vähemalt 24 tundi enne tugiteenusetaotluse avamist.</span><span class="sxs-lookup"><span data-stu-id="04f28-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="04f28-110">Veenduge, kas olete määranud sobivad litsentsid.</span><span class="sxs-lookup"><span data-stu-id="04f28-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="04f28-111">Kui teil on kohapealne Active Directory, veenduge, et kohaliku Active Directory väljal [ProxyAddresses oleva msRTCSIP-PrimaryUserAddressi](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) või SIP-aadressi väärtus on kordumatu ja vorming vastab **sip:** Kasutaja kasutajanimi [Microsoft 365 halduskeskusest](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="04f28-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="04f28-112">Kui kavatsete säilitada Skype'i ärirakenduse serveri juurutuse ning kasutajad on kodus kohapeal ja veebis, järgige Skype'i ärirakenduse serveri juhtpaneelil linki "Hübriidrakenduse loomine Teamsi ja Skype'i ärirakenduse **veebiväljaandega"** ja teisaldage kasutajad veebiväljaandes.</span><span class="sxs-lookup"><span data-stu-id="04f28-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
