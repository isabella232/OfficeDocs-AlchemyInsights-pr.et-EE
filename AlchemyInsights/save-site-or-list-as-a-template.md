---
title: Saidi või loendi salvestamine mallina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048720"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="853dd-102">Saidi või loendi salvestamine mallina</span><span class="sxs-lookup"><span data-stu-id="853dd-102">Save site or list as a template</span></span>

<span data-ttu-id="853dd-103">SharePointi saidimallid on eelehitatud määratlused, mis on mõeldud konkreetse ärivajaduse ümber.</span><span class="sxs-lookup"><span data-stu-id="853dd-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="853dd-104">Lisateavet leiate jaotisest [mallide kasutamine erinevat tüüpi SharePointi saitide loomiseks](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="853dd-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="853dd-105">Siin on mõned levinud probleemid/lahendused saidi või loendi salvestamisel mallina SharePoint Online ' is.</span><span class="sxs-lookup"><span data-stu-id="853dd-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="853dd-106">**Saidi/loendimalli nupu salvestamine pole saadaval või puudub**.</span><span class="sxs-lookup"><span data-stu-id="853dd-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="853dd-107">Administraatorid peavad lubama kohandatud skripti malli funktsioonide lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="853dd-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="853dd-108">Üksikasjalikke juhiseid, näiteid ja kaalutlusi vt [kohandatud skripti lubamine või vältimine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="853dd-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="853dd-109">Salvesta sait mallina käsk ei toetata ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri Avaldamisinfrastruktuur.</span><span class="sxs-lookup"><span data-stu-id="853dd-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="853dd-110">**Saidimalli ei saa luua või ei tööta õigesti**</span><span class="sxs-lookup"><span data-stu-id="853dd-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="853dd-111">Mallis võib olla [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) puudu ja seda ei aktiveerita.</span><span class="sxs-lookup"><span data-stu-id="853dd-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="853dd-112">Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa saidi loomiseks saidimalli kasutada.</span><span class="sxs-lookup"><span data-stu-id="853dd-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="853dd-113">Kontrollige, et näha, kas loendid või teegid ületavad [loendivaate piirmäära piirmäära](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 üksused, kuna see võib blokeerida saidi malli loomine.</span><span class="sxs-lookup"><span data-stu-id="853dd-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="853dd-114">Sait võib kasutada liiga palju ressursse ja seetõttu saidi Mall ületab 50 megabaidise (MB) piirang.</span><span class="sxs-lookup"><span data-stu-id="853dd-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="853dd-115">On probleeme andmete kuvamisel loendist, mis kasutab Lookup veerg.</span><span class="sxs-lookup"><span data-stu-id="853dd-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="853dd-116">Lisateabe saamiseks vaadake [malli loodud loend ei kuvata andmeid õige Lookup loendi SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="853dd-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="853dd-117">Üksikasjalikuma teabe saamiseks levinud probleemide ja lahenduste kohta palun viidata, [luua ja kasutada saidimalle](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="853dd-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

