---
title: Saidi loomine SharePoint Online ' is
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732215"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="82e4e-102">SharePointi saitide loomine mallide abil</span><span class="sxs-lookup"><span data-stu-id="82e4e-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="82e4e-103">Saidi salvestamine mallina pole toetatud moodsa suhtluse või meeskonnatöö saitidega.</span><span class="sxs-lookup"><span data-stu-id="82e4e-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="82e4e-104">Lisateavet mallide kasutamise kohta leiate teemast [SharePointi saidi salvestamine, allalaadimine ja üleslaadimine mallina](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="82e4e-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="82e4e-105">Siin on mõned levinud probleemid/lahendused seoses saidi või loendi salvestamisega mallina SharePoint Online ' is.</span><span class="sxs-lookup"><span data-stu-id="82e4e-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="82e4e-106">**Nupp Salvesta saidi/loendi Mall pole saadaval või puudub**</span><span class="sxs-lookup"><span data-stu-id="82e4e-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="82e4e-107">Administraatorid peavad lubama kohandatud skripti malli funktsioonide lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="82e4e-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="82e4e-108">Üksikasjalikud juhised leiate teemast näited ja kaalutlused</span><span class="sxs-lookup"><span data-stu-id="82e4e-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="82e4e-109">Kohandatud skripti lubamine või keelamine</span><span class="sxs-lookup"><span data-stu-id="82e4e-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="82e4e-110">Käsk Salvesta sait mallina pole toetatud ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri avaldamise infrastruktuuri.</span><span class="sxs-lookup"><span data-stu-id="82e4e-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="82e4e-111">**Saidimalli ei saa luua või see ei tööta õigesti**</span><span class="sxs-lookup"><span data-stu-id="82e4e-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="82e4e-112">Mallil võib olla [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) puudu ja see ei aktiveeru.</span><span class="sxs-lookup"><span data-stu-id="82e4e-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="82e4e-113">Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa te saiti saidi loomiseks kasutada.</span><span class="sxs-lookup"><span data-stu-id="82e4e-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="82e4e-114">Saate vaadata, kas loendid või teegid ületavad 5000 üksuste [loendivaate](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) piirmäära, kuna see võib saidi malli loomist blokeerida.</span><span class="sxs-lookup"><span data-stu-id="82e4e-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="82e4e-115">Sait võib kasutada liiga palju ressursse ja seetõttu ületab saidimall 50 MB piiri.</span><span class="sxs-lookup"><span data-stu-id="82e4e-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="82e4e-116">On probleeme, mis kuvavad andmeid otsinguveeru kasutavast loendist.</span><span class="sxs-lookup"><span data-stu-id="82e4e-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="82e4e-117">Lisateavet leiate teemast [mallide põhjal loodud loend ei kuva SharePoint Online ' is õigete otsinguväljade andmeid](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="82e4e-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="82e4e-118">Üksikasjalikumat teavet levinud probleemide ja lahenduste kohta leiate teemast [saidimallide loomine ja kasutamine](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="82e4e-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



