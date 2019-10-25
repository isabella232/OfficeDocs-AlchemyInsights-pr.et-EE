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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682106"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="386cc-102">Fix e kohaletoimetamise probleemid tõrkekoodi 5.7.23</span><span class="sxs-lookup"><span data-stu-id="386cc-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="386cc-103">Kontrollige SPF DNS-kirje oma domeeni avalikult saadaval SPF või DNS-i kirje kontrollija veebis.</span><span class="sxs-lookup"><span data-stu-id="386cc-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="386cc-104">Veenduge, et väljaminev sõnum ei tuvastatud rämpsposti Office 365 ja marsruuditatud [suure riski kohaletoimetamise kausta](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)kaudu.</span><span class="sxs-lookup"><span data-stu-id="386cc-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="386cc-105">Kõrge riskiga kohaletoimetamise pool sõnumid ei liigu SPF kontrolli ja seetõttu ei aktsepteerita sihtkoha e-posti organisatsioon.</span><span class="sxs-lookup"><span data-stu-id="386cc-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="386cc-106">Kui probleem ei lahene, peate pöörduma e-posti hosti administraatori poole, kuhu proovite meilisõnumeid saata.</span><span class="sxs-lookup"><span data-stu-id="386cc-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="386cc-107">Pange tähele üksikasjalikku välist viga saadaval põrketeates.</span><span class="sxs-lookup"><span data-stu-id="386cc-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="386cc-108">Office 365 tugi ei pruugi enam abiks olla.</span><span class="sxs-lookup"><span data-stu-id="386cc-108">Office 365 support may not be able to assist further.</span></span>