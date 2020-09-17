---
title: Office ' i fail topeltklõpsamisel ei avane
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812075"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="9e5c6-102">Office ' i fail topeltklõpsamisel ei avane</span><span class="sxs-lookup"><span data-stu-id="9e5c6-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="9e5c6-103">Pärast Office ' i failis topeltklõpsamist võidakse kuvada programm avatuna, kuid see ei avane.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="9e5c6-104">Samuti võidakse kuvada tõrketeade: "programmile käsu saatmisel ilmnes probleem."</span><span class="sxs-lookup"><span data-stu-id="9e5c6-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="9e5c6-105">Selleks on mitu põhjust, kuid kaks levinumat lahendust on järgmised.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="9e5c6-106">Veenduge, et Excelis oleks suvand DDE märkimata.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="9e5c6-107">Selle suvandi leiate uue töövihiku loomise teel ja seejärel valige **fail > suvandid > täpsemalt**.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="9e5c6-108">Tühjendage jaotises **Üldine** ruut **Ignoreeri muid rakendusi, mis kasutavad dünaamilist andmevahetust (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="9e5c6-109">Vaikesätete taastamiseks käivitage veebipõhine parandus.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="9e5c6-110">Klõpsake Windowsi nuppu Start ja otsige märksõna "Juhtpaneel".</span><span class="sxs-lookup"><span data-stu-id="9e5c6-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="9e5c6-111">Avage **Juhtpaneel**ja valige programmid **> programmid ja funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="9e5c6-112">Seejärel paremklõpsake valikut **Microsoft Office [versioon]** ja valige **Muuda > online**' i parandamine.</span><span class="sxs-lookup"><span data-stu-id="9e5c6-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="9e5c6-113">Kui kumbki neist lahendustest ei toimi, leiate tugiteenuste artiklist lahenduste täiuslikuma loendi, kui [topeltklõpsate Office ' i faili, ei saa seda avada](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="9e5c6-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
