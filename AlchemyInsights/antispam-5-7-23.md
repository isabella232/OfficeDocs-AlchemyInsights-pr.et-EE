---
title: Rämpspostitõrje-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506439"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f140b-102">Fix e kohaletoimetamise probleemid tõrkekoodi 5.7.23</span><span class="sxs-lookup"><span data-stu-id="f140b-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f140b-103">Kontrollige SPF DNS-kirje oma domeeni avalikult saadaval SPF või DNS-i kirje kontrollija veebis.</span><span class="sxs-lookup"><span data-stu-id="f140b-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f140b-104">Veenduge, et väljaminev sõnum ei tuvastatud rämpsposti Microsoft ja marsruuditatud [suure riski kohaletoimetamise kausta](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)kaudu.</span><span class="sxs-lookup"><span data-stu-id="f140b-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f140b-105">Kõrge riskiga kohaletoimetamise pool sõnumid ei liigu SPF kontrolli ja seetõttu ei aktsepteerita sihtkoha e-posti organisatsioon.</span><span class="sxs-lookup"><span data-stu-id="f140b-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f140b-106">Kui probleem ei lahene, peate pöörduma e-posti hosti administraatori poole, kuhu proovite meilisõnumeid saata.</span><span class="sxs-lookup"><span data-stu-id="f140b-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f140b-107">Pange tähele üksikasjalikku välist viga saadaval põrketeates.</span><span class="sxs-lookup"><span data-stu-id="f140b-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="f140b-108">Microsofti tugiteenis ei pruugi enam abiks olla.</span><span class="sxs-lookup"><span data-stu-id="f140b-108">Microsoft support may not be able to assist further.</span></span>
