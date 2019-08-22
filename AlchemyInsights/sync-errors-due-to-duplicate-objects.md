---
title: 902 (sünkroonimise tõrgete tõttu dubleeritud objektid)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507411"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="a6ec1-102">Sünkroonimise tõrgete tõttu dubleeritud objektid</span><span class="sxs-lookup"><span data-stu-id="a6ec1-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="a6ec1-103">Võite saada ühe järgmistest kataloogi sünkroonimise lõpulejõudmisel Office 365:</span><span class="sxs-lookup"><span data-stu-id="a6ec1-103">You might receive one of the following error messages when directory synchronization finishes in Office 365:</span></span>

- <span data-ttu-id="a6ec1-104">Ei saa värskendada selle objekti Microsoft Online Services, sest järgmise seotud objekt on väärtused, mida juba võib olla seotud mõne muu objekti oma kohaliku kataloogis.</span><span class="sxs-lookup"><span data-stu-id="a6ec1-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="a6ec1-105">Microsofti võrguteenuste kataloogi sünkroonitud objekti koos sama meiliaadress on juba olemas.</span><span class="sxs-lookup"><span data-stu-id="a6ec1-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="a6ec1-106">Ei saa värskendada selle objekti, sest järgmised atribuudid, mis on seostatud selle objekti on väärtused, mis võib juba olla seotud teise objekti kohalik directory Services: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a6ec1-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="a6ec1-107">Tuvastada ja lahendada see probleem, alla laadida ja [IdFix DirSync vea parandamise tööriist](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="a6ec1-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="a6ec1-108">Lisateabe saamiseks vt [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="a6ec1-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
