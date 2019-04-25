---
title: Tõrkeotsingu koos Office 365 arenenud oht kaitse (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420296"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="4332c-102">Office 365 ATP tõrkeotsingu</span><span class="sxs-lookup"><span data-stu-id="4332c-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="4332c-103">**Teade viivitusi e-posti sõnumi kohaletoimetamine**?</span><span class="sxs-lookup"><span data-stu-id="4332c-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="4332c-104">Proovige kasutada ATP Safe Attachments poliitika dünaamiline tellimise võimalus.</span><span class="sxs-lookup"><span data-stu-id="4332c-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="4332c-105">See aitab vältida e-posti sõnumi kohaletoimetamise viivituste, samal ajal kaitstes adressaadid pahatahtlike faile.</span><span class="sxs-lookup"><span data-stu-id="4332c-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="4332c-106">**Kas soovite aruande valepositiivseid või valenegatiivseid**?</span><span class="sxs-lookup"><span data-stu-id="4332c-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="4332c-107">Selle lingi kaudu saada fail analüüsiks:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="4332c-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="4332c-108">**Kas teadsite, et saate lubada ATP Safe Links kaitse meilisõnumid ettevõtte vahel**?</span><span class="sxs-lookup"><span data-stu-id="4332c-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="4332c-109">Toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="4332c-109">Follow these steps:</span></span>
    1. <span data-ttu-id="4332c-110">Mine https://protection.office.com, ja logige sisse.</span><span class="sxs-lookup"><span data-stu-id="4332c-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="4332c-111">Mine **ohu haldamise** > **poliitika** > **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="4332c-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="4332c-112">**Saada adressaatidega poliitika**raames muuta või lisada poliitika.</span><span class="sxs-lookup"><span data-stu-id="4332c-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="4332c-113">Valige **Rakenda ohutu lingid saadetud organisatsiooni sees**.</span><span class="sxs-lookup"><span data-stu-id="4332c-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="4332c-114">Salvestage oma poliitika ja umbes 30 minutit muutuste ilmnemine oma andmekeskuse.</span><span class="sxs-lookup"><span data-stu-id="4332c-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="4332c-115">ATP täiendava abi saamiseks vt [Office 365 täiustatud ohutõrje](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="4332c-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>