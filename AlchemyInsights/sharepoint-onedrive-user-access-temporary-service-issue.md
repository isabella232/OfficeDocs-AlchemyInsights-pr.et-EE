---
title: Jõudluse probleemid-SharePointi või OneDrive'i
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719513"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="e24c7-102">SharePointi või OneDrive aeglane, juurdepääsetav või mitme kasutaja jaoks saadaval</span><span class="sxs-lookup"><span data-stu-id="e24c7-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="e24c7-103">Kui mitmele kasutajale, kellel juurdepääs puudub OneDrive'i või SharePointi saidi, võib teenuse ajutise probleemi.</span><span class="sxs-lookup"><span data-stu-id="e24c7-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="e24c7-104">[Kontrollige teenuste seisundi armatuurlaud](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e24c7-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="e24c7-105">Lisada ja kasutaja litsents</span><span class="sxs-lookup"><span data-stu-id="e24c7-105">Add and license the user</span></span>

<span data-ttu-id="e24c7-106">Tagada, et te [määrama kasutajatele Office 365 Business litsentsid](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="e24c7-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="e24c7-107">Õiguste määramine</span><span class="sxs-lookup"><span data-stu-id="e24c7-107">Assign Permissions</span></span>

<span data-ttu-id="e24c7-108">Kui kasutaja on määratud SharePointi litsentsi ja ikka saab juurdepääsu keelamise teade, siis veenduge, nad on määratud [sobiv õiguste tase](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="e24c7-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="e24c7-109">Võite kasutada funktsiooni juurdepääsu taotluse</span><span class="sxs-lookup"><span data-stu-id="e24c7-109">Consider using the access request feature</span></span>

<span data-ttu-id="e24c7-110">[Juurdepääsu taotluse funktsioon](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) võimaldab inimestel paluda luba sisu, mida nad on praegu õigus näha.</span><span class="sxs-lookup"><span data-stu-id="e24c7-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="e24c7-111">Lubada kohandatud skript võib põhjustada juurdepääs keelatud küsimusi</span><span class="sxs-lookup"><span data-stu-id="e24c7-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="e24c7-112">On teatud stsenaariume, kus *Luba kohandatud skript* funktsiooni võib esitada juurdepääsu keelamise.</span><span class="sxs-lookup"><span data-stu-id="e24c7-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="e24c7-113">Mõjutab funktsioonide, võttes ja võime seda keelata.</span><span class="sxs-lookup"><span data-stu-id="e24c7-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="e24c7-114">Palun külastage [Luba või kohandatud skripti](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e24c7-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

