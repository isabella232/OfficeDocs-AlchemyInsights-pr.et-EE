---
title: Yammeri litsentsimise probleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148236"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="a9bd5-102">Yammeri litsentsimise probleemid</span><span class="sxs-lookup"><span data-stu-id="a9bd5-102">Yammer licensing issues</span></span>

<span data-ttu-id="a9bd5-103">Kõigil kasutajatel peab olema Yammer Enterprise'i teenuse kasutamiseks litsents, kuid vaikimisi ei nõua Yammer, et kasutajatel oleks teenusele juurdepääsuks litsents.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="a9bd5-104">Kui administraator muudab sätet, et blokeerida Microsoft 365 kasutajad ilma Yammeri litsentsideta, ei pääse Yammeri teenusele juurde kasutajad, kellele pole Yammerenterprise'i litsentsi määratud.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="a9bd5-105">Lisateavet leiate teemast [Yammeri kasutajalitsentside haldamine teenusekomplektis Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="a9bd5-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="a9bd5-106">Kui litsentsid eemaldatakse kasutajatelt, ei kuvata enam Yammeri paani ja muud teenused saavad funktsioonide peitmiseks kasutada litsentsi eemaldamist.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="a9bd5-107">Muudel juhtudel võivad funktsioonid siiski ilmuda, kuid nõuavad litsentsi määramist.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="a9bd5-108">**Litsentsi ei värskendata kasutaja jaoks**</span><span class="sxs-lookup"><span data-stu-id="a9bd5-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="a9bd5-109">Aeg-ajalt määratakse kasutajale litsents, kuid ei pääse endiselt Yammerile juurde.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="a9bd5-110">Viivitused on tõenäolisem, kui mass litsentsi määramine on pooleli.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="a9bd5-111">Yammeri kasutajaid ei pruugita värskendada samas järjekorras, kuna litsentse muudetakse Azure AD-s, kuna süsteem töötab asünkroonselt.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="a9bd5-112">Oodake kuni 24 tundi enne tugiteenuse juhtumi avamist, et teatada litsentsi sünkroonimisprobleemidest.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="a9bd5-113">**Hulgilitsentsi määramine**</span><span class="sxs-lookup"><span data-stu-id="a9bd5-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="a9bd5-114">Litsentse saab määrata halduskeskuse või PowerShelli skriptimise kaudu.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="a9bd5-115">Lisateavet leiate teemast [Kasutajatele litsentside määramine](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Kasutajakontodele litsentside määramine Office 365 PowerShelli abil.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="a9bd5-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="a9bd5-116">Microsofti tugiteenus ei paku abi skriptide loomisel, kuid Yammeri litsentsi määramise dokumentatsioon on saadaval.</span><span class="sxs-lookup"><span data-stu-id="a9bd5-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="a9bd5-117">Lisateavet leiate teemast [Yammeri litsentside haldamine Windows PowerShelli abil](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="a9bd5-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>