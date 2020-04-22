---
title: 902 (dubleeritud objektide tõttu sünkroonimise tõrked)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767115"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="94e8d-102">Sünkroonimise tõrked dubleeritud objektide tõttu</span><span class="sxs-lookup"><span data-stu-id="94e8d-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="94e8d-103">Kui kataloogi sünkroonimine lõpetab Microsoft 365 võidakse kuvada üks järgmistest tõrketeadetest:</span><span class="sxs-lookup"><span data-stu-id="94e8d-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="94e8d-104">Seda objekti ei saa Microsoft Online Services värskendada, kuna järgmised selle objektiga seostatud atribuudid on väärtused, mis võivad juba olla seotud mõne muu objektiga teie kohalikus kataloogis.</span><span class="sxs-lookup"><span data-stu-id="94e8d-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="94e8d-105">Sama puhveraadressiga sünkroonitud objekt on teie Microsoft Online Services kataloogis juba olemas.</span><span class="sxs-lookup"><span data-stu-id="94e8d-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="94e8d-106">Seda objekti ei saa värskendada, kuna järgmised selle objektiga seostatud atribuudid on väärtused, mis võivad juba olla seotud teise objektiga teie kohalikus kataloogiteenustes: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="94e8d-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="94e8d-107">Tuvastamiseks ja probleemi lahendamiseks laadige alla ja käivitage [Idfix DirSync tõrge tervendamise tööriista](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="94e8d-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="94e8d-108">Lisateabe saamiseks vaadake [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="94e8d-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
