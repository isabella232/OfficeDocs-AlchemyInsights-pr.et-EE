---
title: Turbelubade nõuete ja atribuutidega seotud probleemid
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035888"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="ce7e2-102">Turbelubade nõuete ja atribuutidega seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="ce7e2-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="ce7e2-103">**Turbelubade nõuete värskendamine, konfigureerimine või eemaldamine**</span><span class="sxs-lookup"><span data-stu-id="ce7e2-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="ce7e2-104">Azure Active Directory (Azure AD) abil saate [kohandada nõude tüüpi argumenti](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) , mis on esitatud vastuses, mis kuvatakse pärast rakenduse autoriseerimist.</span><span class="sxs-lookup"><span data-stu-id="ce7e2-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="ce7e2-105">Rakenduse arendajad saavad oma Azure AD rakendustes kasutada fakultatiivseid nõudeid, et määrata, milliseid nõudeid nad soovivad oma rakendusse saadetavate märkidega.</span><span class="sxs-lookup"><span data-stu-id="ce7e2-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="ce7e2-106">Lisateavet leiate teemast [valikuliste nõuete pakkumine rakenduse](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)jaoks.</span><span class="sxs-lookup"><span data-stu-id="ce7e2-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="ce7e2-107">[Rühma taotluste konfigureerimine Azure Active Directory rakenduste jaoks](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="ce7e2-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="ce7e2-108">Kui kasutate rakenduse sujuvat ühekordset sisselogimist, lugege teemat [SAML lubamine Enterprise ' i rakenduste jaoks välja antud nõuete kohandamine](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="ce7e2-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="ce7e2-109">**Nõuded atribuutide vastendamiseks**</span><span class="sxs-lookup"><span data-stu-id="ce7e2-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="ce7e2-110">Nõuete vastendamise poliitika konfigureerimiseks PowerShelli abil lugege artiklit [rentniku jaoks teatud rakenduse märkidest eralduvate nõuete kohandamine (eelvaade)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="ce7e2-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="ce7e2-111">Directory skeemi laiendi atribuudid pakuvad võimalust salvestada täiendavaid andmeid Azure Active Directory kasutaja objektid ja muud Directory objektid (nt rühmad, rentniku andmed, teenuse põhiosa).</span><span class="sxs-lookup"><span data-stu-id="ce7e2-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="ce7e2-112">Taotlustele nõuete tekitamiseks saab kasutada ainult kasutajate objektide laienduste atribuute.</span><span class="sxs-lookup"><span data-stu-id="ce7e2-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="ce7e2-113">[Directory skeemi laiendi atribuutide kasutamine nõuetes kirjeldab,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) kuidas kasutada kataloogi skeemi laiendi atribuute, et saata kasutaja andmeid turbelubade taotlustele.</span><span class="sxs-lookup"><span data-stu-id="ce7e2-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="ce7e2-114">Lisateavet turbelubade kohta leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="ce7e2-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="ce7e2-115">Nõuded Accessi märkidest</span><span class="sxs-lookup"><span data-stu-id="ce7e2-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="ce7e2-116">Id_token nõuded</span><span class="sxs-lookup"><span data-stu-id="ce7e2-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="ce7e2-117">[Nõuded](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , mida võid oodata AZURE ad B2C väljastatud ID märkide ja juurdepääsulubaega</span><span class="sxs-lookup"><span data-stu-id="ce7e2-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="ce7e2-118">SAML loa nõuete viide</span><span class="sxs-lookup"><span data-stu-id="ce7e2-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
