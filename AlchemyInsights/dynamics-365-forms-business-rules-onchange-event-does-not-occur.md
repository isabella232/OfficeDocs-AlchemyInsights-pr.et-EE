---
title: Dynamics 365 vormide ärireeglid-Business reegel ei tulista vormi
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529015"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="3cd17-102">OnChange sündmus ei esine, kui välja on muudetud programmiliselt</span><span class="sxs-lookup"><span data-stu-id="3cd17-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="3cd17-103">*OnChange* sündmus ei esine, kui välja on muudetud programmiliselt *atribuudi abil.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) meetod.</span><span class="sxs-lookup"><span data-stu-id="3cd17-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="3cd17-104">Kui soovite sündmuseohjurid *OnChange* sündmuse käivitamiseks pärast seda, kui seate väärtus tuleb kasutada *formcontext. Data. olemi atribuut.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) meetod oma koodi.</span><span class="sxs-lookup"><span data-stu-id="3cd17-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
