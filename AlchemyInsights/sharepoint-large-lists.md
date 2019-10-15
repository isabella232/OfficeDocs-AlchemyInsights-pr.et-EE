---
title: SharePointi suured loendid
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488513"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="1af56-102">Suur loendid ja teegid SharePointi töö</span><span class="sxs-lookup"><span data-stu-id="1af56-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="1af56-103">SharePointi loendid ja teegid võivad sisaldada kuni 30 000 000 üksust, kuid kui neil on rohkem kui 5 000 üksust, võidakse kuvada loendivaate läve tõrge, kui proovite nendega töötada.</span><span class="sxs-lookup"><span data-stu-id="1af56-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="1af56-104">See künnis on kehtestatud teenuse toimivuse säilitamiseks.</span><span class="sxs-lookup"><span data-stu-id="1af56-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="1af56-105">Seda ei saa muuta.</span><span class="sxs-lookup"><span data-stu-id="1af56-105">It can't be changed.</span></span> <span data-ttu-id="1af56-106">Et vältida selle piirmäära lööb:</span><span class="sxs-lookup"><span data-stu-id="1af56-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="1af56-107">**Kasuta kaasaegseid**</span><span class="sxs-lookup"><span data-stu-id="1af56-107">**Use modern**</span></span>

<span data-ttu-id="1af56-108">Tänapäevastes kogemustel kõige paremini toimivad vaated, mis näitavad paljusid esemeid.</span><span class="sxs-lookup"><span data-stu-id="1af56-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="1af56-109">[Kasutage kaasaegset kogemust](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , et vältida vigu, mida võite näha klassikalises kogemusega.</span><span class="sxs-lookup"><span data-stu-id="1af56-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="1af56-110">**Registrite lisamine**</span><span class="sxs-lookup"><span data-stu-id="1af56-110">**Add indexes**</span></span>

<span data-ttu-id="1af56-111">Kui filtreerige või Sortige veergu, millel pole indeksit, võidakse kuvada veateade.</span><span class="sxs-lookup"><span data-stu-id="1af56-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="1af56-112">[Lisage indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) käsitsi sätete menüüst **loendist sätted** ja seejärel **Indekseeritud veerud**.</span><span class="sxs-lookup"><span data-stu-id="1af56-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="1af56-113">**Loendivaate redigeerimine**</span><span class="sxs-lookup"><span data-stu-id="1af56-113">**Edit the list view**</span></span>

<span data-ttu-id="1af56-114">Kui suure loendiga töötamisel ilmneb tõrge, [redigeerige loendivaadet](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="1af56-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="1af56-115">Järgmised neli muudatust eemaldab loendivaate läve tõrked.</span><span class="sxs-lookup"><span data-stu-id="1af56-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="1af56-116">Kõigi tõrgete eemaldamiseks tehke kõik neli muudatust.</span><span class="sxs-lookup"><span data-stu-id="1af56-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="1af56-117">Kui teil on endiselt tõrkeid, kontrollige [Halda suuri loendeid ja teegid](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="1af56-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="1af56-118">Valige **mitte ükski** **esimesest sordist veeru järgi** ja **seejärel Sortige veeru järgi**.</span><span class="sxs-lookup"><span data-stu-id="1af56-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="1af56-119">Valige **veeru järgi esimesest rühmast** **mitte ükski** ja **seejärel Rühmita veeru järgi**.</span><span class="sxs-lookup"><span data-stu-id="1af56-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="1af56-120">Valige **pole** kõigi veergude jaotises **kogusummad** .</span><span class="sxs-lookup"><span data-stu-id="1af56-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="1af56-121">Tühistage kõik **veerud jaotises veergude** kuvamiseks.</span><span class="sxs-lookup"><span data-stu-id="1af56-121">Deselect all but one column for display from the **Columns** section.</span></span>

