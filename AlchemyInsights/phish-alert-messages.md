---
title: 2491 hoiatus e-kirju "Phish tarnitud tõttu rentniku või kasutaja alistamine" poliitika
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758905"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="3f4cb-102">Teavita e-kirju "Phish tarnitud tõttu rentniku või kasutaja alistamine" poliitika</span><span class="sxs-lookup"><span data-stu-id="3f4cb-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="3f4cb-103">Vaikimisi Alert poliitika nimega "Phish tarnitud tõttu rentniku või kasutaja alistamine" on välja antud rentnike Office 365 ATP P1 ja P2 litsentsid.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="3f4cb-104">Kui saite selle hoiatuse, on siin juhised uurimiseks.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="3f4cb-105">Hoiatusteate, klõpsake nuppu **Kuva hoiatus** , et minna **hoiatuste** lehele Security & vastavuse keskus.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="3f4cb-106">Valige teatis, et näha sõnumite **loendit** või **vaadata sõnumeid Exploreris**.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="3f4cb-107">Mõlemad suvandid viib teid sõnumi üksikasjadega, mis sisaldab sõnumi ID-ga.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="3f4cb-108">Pange tähele, et Ohuuurija link filtreerita automaatselt hoiatuskriteeriumidele vastavaid sõnumeid.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="3f4cb-109">Võimalik, et peate kohandama kuupäeva filtrit Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="3f4cb-110">Andmepüügiteade toimetati käsitsi konfigureeritud alistamise tõttu:</span><span class="sxs-lookup"><span data-stu-id="3f4cb-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="3f4cb-111">Kasutaja määratud lubatud saatja või Domeen.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="3f4cb-112">Lubatud saatja või domeeni määratud administraatori Rämpspostivastane poliitika.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="3f4cb-113">Ühenduse filtripoliitika lubatud IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="3f4cb-114">Meilivoo reegel (tuntud ka kui transpordireegel), mis on konfigureeritud sõnumite lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="3f4cb-115">Kui arvate, et sõnum oli valesti märgistatud Fish, kasutage Outlooki [aruande sõnumi lisandmoodul](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) edastada sõnumi näidised Microsoftile.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
