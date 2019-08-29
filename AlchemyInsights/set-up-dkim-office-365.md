---
title: Setup DKIM Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666260"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="9f14f-102">Setup DKIM Office 365</span><span class="sxs-lookup"><span data-stu-id="9f14f-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="9f14f-103">Täielikud juhised konfigureerimine DKIM kohandatud domeenide Office 365 on [siin](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9f14f-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="9f14f-104">**Iga** kohandatud domeeni, peate looma **kaks** DKIM CNAME kirjeid oma domeeni DNS-i hosting teenus (tavaliselt, domeeni kohtusekretäri).</span><span class="sxs-lookup"><span data-stu-id="9f14f-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="9f14f-105">Näiteks contoso.com ja fourthcoffee.com nõuavad nelja DKIM CNAME kirjeid: kaks contoso.com ja kaks fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="9f14f-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="9f14f-106">DKIM CNAME kirjed **iga** kohandatud domeeni kasutada järgmisi vorminguid:</span><span class="sxs-lookup"><span data-stu-id="9f14f-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="9f14f-107">**Hosti nimi**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f14f-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9f14f-108">**Osutab aadressile või väärtusele**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f14f-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9f14f-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9f14f-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="9f14f-110">**Hosti nimi**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f14f-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9f14f-111">**Osutab aadressile või väärtusele**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9f14f-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9f14f-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9f14f-112">**TTL**: 3600</span></span>

   <span data-ttu-id="9f14f-113">\<DomainGUID\> on kohandatud domeeni kohandatud MX-kirjes vasakul `.mail.protection.outlook.com` olev tekst (nt domeeni contoso.com `contoso-com` puhul).</span><span class="sxs-lookup"><span data-stu-id="9f14f-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="9f14f-114">\<InitialDomain\> on domeen, mida kasutasite, kui registreerite Office 365 (nt contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="9f14f-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="9f14f-115">Pärast seda, kui olete loonud oma kohandatud domeenide CNAME-kirjed, täitke järgmised juhised:</span><span class="sxs-lookup"><span data-stu-id="9f14f-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="9f14f-116">A.</span><span class="sxs-lookup"><span data-stu-id="9f14f-116">a.</span></span> <span data-ttu-id="9f14f-117">[Logige sisse Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) oma töö või kooli kontoga.</span><span class="sxs-lookup"><span data-stu-id="9f14f-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="9f14f-118">B.</span><span class="sxs-lookup"><span data-stu-id="9f14f-118">b.</span></span> <span data-ttu-id="9f14f-119">Valige ülemise vasakpoolse rakenduse käivitaja ikoon ja valige **admin**.</span><span class="sxs-lookup"><span data-stu-id="9f14f-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="9f14f-120">C.</span><span class="sxs-lookup"><span data-stu-id="9f14f-120">c.</span></span> <span data-ttu-id="9f14f-121">Alumises vasakus navigeerimise, laiendage **admin** ja valige **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="9f14f-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="9f14f-122">D.</span><span class="sxs-lookup"><span data-stu-id="9f14f-122">d.</span></span> <span data-ttu-id="9f14f-123">Mine **kaitse** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="9f14f-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="9f14f-124">E.</span><span class="sxs-lookup"><span data-stu-id="9f14f-124">e.</span></span> <span data-ttu-id="9f14f-125">Valige domeen ja seejärel valige **Luba** **Logi sõnumid selle domeeni DKIM allkirjad**.</span><span class="sxs-lookup"><span data-stu-id="9f14f-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="9f14f-126">Korrake seda toimingut iga kohandatud domeeni puhul.</span><span class="sxs-lookup"><span data-stu-id="9f14f-126">Repeat this step for each custom domain.</span></span>
