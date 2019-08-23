---
title: Saidi või loendi salvestada mallina
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551627"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="e5a6b-102">Saidi või loendi salvestada mallina</span><span class="sxs-lookup"><span data-stu-id="e5a6b-102">Save site or list as a template</span></span>

<span data-ttu-id="e5a6b-103">SharePointi saidi templates on mõeldud ärivaldkonnas vaja umbes Varemkoostatud mõisted.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="e5a6b-104">Lisateabe saamiseks vt [kasutamine malle luua erinevat tüüpi SharePointi saitidele](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="e5a6b-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="e5a6b-105">Siin on mõned ühised probleemid/lahendusi seoses salvestamine on saidi- või mallina SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="e5a6b-106">**Saidilt/sellest loendist Salvesta Mall nupp ei ole olemas või puudub**.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="e5a6b-107">Administraatorid tuleb lubada kohandatud skripti malli funktsioonide lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="e5a6b-108">Leiate täpsed juhised, näidised ja arvestamine [Luba või kohandatud skripti](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e5a6b-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="e5a6b-109">Salvesta saidi malli käsku ei toetata ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri Publishing infrastruktuuri.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="e5a6b-110">**Saidimalli ei saa luua või ei tööta õigesti**</span><span class="sxs-lookup"><span data-stu-id="e5a6b-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="e5a6b-111">Malli võib puududa [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ja ei Aktiveeri.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="e5a6b-112">Kui funktsioon ei ole saadaval praeguses saidikogumis aktiveerida, ei saa saidimalli abil saidi loomine.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="e5a6b-113">Kontrollige, kui loendeid ja teeke ületab [Loendivaateläve piir](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 üksust, kuna see võib takistada saidi malli loomine.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="e5a6b-114">Sait kasutab liiga palju ressursse ja seega saidi malli ületab 50 megabaidi (MB).</span><span class="sxs-lookup"><span data-stu-id="e5a6b-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="e5a6b-115">On probleeme, mis kasutab otsinguveeru andmed kuvatud.</span><span class="sxs-lookup"><span data-stu-id="e5a6b-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="e5a6b-116">Lisateabe saamiseks vt [mall loodud loendis ei kuvata SharePoint Online õige otsinguloendis andmeid](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="e5a6b-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="e5a6b-117">Üksikasjalikumat teavet ühiste probleemide ja lahenduste palun viidet, [saidimallide loomine ja kasutamine](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="e5a6b-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

