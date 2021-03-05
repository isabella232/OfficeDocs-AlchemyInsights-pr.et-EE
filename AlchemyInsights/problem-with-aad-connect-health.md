---
title: Probleem AAD Connecti tervisega
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481465"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="fe690-102">Probleem AAD Connecti tervisega</span><span class="sxs-lookup"><span data-stu-id="fe690-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="fe690-103">Veenduge, et teil on toimingu tegemiseks õigus.</span><span class="sxs-lookup"><span data-stu-id="fe690-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="fe690-104">Globaalsetel administraatoritel on vaikimisi juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="fe690-104">Global Admins have access by default.</span></span> <span data-ttu-id="fe690-105">Lisaks saate kasutada [rolli baasil juurdepääsu juhtelementi](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , et anda delegaadile registreerimise õigused.</span><span class="sxs-lookup"><span data-stu-id="fe690-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="fe690-106">Veenduge, et nõutavad lõpp-punktid on lubatud ja tulemüüri tõttu blokeeritud.</span><span class="sxs-lookup"><span data-stu-id="fe690-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="fe690-107">Lisateavet leiate teemast [nõuded](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="fe690-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="fe690-108">Registreerimine võib nurjuda tänu sellele, et võrgu kiht teostab väljaminevat suhtlust SSL-i kaudu.</span><span class="sxs-lookup"><span data-stu-id="fe690-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="fe690-109">Veenduge, et olete Azure AD Connecti tervise teatiste sätteid kinnitanud.</span><span class="sxs-lookup"><span data-stu-id="fe690-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="fe690-110">Vaadake oma säte üle.</span><span class="sxs-lookup"><span data-stu-id="fe690-110">Please review your setting.</span></span> <span data-ttu-id="fe690-111">See [juhend](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) aitab teil aru saada, kuidas KONFIGUREERIDA Azure AD Notificationi teatiste sätteid.</span><span class="sxs-lookup"><span data-stu-id="fe690-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="fe690-112">Lisateavet AAD Connecti Health Synci aruannete ja selle allalaadimise kohta leiate teemast [objekti taseme sünkroonimise teatis](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="fe690-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="fe690-113">Kui soovite, et AAD Connect Healthi teatised, järgige juhiseid, mis [on esitatud jaotises AAD ühenduse tervise andmete värskuse teatiste](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ja korduma kippuvate küsimuste kohta leiate teavet teemast [Üldine AAD Connect Health Installation](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="fe690-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
