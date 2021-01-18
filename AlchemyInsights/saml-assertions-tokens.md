---
title: SAML kinnitused (märked)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885218"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="2a1d8-102">SAML kinnitused (märked)</span><span class="sxs-lookup"><span data-stu-id="2a1d8-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="2a1d8-103">Turbe kinnitused märgistuskeel (SAML) märgid on nõuete XML-esitus.</span><span class="sxs-lookup"><span data-stu-id="2a1d8-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="2a1d8-104">Vaikimisi väljastatakse SAML märgid Windowsi teatise Sihtasutus (WCF) välise turvalisuse stsenaariumid.</span><span class="sxs-lookup"><span data-stu-id="2a1d8-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="2a1d8-105">Lisateavet leiate teemast [SAML märgid ja nõuded](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="2a1d8-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="2a1d8-106">Microsoft Identity Platform eraldab iga autentimise voo töötlemiseks mitu tüüpi turbelubade.</span><span class="sxs-lookup"><span data-stu-id="2a1d8-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="2a1d8-107">[SAML sümboolne nõuete viide](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) kirjeldab vormingut, turbe omadusi ja SAML 2,0 märkide sisu.</span><span class="sxs-lookup"><span data-stu-id="2a1d8-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="2a1d8-108">Kui soovite teada, kuidas konfigureerida turbelubade eluiga, järgige juhiseid [Microsoft Identity Platformi konfigureeritav turbelubade eluajal](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) .</span><span class="sxs-lookup"><span data-stu-id="2a1d8-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="2a1d8-109">Järgige [selles artiklis](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) kirjeldatud juhiseid, et saada teada, kuidas KONFIGUREERIDA AZURE ad SAML turbelubade krüptimist.</span><span class="sxs-lookup"><span data-stu-id="2a1d8-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="2a1d8-110">Rakenduses Azure AD saate häälestada serdi allkirjastamise suvandeid ja serdi allkirjastamise algoritmi.</span><span class="sxs-lookup"><span data-stu-id="2a1d8-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="2a1d8-111">Lisateavet leiate teemast [Täpsemad serdi allkirjastamise suvandid rakenduses Azure Active Directory rakenduse Galerii rakenduste SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="2a1d8-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
