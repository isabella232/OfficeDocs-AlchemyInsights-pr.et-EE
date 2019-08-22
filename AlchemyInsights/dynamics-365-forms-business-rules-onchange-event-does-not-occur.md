---
title: Dynamics 365 moodustab Ärireeglite - Business reegel ei süütamise vormi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529015"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="3bd6f-102">OnChange sündmuse ilmneda juhul, kui välja muudetakse programmiliselt</span><span class="sxs-lookup"><span data-stu-id="3bd6f-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="3bd6f-103">*OnChange* sündmuse ilmneda juhul, kui välja muudetakse programmiliselt kasutades selle *atribuut.* [Sea_väärtus](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) meetod.</span><span class="sxs-lookup"><span data-stu-id="3bd6f-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="3bd6f-104">Kas sündmuseohjureid *OnChange* sündmus pärast seate kasutage selle *atribuut formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) meetod koodi.</span><span class="sxs-lookup"><span data-stu-id="3bd6f-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
