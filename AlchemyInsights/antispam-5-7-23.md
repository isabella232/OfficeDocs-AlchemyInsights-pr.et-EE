---
title: Rämpspostitõrje – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821407"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="90437-102">Meiliedastusprobleemide lahendamine tõrkekoodi 5.7.23 korral</span><span class="sxs-lookup"><span data-stu-id="90437-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="90437-103">Kontrollige oma domeeni SPF-i DNS-i kirjet veebis avalikult saadaoleva SPF-i või DNS-i kirjekontrolli kaudu.</span><span class="sxs-lookup"><span data-stu-id="90437-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="90437-104">Veenduge, et Microsoft ei tuvastanud väljaminevat sõnumit rämpspostina ja marsruuditud suure [riskiga kohaletoimetamiskausta kaudu.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="90437-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="90437-105">Suure riskiga kohaletoimetamiskausta sõnumid ei läbi SPF-kontrolle ja seetõttu ei aktsepteeri sihtmeiliorganisatsioon.</span><span class="sxs-lookup"><span data-stu-id="90437-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="90437-106">Kui probleem ei lahene, peate võib-olla pöörduma selle meilihosti administraatori poole, kuhu proovite meilisõnumeid saata.</span><span class="sxs-lookup"><span data-stu-id="90437-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="90437-107">Pöörake tähelepanu üksikasjalikule välisele tõrkele, mis on tagasilöögisõnumis saadaval.</span><span class="sxs-lookup"><span data-stu-id="90437-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="90437-108">Microsofti tugi ei pruugi olla enam abiks.</span><span class="sxs-lookup"><span data-stu-id="90437-108">Microsoft support may not be able to assist further.</span></span>
