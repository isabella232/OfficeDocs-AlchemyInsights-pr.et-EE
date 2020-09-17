---
title: DKIM häälestamine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808703"
---
# <a name="setup-dkim"></a><span data-ttu-id="5170b-102">DKIM häälestamine</span><span class="sxs-lookup"><span data-stu-id="5170b-102">Setup DKIM</span></span>

<span data-ttu-id="5170b-103">Microsoft 365 kohandatud domeenide DKIM konfigureerimise terviklikud juhised on [siin](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="5170b-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="5170b-104">**Iga** kohandatud domeeni jaoks peate looma **kaks** DKIM CNAME-kirjet oma domeeni DNS-i hostimise teenuses (tavaliselt domeeni registripidaja).</span><span class="sxs-lookup"><span data-stu-id="5170b-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="5170b-105">Näiteks contoso.com ja fourthcoffee.com nõuavad nelja DKIM CNAME-kirjet: kaks contoso.com ja kaks fourthcoffee.com jaoks.</span><span class="sxs-lookup"><span data-stu-id="5170b-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="5170b-106">**Iga** kohandatud domeeni DKIM CNAME-kirjed kasutavad järgmisi vorminguid.</span><span class="sxs-lookup"><span data-stu-id="5170b-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="5170b-107">**Hosti nimi**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="5170b-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="5170b-108">Osutage **aadressile või väärtusele**.`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="5170b-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="5170b-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="5170b-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="5170b-110">**Hosti nimi**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="5170b-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="5170b-111">Osutage **aadressile või väärtusele**.`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="5170b-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="5170b-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="5170b-112">**TTL**: 3600</span></span>

   <span data-ttu-id="5170b-113">\<DomainGUID\> on `.mail.protection.outlook.com` kohandatud domeeni kohandatud MX-kirjest vasakul asuv tekst (nt `contoso-com` domeeni contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5170b-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="5170b-114">\<InitialDomain\> on domeen, mida kasutasite Microsoft 365 kasutajaks registreerumisel (nt contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="5170b-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="5170b-115">Kui olete oma kohandatud domeenide jaoks loonud CNAME-kirjed, tehke järgmised juhised.</span><span class="sxs-lookup"><span data-stu-id="5170b-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="5170b-116">loomine.</span><span class="sxs-lookup"><span data-stu-id="5170b-116">a.</span></span> <span data-ttu-id="5170b-117">[logige sisse rakendusse Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) oma töökoha või kooli kontoga.</span><span class="sxs-lookup"><span data-stu-id="5170b-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="5170b-118">b.</span><span class="sxs-lookup"><span data-stu-id="5170b-118">b.</span></span> <span data-ttu-id="5170b-119">Valige vasakus ülanurgas rakenduse käivitaja ikoon ja valige **administraator**.</span><span class="sxs-lookup"><span data-stu-id="5170b-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="5170b-120">c.</span><span class="sxs-lookup"><span data-stu-id="5170b-120">c.</span></span> <span data-ttu-id="5170b-121">Laiendage vasakus allnurgas nuppu **administraator** ja valige **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="5170b-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="5170b-122">d.</span><span class="sxs-lookup"><span data-stu-id="5170b-122">d.</span></span> <span data-ttu-id="5170b-123">Avage **kaitse**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="5170b-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="5170b-124">e.</span><span class="sxs-lookup"><span data-stu-id="5170b-124">e.</span></span> <span data-ttu-id="5170b-125">Valige domeen ja seejärel valige **DKIM allkirjaga selle domeeni jaoks sõnumite allkirjastamise** **lubamine** .</span><span class="sxs-lookup"><span data-stu-id="5170b-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="5170b-126">Korrake seda toimingut iga kohandatud domeeni korral.</span><span class="sxs-lookup"><span data-stu-id="5170b-126">Repeat this step for each custom domain.</span></span>
