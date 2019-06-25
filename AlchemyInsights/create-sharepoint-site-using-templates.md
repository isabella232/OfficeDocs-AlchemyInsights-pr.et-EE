---
title: Luua saidi SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199269"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="77eeb-102">Luua SharePointi saitide abil</span><span class="sxs-lookup"><span data-stu-id="77eeb-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="77eeb-103">SharePointi saidi templates on mõeldud ärivaldkonnas vaja umbes Varemkoostatud mõisted.</span><span class="sxs-lookup"><span data-stu-id="77eeb-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="77eeb-104">Lisateabe saamiseks vt [kasutamine malle luua erinevat tüüpi SharePointi saitidele](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="77eeb-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="77eeb-105">Siin on mõned ühised probleemid/lahendusi seoses salvestamine on saidi- või mallina Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="77eeb-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="77eeb-106">**Salvesta saidilt/sellest loendist malli nupp ei ole saadaval või puudub**</span><span class="sxs-lookup"><span data-stu-id="77eeb-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="77eeb-107">Administraatorid tuleb lubada kohandatud skripti malli funktsioonide lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="77eeb-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="77eeb-108">Üksikasjalikud näited ja kaalutluste kohta leiate</span><span class="sxs-lookup"><span data-stu-id="77eeb-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="77eeb-109">Või mitte kohandatud skripti</span><span class="sxs-lookup"><span data-stu-id="77eeb-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="77eeb-110">Salvesta saidi malli käsku ei toetata ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri Publishing infrastruktuuri.</span><span class="sxs-lookup"><span data-stu-id="77eeb-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="77eeb-111">**Saidimalli ei saa luua või ei tööta õigesti**</span><span class="sxs-lookup"><span data-stu-id="77eeb-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="77eeb-112">Malli võib puududa [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ja ei Aktiveeri.</span><span class="sxs-lookup"><span data-stu-id="77eeb-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="77eeb-113">Kui funktsioon ei ole saadaval praeguses saidikogumis aktiveerida, ei saa saidimalli abil saidi loomine.</span><span class="sxs-lookup"><span data-stu-id="77eeb-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="77eeb-114">Kontrollige, kui loendeid ja teeke ületab [Loendivaateläve piir](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 üksust, kuna see võib takistada saidi malli loomine.</span><span class="sxs-lookup"><span data-stu-id="77eeb-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="77eeb-115">Sait kasutab liiga palju ressursse ja seega saidi malli ületab 50 MB.</span><span class="sxs-lookup"><span data-stu-id="77eeb-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="77eeb-116">On probleeme, mis kasutab otsinguveeru andmed kuvatud.</span><span class="sxs-lookup"><span data-stu-id="77eeb-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="77eeb-117">Lisateabe saamiseks vt [mall loodud loendis ei kuvata SharePoint Online õige otsinguloendis andmeid](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="77eeb-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="77eeb-118">Täpsemat infot üldlevinud probleeme ja lahendusi, Palun kontrollige [saidimallide loomine ja kasutamine](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="77eeb-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



