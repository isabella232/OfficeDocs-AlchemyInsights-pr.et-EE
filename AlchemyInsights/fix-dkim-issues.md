---
title: DKIM setup probleemide lahendamine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506770"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="461d9-102">DKIM setup probleemide lahendamine</span><span class="sxs-lookup"><span data-stu-id="461d9-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="461d9-103">Kui teil tekib probleeme, mis võimaldavad DKIM oma kohandatud domeeni, toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="461d9-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="461d9-104">Enamik DKIM setup probleemid on seotud vale DNS-kirjete.</span><span class="sxs-lookup"><span data-stu-id="461d9-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="461d9-105">Kontrollige DKIM CNAME kirje (**mitte** TXT kirje) on õigesti vormindatud.</span><span class="sxs-lookup"><span data-stu-id="461d9-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="461d9-106">Lisateabe saamiseks vaadake seda [teemat](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="461d9-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="461d9-107">Pärast seda, kui loote või värskendage oma DKIM DNS-kirjete DNS-i hosting teenus domeeni (tavaliselt, teie domeeni kohtusekretäri), oodake DNS-kirjete paljundada.</span><span class="sxs-lookup"><span data-stu-id="461d9-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="461d9-108">Kui te ei saa luua DKIM DNS-kirjete administreerimiskeskus, saate asendada \<CustomDomain\> oma kohandatud domeeni (nt contoso.com) ja käivitage see käsk [Exchange Online PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="461d9-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
