---
title: SharePoint Online ' i saidi loomine
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770419"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="3256d-102">SharePointi saitide loomine mallide abil</span><span class="sxs-lookup"><span data-stu-id="3256d-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="3256d-103">Kaasaegne side-või meeskonnatöö saidid ei toeta saidi mallina salvestamise võimalust.</span><span class="sxs-lookup"><span data-stu-id="3256d-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="3256d-104">Mallide kasutamise kohta lisateabe saamiseks vaadake teemat [salvestamine, allalaadimine ja üleslaadimine SharePointi saidi mallina](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="3256d-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="3256d-105">Siin on mõned levinud probleemid/lahendused saidi või loendi salvestamisel mallina SharePoint Online ' is.</span><span class="sxs-lookup"><span data-stu-id="3256d-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="3256d-106">**Saidi/loendimalli nupu salvestamine pole saadaval või puudub**</span><span class="sxs-lookup"><span data-stu-id="3256d-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="3256d-107">Administraatorid peavad lubama kohandatud skripti malli funktsioonide lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="3256d-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="3256d-108">Üksikasjalikke samme, näiteid ja kaalutlusi vt</span><span class="sxs-lookup"><span data-stu-id="3256d-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="3256d-109">Kohandatud skripti lubamine või vältimine</span><span class="sxs-lookup"><span data-stu-id="3256d-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="3256d-110">Salvesta sait mallina käsk ei toetata ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri Avaldamisinfrastruktuur.</span><span class="sxs-lookup"><span data-stu-id="3256d-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="3256d-111">**Saidimalli ei saa luua või ei tööta õigesti**</span><span class="sxs-lookup"><span data-stu-id="3256d-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="3256d-112">Mallis võib olla [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) puudu ja seda ei aktiveerita.</span><span class="sxs-lookup"><span data-stu-id="3256d-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="3256d-113">Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa saidi loomiseks saidimalli kasutada.</span><span class="sxs-lookup"><span data-stu-id="3256d-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="3256d-114">Kontrollige, et näha, kas loendid või teegid ületavad [loendivaate piirmäära piirmäära](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 üksused, kuna see võib blokeerida saidi malli loomine.</span><span class="sxs-lookup"><span data-stu-id="3256d-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="3256d-115">Sait võib kasutada liiga palju ressursse ja seetõttu saidi Mall ületab 50 MB piirangu.</span><span class="sxs-lookup"><span data-stu-id="3256d-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="3256d-116">On probleeme andmete kuvamisel loendist, mis kasutab Lookup veerg.</span><span class="sxs-lookup"><span data-stu-id="3256d-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="3256d-117">Lisateabe saamiseks vaadake [malli loodud loend ei kuvata andmeid õige Lookup loendi SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="3256d-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="3256d-118">Üksikasjalikuma teabe saamiseks levinud probleemide ja lahenduste kohta kontrollige palun [Loo ja kasuta saidimalle](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="3256d-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



