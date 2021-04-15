---
title: Litsentsimata toote tõrgete lahendamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786845"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="dfcd2-102">Soovitused tõrgete "Litsentsimata toode" lahendamiseks</span><span class="sxs-lookup"><span data-stu-id="dfcd2-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="dfcd2-103">Litsentsimata tootega seotud tõrgete lahendamiseks proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="dfcd2-104">Kontrollige, kas teie tellimuse olek on aegunud.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="dfcd2-105">Veenduge, et teil oleks tellimus, mis lubab kliendilitsentse (nt Microsoft 365 ettevõtterakendused või Business Premium) ja veenduge, et kasutajale [on määratud litsents.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="dfcd2-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="dfcd2-106">Veenduge, et kasutaja logiks Office'i sisse sama kontoga, millele on määratud litsents.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="dfcd2-107">Vaadake lehel [Teenuse seisundist,](https://docs.microsoft.com/office365/enterprise/view-service-health) kas teenusega on teadaolevaid probleeme.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="dfcd2-108">Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Microsoft 365 rakenduste juurdepääsu Internetile.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="dfcd2-109">Vt [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="dfcd2-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="dfcd2-110">Samuti võite proovida järgmisi tõrkeotsingutoiminguid.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="dfcd2-111">Avage Office'i rakendus [ja logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="dfcd2-112">[Eemaldage](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [Office'i litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määrake see uuesti ning logige seejärel mõjutatud kasutajakonto abil [Office'i](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sisse.</span><span class="sxs-lookup"><span data-stu-id="dfcd2-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="dfcd2-113">Käivitage [aktiveerimistõrkeotsija.](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="dfcd2-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="dfcd2-114">[Lähtestage Office'i aktiveerimisolekut](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="dfcd2-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="dfcd2-115">[Parandage Office'i võrgus.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="dfcd2-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="dfcd2-116">Täiendavad tõrkeotsingu lahendused leiate järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="dfcd2-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="dfcd2-117">Litsentsimata toote ja aktiveerimisega seotud tõrketeated Office’is</span><span class="sxs-lookup"><span data-stu-id="dfcd2-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="dfcd2-118">Office’i aktiveerimisel kuvatakse tõrketeade: „Kahjuks ei saa teie kontoga ühendust luua. Proovige hiljem uuesti.“</span><span class="sxs-lookup"><span data-stu-id="dfcd2-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)