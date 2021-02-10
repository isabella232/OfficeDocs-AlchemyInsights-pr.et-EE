---
title: Domeeni teenuse parooli Hash sünkroonimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177416"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="c6394-102">Domeeni teenuse parooli Hash sünkroonimine</span><span class="sxs-lookup"><span data-stu-id="c6394-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="c6394-103">**Kui teie Azure AD DS-i eksemplar palub teil parooli räsi sünkroonimise lubada**</span><span class="sxs-lookup"><span data-stu-id="c6394-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="c6394-104">Ilmneb stsenaarium, kus töötab hübriid-keskkond, kus kasutajad sünkroonivad kohapealset Azure Active Directory Domain Services (AD DS) keskkonda.</span><span class="sxs-lookup"><span data-stu-id="c6394-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="c6394-105">See stsenaarium ilmneb hoolimata sellest, et teil on kohapealne AD DS-i Azure AD rentniku jaoks parooli räsi sünkroonimine.</span><span class="sxs-lookup"><span data-stu-id="c6394-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="c6394-106">**Põhjustada**</span><span class="sxs-lookup"><span data-stu-id="c6394-106">**Cause**</span></span>

<span data-ttu-id="c6394-107">See juhtub, sest Azure AD Connect vaikimisi ei sünkroonita pärand uus tehnoloogia LAN Manageri (NTLM) ja Kerberose parool hashes, mis on vajalik Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="c6394-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="c6394-108">**Ajutine lahendus**</span><span class="sxs-lookup"><span data-stu-id="c6394-108">**Workaround**</span></span> 

<span data-ttu-id="c6394-109">Peate konfigureerima Azure AD Connecti, et sünkroonida NTLM-ja Kerberose autentimise jaoks nõutavad parooli hashud.</span><span class="sxs-lookup"><span data-stu-id="c6394-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="c6394-110">Kui Azure AD Connect on konfigureeritud, siis sünkroonitakse ka kohapealne konto loomise või parooli muutmise sündmus ja seejärel sünkroonitakse pärand parooli hashes Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c6394-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="c6394-111">Lisateavet leiate [siit](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) ja juhised selle kohta, kuidas lubada AZURE AD DS Hybrid keskkonnas parooli sünkroonimine.</span><span class="sxs-lookup"><span data-stu-id="c6394-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>