---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717321"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="ae68e-102">Meili kohaletoimetamisega seotud probleemide lahendamine tõrkekood 5.7.23</span><span class="sxs-lookup"><span data-stu-id="ae68e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="ae68e-103">Kontrollige oma domeeni SPF-i DNS-i kirjet avalikult kättesaadaval SPF-või DNS-i kirje kontrollijal veebis.</span><span class="sxs-lookup"><span data-stu-id="ae68e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="ae68e-104">Veenduge, et Microsoft ei tuvastanud väljaminevat sõnumit rämpspostina ja marsruuditakse [suure riski kohaletoimetamise puuli](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)kaudu.</span><span class="sxs-lookup"><span data-stu-id="ae68e-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="ae68e-105">Suure riskiga kohaletoimetamise pargis olevad sõnumid ei anna SPF-i tšekke ning seetõttu ei aktsepteeri sihtkoha e-posti organisatsioon seda.</span><span class="sxs-lookup"><span data-stu-id="ae68e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="ae68e-106">Kui probleem ei lahene, peate ühendust võtma selle meilikasutaja administraatoriga, kellele proovite meilisõnumeid saata.</span><span class="sxs-lookup"><span data-stu-id="ae68e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="ae68e-107">Märkige üles põrge sõnumis saadaolev üksikasjalik väline tõrge.</span><span class="sxs-lookup"><span data-stu-id="ae68e-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="ae68e-108">Võimalik, et Microsofti tugi ei saa enam abiks olla.</span><span class="sxs-lookup"><span data-stu-id="ae68e-108">Microsoft support may not be able to assist further.</span></span>
