---
title: 2491 teatise meilisõnumid Phish, mis on tarnitud rentniku või kasutaja alistamise poliitika tõttu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728607"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="c50fb-102">Meilisõnumite teavitamine rentniku või kasutaja alistamise tõttu antud Phish</span><span class="sxs-lookup"><span data-stu-id="c50fb-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="c50fb-103">Vaike-teatise poliitika, mille nimi on "rentniku või kasutaja alistamise tõttu", on välja antud rentnikele, kellel on Office 365 ATP P1 ja P2 litsentsid.</span><span class="sxs-lookup"><span data-stu-id="c50fb-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="c50fb-104">Kui saite teatise, saate uurida järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="c50fb-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="c50fb-105">Klõpsake hoiatusteate nuppu **Kuva teatis** , et minna turbe & vastavuskontrolli lehe lehele **teatised** .</span><span class="sxs-lookup"><span data-stu-id="c50fb-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="c50fb-106">Valige teatis, et näha **sõnumite loendit** ja **vaadata sõnumeid Exploreris**.</span><span class="sxs-lookup"><span data-stu-id="c50fb-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="c50fb-107">Mõlemad suvandid viivad teid sõnumi üksikasjade juurde, mis sisaldab sõnumi ID-dokumenti.</span><span class="sxs-lookup"><span data-stu-id="c50fb-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="c50fb-108">Pange tähele, et ohu Exploreri link filtreerib automaatselt teatiste kriteeriumidele vastavaid sõnumeid.</span><span class="sxs-lookup"><span data-stu-id="c50fb-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="c50fb-109">Võimalik, et peate täpsustama ohu Exploreris kuupäeva filtrit.</span><span class="sxs-lookup"><span data-stu-id="c50fb-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="c50fb-110">Andmepüügifilter edastati käsitsi konfigureeritud alistamise tõttu.</span><span class="sxs-lookup"><span data-stu-id="c50fb-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="c50fb-111">Kasutaja määratud lubatud saatja või Domeen.</span><span class="sxs-lookup"><span data-stu-id="c50fb-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="c50fb-112">Lubatud saatja või domeen, mille administraator on rämpsposti poliitikas määranud.</span><span class="sxs-lookup"><span data-stu-id="c50fb-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="c50fb-113">Lubatud IP-aadress seoses filtri poliitikaga.</span><span class="sxs-lookup"><span data-stu-id="c50fb-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="c50fb-114">Meilivoo reegel (tuntud ka kui transpordi reegel), mis on konfigureeritud sõnumite lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="c50fb-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="c50fb-115">Kui arvate, et sõnum oli valesti märgitud kui Phish, kasutage meilisõnumite saatmiseks Microsoftile sõnumite saatmiseks Outlooki [aruannete lisandmoodulit](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) .</span><span class="sxs-lookup"><span data-stu-id="c50fb-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
