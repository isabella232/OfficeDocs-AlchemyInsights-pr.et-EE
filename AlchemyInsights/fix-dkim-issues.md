---
title: DKIM installiprobleemide lahendamiseks
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764999"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="6a4f9-102">DKIM installiprobleemide lahendamiseks</span><span class="sxs-lookup"><span data-stu-id="6a4f9-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="6a4f9-103">Kui teil tekib küsimusi, mis võimaldavad DKIM oma kohandatud domeeni, tehke järgmist:</span><span class="sxs-lookup"><span data-stu-id="6a4f9-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="6a4f9-104">Enamik DKIM installiprobleemide on seotud vale DNS-kirjeid.</span><span class="sxs-lookup"><span data-stu-id="6a4f9-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="6a4f9-105">Kontrollida (**ole** TXT-kirje) DKIM CNAME-kirje on õigesti vormindatud.</span><span class="sxs-lookup"><span data-stu-id="6a4f9-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6a4f9-106">Lisateavet vt selle [teema](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="6a4f9-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="6a4f9-107">Pärast loomist või värskendada oma DKIM DNS-kirjeid DNS-i hostimisteenuses domeeni (tavaliselt oma domeeniregistraatori), oodake, kuni DNS-kirjete propageerida.</span><span class="sxs-lookup"><span data-stu-id="6a4f9-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="6a4f9-108">Kui te ei saa luua DKIM DNS kirjed administreerimiskeskuses, saate asendada \<CustomDomain\> kohandatud domeeni (nt contoso.com) ja piisavaid [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)PowerShelli: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="6a4f9-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
