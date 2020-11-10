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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982451"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="21a87-102">Loendiüksuste kommentaarid</span><span class="sxs-lookup"><span data-stu-id="21a87-102">Comments on List items</span></span>

<span data-ttu-id="21a87-103">Kasutajad saavad peagi lisada ja kustutada loendiüksuste kommentaare.</span><span class="sxs-lookup"><span data-stu-id="21a87-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="21a87-104">Kasutajad saavad vaadata kõiki loendiüksuse kommentaare ja filtreerida mõne üksusega seotud kommentaare või tegevust kuvavate vaadete vahel.</span><span class="sxs-lookup"><span data-stu-id="21a87-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="21a87-105">**Ajastus** :</span><span class="sxs-lookup"><span data-stu-id="21a87-105">**Timing** :</span></span>

<span data-ttu-id="21a87-106">**Sihipärane väljalase** : järk-järguline väljarullimine oktoobri keskel ja eeldatav lõpp novembri keskpaigaks</span><span class="sxs-lookup"><span data-stu-id="21a87-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="21a87-107">**Standard pressiteade** : järk-järgult rullimine novembri keskel ja eeldatavasti lõpetamine detsembri alguses</span><span class="sxs-lookup"><span data-stu-id="21a87-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="21a87-108">**Levikuga** : kogu ettevõtte jaoks suunatud väljalase</span><span class="sxs-lookup"><span data-stu-id="21a87-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="21a87-109">Enne kommentaaride lisamist ja kustutamist peavad kasutajad arvestama järgmist.</span><span class="sxs-lookup"><span data-stu-id="21a87-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="21a87-110">Kommentaarid järgivad SharePointis omaseid õiguste sätteid.</span><span class="sxs-lookup"><span data-stu-id="21a87-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="21a87-111">Klassikalised loendid, mis pole veel üles ehitatud, et kuvada moodsad kasutajaliidesed (nt tööülesannete loendid), ei avalda seda kommenteerimise funktsiooni.</span><span class="sxs-lookup"><span data-stu-id="21a87-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="21a87-112">Selle väljaandega pole saadaval kommenteerimine võistkondade loendites.</span><span class="sxs-lookup"><span data-stu-id="21a87-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="21a87-113">Kommentaarid pole otsingus indekseeritud.</span><span class="sxs-lookup"><span data-stu-id="21a87-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="21a87-114">Administraatorid saavad selle funktsiooni keelata ettevõtte tasandil, muutes parameetrit **CommentsOnListItemsDisabled** cmdlet **-käsu Set-spotenantiga** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21a87-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="21a87-115">Praegu ei saa saidi või loendi tasemel kommenteerida.</span><span class="sxs-lookup"><span data-stu-id="21a87-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="21a87-116">Loodame, et need juhtelemendid on hilisemas värskenduses, tõenäoliselt esimese kvartali 2021.</span><span class="sxs-lookup"><span data-stu-id="21a87-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
