---
title: Wix-i veebisaidi kasutamine office 365 ostetud või hallatavate domeenidega
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825943"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="b82f7-102">Wix-i veebisaidi kasutamine office 365 ostetud või hallatavate domeenidega</span><span class="sxs-lookup"><span data-stu-id="b82f7-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="b82f7-103">Värskendage DNS-i kirjeid, et hoida oma veebisaiti praeguse majutusteenuse pakkuja juures</span><span class="sxs-lookup"><span data-stu-id="b82f7-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="b82f7-104">Wix-artikkel "Domeeni ühendamine Wix-iga osutamismeetodi abil" soovitab office 365 kasutamisel nimede serverite muutmise asemel kasutada osutamist (DNS-i kirjete lisamine ülaltoodud lingi kohta)</span><span class="sxs-lookup"><span data-stu-id="b82f7-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="b82f7-105">Kui otsustate endiselt muuta nimeserverid Wix-iks, peate microsofti jaoks  [wix-is dns-i kirjeid looma.](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="b82f7-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="b82f7-106">Kui teie domeen on ostetud Microsoftilt, ei saa nimeservereid muuta.</span><span class="sxs-lookup"><span data-stu-id="b82f7-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="b82f7-107">Kui peate nimeservereid muutma, tuleb Microsofti ostetud domeen 60 päeva pärast üle viia  [teisele hostiteenuse pakkujale.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span><span class="sxs-lookup"><span data-stu-id="b82f7-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span></span>