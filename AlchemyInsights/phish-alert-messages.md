---
title: 2491 teatiste e-kirju poliitikast "Phish tarnitud rentniku või kasutaja alistada"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391228"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="28d80-102">Teatiste e-kirju poliitikast "Phish tarnitud rentniku või kasutaja alistada"</span><span class="sxs-lookup"><span data-stu-id="28d80-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="28d80-103">Alert vaikepoliitika nimeks "Phish andis tõttu rentniku või kasutaja alistamine" rullitakse üürnike Office 365 ATP P1 ja P2 litsentsiga.</span><span class="sxs-lookup"><span data-stu-id="28d80-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="28d80-104">Kui teemasse, siis siin on korras uurida:</span><span class="sxs-lookup"><span data-stu-id="28d80-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="28d80-105">Klõpsake hoiatusteate, turvalisuse & vastavuse Center lehe **teatiste** **Vaate teatise** .</span><span class="sxs-lookup"><span data-stu-id="28d80-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="28d80-106">Valige märguanne, et **vaadata sõnumi** või **sõnumite kuvamine Exploreris**ei näe.</span><span class="sxs-lookup"><span data-stu-id="28d80-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="28d80-107">Mõlemad Valikud viivad teid üksikasjad ning mis sisaldab sõnumi ID-d.</span><span class="sxs-lookup"><span data-stu-id="28d80-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="28d80-108">Pange tähele, et oht Explorer link automaatselt filtreerida sõnumite, teatiste kriteeriumile vastavad.</span><span class="sxs-lookup"><span data-stu-id="28d80-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="28d80-109">Peate kohandada ohtu Exploreri Kuupäevafilter.</span><span class="sxs-lookup"><span data-stu-id="28d80-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="28d80-110">Phishing sõnumi kättetoimetamise tõttu käsitsi konfigureeritud alistamine:</span><span class="sxs-lookup"><span data-stu-id="28d80-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="28d80-111">Lubatud saatja või domeeni kasutaja määratud.</span><span class="sxs-lookup"><span data-stu-id="28d80-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="28d80-112">Lubatud saatja või domeeni admin Rämpspostivastane poliitika seatud.</span><span class="sxs-lookup"><span data-stu-id="28d80-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="28d80-113">Lubatud IP-aadressi ühenduse filter poliitika.</span><span class="sxs-lookup"><span data-stu-id="28d80-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="28d80-114">Mail voolu reeglina (ka Transpordireegli) on konfigureeritud lubama sõnumeid.</span><span class="sxs-lookup"><span data-stu-id="28d80-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="28d80-115">Kui arvate, et sõnum oli valesti märgitud phish, kasuta Outlook [teatesõnum lisandmoodul](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Microsoft sõnumi proovide.</span><span class="sxs-lookup"><span data-stu-id="28d80-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
