---
title: Office‘t ei saa aktiveerida
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798676"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="30a1b-102">Office‘t ei saa aktiveerida</span><span class="sxs-lookup"><span data-stu-id="30a1b-102">Unable to activate Office</span></span>

<span data-ttu-id="30a1b-103">**Märkus.** Kui kasutate vanemat versiooni Windows (nt Windows 7), veenduge, et TLS 1.2 oleks vaikimisi lubatud.</span><span class="sxs-lookup"><span data-stu-id="30a1b-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="30a1b-104">Lisateavet leiate teemast [Värskendus TLS 1.1 ja TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)lubamiseks winHTTP-s vaikimisi turvaliste protokollidena Windows .</span><span class="sxs-lookup"><span data-stu-id="30a1b-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="30a1b-105">Kontrollige, kas teie tellimuse olek on aegunud.</span><span class="sxs-lookup"><span data-stu-id="30a1b-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="30a1b-106">Veenduge, et teil on tellimus, mis võimaldab kliendilitsentse (nt Office 365 Business või Business Premium) ning et [kasutajal on määratud litsents](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="30a1b-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="30a1b-107">Veenduge, et kasutaja oleks Office’isse sisse logitud sama kontoga, millele on määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="30a1b-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="30a1b-108">Vaadake [Office 365 teenuste seisundi lehelt](/office365/enterprise/view-service-health) järele, kas teenusega on teadaolevalt probleeme.</span><span class="sxs-lookup"><span data-stu-id="30a1b-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="30a1b-109">Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, veendumaks, et need ei blokeeri Microsoft 365 rakenduste interneti-pääsu.</span><span class="sxs-lookup"><span data-stu-id="30a1b-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="30a1b-110">Lugege teemat [Office 365 URL-id ja IP-aadresside vahemikud](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL-id ja IP-aadresside vahemikud").</span><span class="sxs-lookup"><span data-stu-id="30a1b-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="30a1b-111">**Näpunäide** Windowsi seadmetes saame diagnoosida ja automaatselt lahendada mitmed levinud Office'i sisselogimisprobleeme.</span><span class="sxs-lookup"><span data-stu-id="30a1b-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="30a1b-112">Meie automatiseeritud tööriista kasutamiseks laadige alla ja käivitage **[Microsofti tugi- ja taasteteenuste abiline](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="30a1b-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="30a1b-113">Saate kasutada järgmisi tõrkeotsingu toiminguid.</span><span class="sxs-lookup"><span data-stu-id="30a1b-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="30a1b-114">Avage Office’i rakendus ja [logige](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) kõigist olemasolevatest kasutajakontotest välja.</span><span class="sxs-lookup"><span data-stu-id="30a1b-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="30a1b-115">[Eemaldage](/microsoft-365/admin/manage/remove-licenses-from-users) Office’i litsents ja [määrake see uuesti](/microsoft-365/admin/manage/assign-licenses-to-users) ning seejärel [logige Office’isse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakontoga sisse.</span><span class="sxs-lookup"><span data-stu-id="30a1b-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="30a1b-116">Käivitage [aktiveerimise tõrkeotsija](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="30a1b-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="30a1b-117">Määrake uuesti Office’i aktiveerimisolek</span><span class="sxs-lookup"><span data-stu-id="30a1b-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office’i aktiveerimisoleku lähtestamine")
- [<span data-ttu-id="30a1b-118">Parandage Office võrgus</span><span class="sxs-lookup"><span data-stu-id="30a1b-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="30a1b-119">Täiendavad tõrkeotsingu lahendused leiate järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="30a1b-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="30a1b-120">Litsentsimata toote ja aktiveerimisega seotud tõrketeated Office’is</span><span class="sxs-lookup"><span data-stu-id="30a1b-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="30a1b-121">Office’i aktiveerimisel kuvatakse tõrketeade: „Kahjuks ei saa teie kontoga ühendust luua. Proovige hiljem uuesti.“</span><span class="sxs-lookup"><span data-stu-id="30a1b-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)