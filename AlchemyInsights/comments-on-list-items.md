---
title: Loendiüksuste kommentaarid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724150"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="6c822-102">Loendiüksuste kommentaarid</span><span class="sxs-lookup"><span data-stu-id="6c822-102">Comments on List items</span></span>

<span data-ttu-id="6c822-103">Kasutajad saavad vaadata kõiki loendiüksuse kommentaare ja filtreerida mõne üksusega seotud kommentaare või tegevust kuvavate vaadete vahel.</span><span class="sxs-lookup"><span data-stu-id="6c822-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="6c822-104">Enne kommentaaride lisamist ja kustutamist peavad kasutajad arvestama järgmist.</span><span class="sxs-lookup"><span data-stu-id="6c822-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="6c822-105">Kommentaarid järgivad SharePointis omaseid õiguste sätteid.</span><span class="sxs-lookup"><span data-stu-id="6c822-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="6c822-106">Klassikalised loendid, mis pole veel üles ehitatud, et kuvada moodsad kasutajaliidesed (nt tööülesannete loendid), ei avalda seda kommenteerimise funktsiooni.</span><span class="sxs-lookup"><span data-stu-id="6c822-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="6c822-107">Selle väljaandega pole saadaval kommenteerimine võistkondade loendites.</span><span class="sxs-lookup"><span data-stu-id="6c822-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="6c822-108">Kommentaarid pole otsingus indekseeritud.</span><span class="sxs-lookup"><span data-stu-id="6c822-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="6c822-109">Administraatorid saavad selle funktsiooni keelata ettevõtte tasandil, muutes parameetrit **CommentsOnListItemsDisabled** cmdlet **-käsu Set-spotenantiga** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6c822-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="6c822-110">Praegu ei saa saidi või loendi tasemel kommenteerida.</span><span class="sxs-lookup"><span data-stu-id="6c822-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="6c822-111">Loodame, et need juhtelemendid on hilisemas värskenduses, tõenäoliselt esimese kvartali 2021.</span><span class="sxs-lookup"><span data-stu-id="6c822-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
