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
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812568"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="c0a17-102">Office‘t ei saa aktiveerida</span><span class="sxs-lookup"><span data-stu-id="c0a17-102">Unable to activate Office</span></span>

- <span data-ttu-id="c0a17-103">Kontrollige, kas teie tellimuse olek on aegunud.</span><span class="sxs-lookup"><span data-stu-id="c0a17-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="c0a17-104">Veenduge, et teil on tellimus, mis võimaldab kliendilitsentse (nt Office 365 Business või Business Premium) ning et [kasutajal on määratud litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c0a17-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="c0a17-105">Veenduge, et kasutaja oleks Office’isse sisse logitud sama kontoga, millele on määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="c0a17-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="c0a17-106">Vaadake [Office 365 teenuste seisundi lehelt](https://docs.microsoft.com/office365/enterprise/view-service-health) järele, kas teenusega on teadaolevalt probleeme.</span><span class="sxs-lookup"><span data-stu-id="c0a17-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="c0a17-107">Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, veendumaks, et need ei blokeeri Microsoft 365 rakenduste interneti-pääsu.</span><span class="sxs-lookup"><span data-stu-id="c0a17-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="c0a17-108">Lugege teemat [Office 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL-id ja IP-aadresside vahemikud").</span><span class="sxs-lookup"><span data-stu-id="c0a17-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="c0a17-109">**Näpunäide** Windowsi seadmetes saame diagnoosida ja automaatselt lahendada mitmed levinud Office'i sisselogimisprobleeme.</span><span class="sxs-lookup"><span data-stu-id="c0a17-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="c0a17-110">Meie automatiseeritud tööriista kasutamiseks laadige alla ja käivitage **[Microsofti tugi- ja taasteteenuste abiline](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="c0a17-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="c0a17-111">Saate kasutada järgmisi tõrkeotsingu toiminguid.</span><span class="sxs-lookup"><span data-stu-id="c0a17-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="c0a17-112">Avage Office’i rakendus ja [logige](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) kõigist olemasolevatest kasutajakontotest välja.</span><span class="sxs-lookup"><span data-stu-id="c0a17-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="c0a17-113">[Eemaldage](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) Office’i litsents ja [määrake see uuesti](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ning seejärel [logige Office’isse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakontoga sisse.</span><span class="sxs-lookup"><span data-stu-id="c0a17-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="c0a17-114">Käivitage [aktiveerimise tõrkeotsija](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="c0a17-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="c0a17-115">Määrake uuesti Office’i aktiveerimisolek</span><span class="sxs-lookup"><span data-stu-id="c0a17-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office’i aktiveerimisoleku lähtestamine")
- [<span data-ttu-id="c0a17-116">Parandage Office võrgus</span><span class="sxs-lookup"><span data-stu-id="c0a17-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="c0a17-117">Täiendavad tõrkeotsingu lahendused leiate järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="c0a17-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="c0a17-118">Litsentsimata toote ja aktiveerimisega seotud tõrketeated Office’is</span><span class="sxs-lookup"><span data-stu-id="c0a17-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="c0a17-119">Office’i aktiveerimisel kuvatakse tõrketeade: „Kahjuks ei saa teie kontoga ühendust luua. Proovige hiljem uuesti.“</span><span class="sxs-lookup"><span data-stu-id="c0a17-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)