---
title: Teatis AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035430"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="e4b12-102">Teatis AAD Connect</span><span class="sxs-lookup"><span data-stu-id="e4b12-102">Notification AAD Connect</span></span>

- <span data-ttu-id="e4b12-103">Veenduge, et teil on toimingu tegemiseks õigus.</span><span class="sxs-lookup"><span data-stu-id="e4b12-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="e4b12-104">Globaalsetel administraatoritel on vaikimisi juurdepääs.</span><span class="sxs-lookup"><span data-stu-id="e4b12-104">Global Admins have access by default.</span></span> <span data-ttu-id="e4b12-105">Lisaks saate kasutada [rolli baasil juurdepääsu juhtelementi](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , et anda delegaadile registreerimise õigused.</span><span class="sxs-lookup"><span data-stu-id="e4b12-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="e4b12-106">Veenduge, et nõutavad lõpp-punktid on lubatud ja tulemüüri tõttu blokeeritud.</span><span class="sxs-lookup"><span data-stu-id="e4b12-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="e4b12-107">Lisateavet leiate teemast [nõuded](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="e4b12-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="e4b12-108">Registreerimine võib nurjuda tänu sellele, et võrgu kiht teostab väljaminevat suhtlust SSL-i kaudu.</span><span class="sxs-lookup"><span data-stu-id="e4b12-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="e4b12-109">Veenduge, et olete kontrollinud Azure AD Connecti Healthi teatiste sätteid ja vaadake üle oma säte.</span><span class="sxs-lookup"><span data-stu-id="e4b12-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="e4b12-110">Kui soovite teada saada, kuidas konfigureerida Azure AD Notificationi teatiste sätteid, lugege seda [juhendit](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="e4b12-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="e4b12-111">Lisateavet AAD Connecti Health Synci aruannete ja selle allalaadimise kohta leiate teemast [objekti taseme sünkroonimise teatis](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="e4b12-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="e4b12-112">AAD Connect Healthi teatiste tõrkeotsinguks järgige juhiseid, mis puudutavad [AAD ühenduse tervise andmete värskuse teatiste](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ja korduma kippuvate küsimuste kohta leiate teavet teemast [Üldine AAD Connect Health Installation küsimused](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="e4b12-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
