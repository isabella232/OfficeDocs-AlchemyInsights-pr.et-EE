---
title: Levinud probleemide lahendamine DKIM kirje vorminguga
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524399"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="d4360-102">Levinud probleemide lahendamine DKIM kirje vorminguga</span><span class="sxs-lookup"><span data-stu-id="d4360-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="d4360-103">Enamik DKIM on seotud valede DNS-i kirjetega.</span><span class="sxs-lookup"><span data-stu-id="d4360-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="d4360-104">DKIM lahendamiseks veenduge, et DKIM CNAME-kirje (**mitte** TXT-kirje) oleks õigesti vormindatud.</span><span class="sxs-lookup"><span data-stu-id="d4360-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="d4360-105">Lisateavet leiate teemast [mida peate tegema DKIM käsitsi häälestamiseks rakenduses Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="d4360-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="d4360-106">Kui vajate DNS-i kirjete üldist abi, lugege teemat [DNS-i kirjete loomine veebisaidil Office 365 DNS-i majutusteenuse pakkuja](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="d4360-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="d4360-107">Pärast seda, kui olete oma domeeni DNS-i DKIM loonud või värskendanud DNS-i kirjeid, peate ootama, kuni DNS-i kirjed on paljundatud.</span><span class="sxs-lookup"><span data-stu-id="d4360-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
