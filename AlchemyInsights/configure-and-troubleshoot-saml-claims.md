---
title: SAML nõuete konfigureerimine ja tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900866"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="8e854-102">SAML nõuete konfigureerimine ja tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="8e854-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="8e854-103">SAML nõuete konfigureerimiseks ja tõrkeotsinguks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="8e854-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="8e854-104">Järgige [selles artiklis](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) kirjeldatud juhiseid ettevõtteportaali SAML turbelubade jaoks antud rolli konfigureerimiseks.</span><span class="sxs-lookup"><span data-stu-id="8e854-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="8e854-105">Järgige [selle artikli](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) juhiseid, et kohandada SAML-i turbelubade jaoks välja antud nõudeid.</span><span class="sxs-lookup"><span data-stu-id="8e854-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="8e854-106">Järgige [selles artiklis](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) toodud juhiseid, et kohandada teatud rakenduse rentniku jaoks määratud märkidest tulenevaid nõudeid.</span><span class="sxs-lookup"><span data-stu-id="8e854-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="8e854-107">Lugege [seda artiklit](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) , et mõista rakenduse puhverserveri kaudu töötamisest nõuetest teadlikke rakendusi.</span><span class="sxs-lookup"><span data-stu-id="8e854-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>