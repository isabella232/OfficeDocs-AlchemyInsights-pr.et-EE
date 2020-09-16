---
title: Yammeri litsentsimise probleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657272"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="e90c1-102">Yammeri litsentsimise probleemid</span><span class="sxs-lookup"><span data-stu-id="e90c1-102">Yammer licensing issues</span></span>

<span data-ttu-id="e90c1-103">Kõigi kasutajate jaoks peab olema litsents Yammeri Enterprise ' i teenuse kasutamiseks, kuid vaikimisi ei nõua Yammeri kasutajatel teenusele juurdepääsuks litsentsi.</span><span class="sxs-lookup"><span data-stu-id="e90c1-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="e90c1-104">Kui administraator muudab sätteid Microsoft 365 kasutajate blokeerimiseks ilma Yammeri litsentsideta, ei saa kasutajad, kellele on määratud Yammeri Enterprise ' i litsents, juurdepääsu Yammeri teenusele.</span><span class="sxs-lookup"><span data-stu-id="e90c1-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="e90c1-105">Lisateavet leiate teemast [Yammeri kasutajate litsentside haldamine Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="e90c1-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="e90c1-106">Kui litsentsid eemaldatakse kasutajatelt, ei kuvata enam Yammeri paani ja muud teenused saavad funktsioonide peitmiseks kasutada litsentside eemaldamist.</span><span class="sxs-lookup"><span data-stu-id="e90c1-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="e90c1-107">Muudel juhtudel saab funktsioone endiselt näha, kuid vaja on kasutada litsentsi määramise funktsiooni.</span><span class="sxs-lookup"><span data-stu-id="e90c1-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="e90c1-108">**Litsentsi ei saa kasutaja jaoks värskendada**</span><span class="sxs-lookup"><span data-stu-id="e90c1-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="e90c1-109">Mõnikord määratakse kasutajale litsents, kuid Yammerile ei pääse endiselt juurde.</span><span class="sxs-lookup"><span data-stu-id="e90c1-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="e90c1-110">Viivitusi esineb suurema tõenäosusega, kui on käimas massmälu määramine.</span><span class="sxs-lookup"><span data-stu-id="e90c1-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="e90c1-111">Yammeri kasutajaid ei pruugita värskendada samas korralduses, nagu litsentsid on Azure AD-s muudetud, kuna süsteem töötab asünkroonselt.</span><span class="sxs-lookup"><span data-stu-id="e90c1-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="e90c1-112">Oodake kuni 24 tundi, enne kui avate tugiteenuse juhtumi, et teatada litsentsi sünkroonimise probleemidest.</span><span class="sxs-lookup"><span data-stu-id="e90c1-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="e90c1-113">**Litsentsi põhiosa määramine**</span><span class="sxs-lookup"><span data-stu-id="e90c1-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="e90c1-114">Litsentse saab määrata administreerimiskeskuse või PowerShelli skriptimise kaudu.</span><span class="sxs-lookup"><span data-stu-id="e90c1-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="e90c1-115">Lisateavet leiate teemast [kasutajatele litsentside määramine](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Office 365 PowerShelli abil kasutajakontodele litsentside määramine](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="e90c1-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="e90c1-116">Microsoft support ei paku skriptide loomisele abi, kuid saadaval on Yammeri litsentsi määramise dokumentatsioon.</span><span class="sxs-lookup"><span data-stu-id="e90c1-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="e90c1-117">Lisateavet leiate teemast [Yammeri litsentside haldamine Windows PowerShelli abil](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="e90c1-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>