---
title: LDAP-konfigureerimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885165"
---
# <a name="configure-ldap"></a><span data-ttu-id="3fd7f-102">LDAP-konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="3fd7f-102">Configure LDAP</span></span>

<span data-ttu-id="3fd7f-103">LDAP-i konfigureerimiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="3fd7f-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="3fd7f-104">Kontrollige oma domeeni tervist [Azure ' i portaalis](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="3fd7f-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="3fd7f-105">Veenduge, et saadaolev Azure AD tellimus on saadaval ja Azure AD Domain Services on lubatud.</span><span class="sxs-lookup"><span data-stu-id="3fd7f-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="3fd7f-106">Turvalise LDAP-i lubamiseks nõutav sert peab olema saadud usaldusväärsest avaliku sertimiskeskuse või iseallkirjastatud serdiga.</span><span class="sxs-lookup"><span data-stu-id="3fd7f-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="3fd7f-107">Veenduge, et sert järgib nõutavaid [juhiseid](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="3fd7f-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="3fd7f-108">**Kehtetu sert**</span><span class="sxs-lookup"><span data-stu-id="3fd7f-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="3fd7f-109">Serdi pikendamiseks järgige juhiseid uue serdi loomiseks ja uuesti üleslaadimiseks: LDAP-i [konfigureerimine](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3fd7f-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="3fd7f-110">Azure Active Directory Domain Services turvaliste LDAP-teatistega teadaoleva probleemi lahendamiseks lugege teemat [LDAP-teatiste lahendamine](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3fd7f-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
