---
title: 726 meilisõnumite edasisaatmise blokeerimine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219851"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="b5006-102">Meilisõnumite edasisaatmise blokeerimine või blokeeringu tühistamine</span><span class="sxs-lookup"><span data-stu-id="b5006-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="b5006-103">Mõne kindla postkasti meilisõnumite edasisaatmise lubamiseks või keelamiseks vaadake teemat [meilisõnumite edasisaatmise konfigureerimine](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="b5006-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="b5006-104">Rentniku tasandil kontrollitakse välise edasisaatmise kontrolli väljamineva rämpsposti poliitika abil.</span><span class="sxs-lookup"><span data-stu-id="b5006-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="b5006-105">Kui see on välja lülitatud või automaatne, võib see blokeerida meilisõnumite edasisaatmise "550 5.7.520 juurdepääs keelatud, teie ettevõte ei luba välist edasisaatmist".</span><span class="sxs-lookup"><span data-stu-id="b5006-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="b5006-106">Seejärel, kui edasisaatmine oli seatud blokeerima, on see viga, mida kasutajad näevad.</span><span class="sxs-lookup"><span data-stu-id="b5006-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="b5006-107">Kui edasisaatmine on blokeeritud, veenduge, et poliitika oleks konfigureeritud väliste Autoforward lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="b5006-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="b5006-108">Väljamineva rämpsmeili filtri poliitika saate kontrollida turbe-ja vastavuskontrolli keskusest või käivitades käsu Get-HostedOutboundSpamFilterPolicy | välgu nimi, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="b5006-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="b5006-109">Kui soovite häälestada Autoforward blokeerimist, siis ütleb sama käsk teile kohe poliitika oleku.</span><span class="sxs-lookup"><span data-stu-id="b5006-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="b5006-110">Märkus: soovitatav on jätta välist Autoforward teie väljamineva rämpsmeili filtri poliitikas keelatud ja lubada seda ainult nende kasutajate jaoks, kes vajavad välisedasisaatmist, luues kohandatud poliitika nende kasutajate jaoks.</span><span class="sxs-lookup"><span data-stu-id="b5006-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="b5006-111">Lisateavet leiate teemast [väliste meilisõnumite edasisaatmise konfigureerimine rakenduses Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="b5006-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>