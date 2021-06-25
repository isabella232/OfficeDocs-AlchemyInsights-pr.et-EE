---
title: Meilisõnumite edastamine Microsoft 365 kaudu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117979"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="9355b-102">Mitmeotstarbelise seadme või rakenduse häälestamine meili saatma</span><span class="sxs-lookup"><span data-stu-id="9355b-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="9355b-103">Teavet variantide kohta ja juhised leiate artiklist [Mitmeotstarbelise seadme või rakenduse häälestamine Microsoft 365 kaudu meili saatma](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="9355b-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="9355b-104">Kui teil on seade või rakendus, mis on hiljuti lõpetanud töötamise, on kõige levinumad probleemid järgmised.</span><span class="sxs-lookup"><span data-stu-id="9355b-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="9355b-105">**Autentimistõrked SMTP-autentimisrakenduse edastuse kasutamisel** Oleme hiljuti teinud mõned muudatused seoses SMTP-autentimise tööga.</span><span class="sxs-lookup"><span data-stu-id="9355b-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="9355b-106">Probleemide lahendamise kohta leiate lisateavet jaotisest Printerite, skannerite ja [LOB-rakendustega](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)seotud probleemide lahendamine, mis saadavad meilisõnumeid Microsoft 365 või Office 365 .</span><span class="sxs-lookup"><span data-stu-id="9355b-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="9355b-107">**Aktsepteerime ainult TLS 1.2 versiooni,** kui teeme turvalise ühenduse Office 365 Kui kasutate turvalist ühendust (TLS), veenduge, et teie rakendusseade toetab TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="9355b-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="9355b-108">Lisateavet leiate teemast [TLS 1.2 ettevalmistamine Office 365 ja Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9355b-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="9355b-109">Muude probleemide ja lahenduste kohta leiate teavet teemast Probleemide lahendamine printerite, skannerite ja [LOB-rakendustega,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)mis saadavad meilisõnumeid Microsoft 365 või Office 365 .</span><span class="sxs-lookup"><span data-stu-id="9355b-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="9355b-110">Mõjutatud seadmete kuvamiseks avage [SMTP autentimise kliendi aruanne](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="9355b-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="9355b-111">**Märkus.** Exchange Online ei mahu hulgipostitusstsenaariumidesse.</span><span class="sxs-lookup"><span data-stu-id="9355b-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="9355b-112">Hulgimeilisõnumite (nt klientide teabelehtede) saatmiseks peaksite kasutama nendele teenustele spetsialiseerunud kolmanda osapoole teenusepakkujaid.</span><span class="sxs-lookup"><span data-stu-id="9355b-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
