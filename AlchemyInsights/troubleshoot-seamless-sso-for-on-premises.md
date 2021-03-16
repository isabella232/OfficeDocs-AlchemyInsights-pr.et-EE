---
title: Kohapealsete tõrgeteta ühekordse sisselogimise (SSO) tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816127"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="70473-102">Kohapealsete tõrgeteta ühekordse sisselogimise (SSO) tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="70473-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="70473-103">Tõrgeteta ühekordse sisselogimise (SSO) probleemide lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="70473-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="70473-104">**Kuidas saan AZUREADSSO arvuti konto Kerberose dekrüptimise võtit üle rullida?**</span><span class="sxs-lookup"><span data-stu-id="70473-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="70473-105">Soovitame tungivalt üle minna Kerberose dekrüptimise võtmest vähemalt iga 30 päeva järel.</span><span class="sxs-lookup"><span data-stu-id="70473-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="70473-106">Kui soovite seda teha käsitsi, lugege teemat [Kerberose dekrüptimise võtmete ümberpööramine](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="70473-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="70473-107">**Sujuva SSO konfigureerimine**</span><span class="sxs-lookup"><span data-stu-id="70473-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="70473-108">Sujuva SSO juurutamiseks järgige [Azure Active Directory õmblusteta ühekordse sisselogimise juhiseid: Kiirjuhend](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="70473-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="70473-109">**Nõuandev teade**</span><span class="sxs-lookup"><span data-stu-id="70473-109">**Advisory**</span></span>

- <span data-ttu-id="70473-110">[Azure Active Directory sujuv Ühekordne sisselogimine: korduma kippuvad küsimused](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) – selles artiklis käsitleme korduma kippuvaid küsimusi Azure Active Directory õmblusteta ühe Sign-On (sujuv SSO) kohta.</span><span class="sxs-lookup"><span data-stu-id="70473-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="70473-111">Jätkake uue sisu kontrollimist.</span><span class="sxs-lookup"><span data-stu-id="70473-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="70473-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – sellest artiklist leiate teavet selle kohta, kuidas teha funktsioonide taotlusi või esitada tehnilisi küsimusi õmblusteta SSO kohta.</span><span class="sxs-lookup"><span data-stu-id="70473-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="70473-113">**Tõrkeotsing**</span><span class="sxs-lookup"><span data-stu-id="70473-113">**Troubleshoot**</span></span>

<span data-ttu-id="70473-114">[Azure Active Directory tõrgeteta ühekordse sisselogimise tõrkeotsing](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) – see artikkel aitab teil leida tõrkeotsingu teavet seoses Azure Active Directory (Azure AD) õmblusteta ühekordse Sign-On (sujuv SSO) levinumate probleemidega.</span><span class="sxs-lookup"><span data-stu-id="70473-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







