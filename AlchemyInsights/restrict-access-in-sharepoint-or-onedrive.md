---
title: Juurdepääsu piiramine SharePointis või OneDrive ' is
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720678"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="88256-102">Juurdepääsu piiramine SharePointis või OneDrive ' is</span><span class="sxs-lookup"><span data-stu-id="88256-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="88256-103">SharePointis ja OneDrive ' is saate piirata juurdepääsu üksustele (nt failid, kaustad ja loendid), andes juurdepääsu ainult rühmadele või isikutele, kellele soovite juurde pääseda.</span><span class="sxs-lookup"><span data-stu-id="88256-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="88256-104">Vaikimisi pärivad SharePointis olevad õiguste hierarhiast kõrgemad.</span><span class="sxs-lookup"><span data-stu-id="88256-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="88256-105">Seega pärib faili kaustast oma juurdepääsuõigused, mis pärib teegist teegis olevad teegid, mis pärib saidilt selle õiguste.</span><span class="sxs-lookup"><span data-stu-id="88256-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="88256-106">Saate ühiskasutusse anda kõrgemal tasemel (nt kogu saidi ühiskasutusse andmise kaudu) ja seejärel katkestada pärandi, kui te ei soovi kõiki saidil olevaid üksusi ühiskasutusse anda.</span><span class="sxs-lookup"><span data-stu-id="88256-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="88256-107">Kuid me ei soovita seda, sest see muudab paremate ja segavate lubade säilitamise tulevikus.</span><span class="sxs-lookup"><span data-stu-id="88256-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="88256-108">Selle asemel saate teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="88256-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="88256-109">Kui soovite näiteks ühiskasutada kausta kogu sisu, välja arvatud üks fail, teisaldage see fail uude asukohta, mida pole ühiskasutusse antud.</span><span class="sxs-lookup"><span data-stu-id="88256-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="88256-110">Kui teil on kaustas kaks alamkausta ja soovite jagada ühe alamkausta rühmadega A ja B ning lubada ainult rühmale juurdepääsu teise alamkausta, Jagage emakausta rühmaga A ja lisage rühm B esimesse alamkausta.</span><span class="sxs-lookup"><span data-stu-id="88256-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="88256-111">Faili või kausta ühiskasutuse peatamine </span><span class="sxs-lookup"><span data-stu-id="88256-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

