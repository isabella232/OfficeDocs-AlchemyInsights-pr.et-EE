---
title: 902 (vigade sünkroonimine dubleeritud objektide tõttu)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737337"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="4584c-102">Vigade sünkroonimine dubleeritud objektide tõttu</span><span class="sxs-lookup"><span data-stu-id="4584c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="4584c-103">Kui kataloogi sünkroonimine Microsoft 365 lõpeb, võidakse kuvada mõni järgmistest tõrketeadetest.</span><span class="sxs-lookup"><span data-stu-id="4584c-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="4584c-104">Microsoft Online Services ei saa seda objekti värskendada, kuna selle objektiga seotud järgmistele atribuutidele on lisatud väärtused, mis võivad juba olla seotud mõne muu kohalikus kataloogis oleva objektiga.</span><span class="sxs-lookup"><span data-stu-id="4584c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="4584c-105">Teie Microsoft Online Services kataloogis on sama puhverserveri aadressiga sünkroonitud objekt juba olemas.</span><span class="sxs-lookup"><span data-stu-id="4584c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="4584c-106">Seda objekti ei saa värskendada, sest järgmised selle objektiga seostuvad atribuudid sisaldavad väärtusi, mis võivad juba olla seotud mõne muu kohaliku kataloogiteenuse objektiga: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4584c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="4584c-107">Probleemi tuvastamiseks ja lahendamiseks laadige alla ja käivitage [IdFix Dirsynci tõrke parandamise tööriist](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="4584c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="4584c-108">Lisateavet leiate teemast [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="4584c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
