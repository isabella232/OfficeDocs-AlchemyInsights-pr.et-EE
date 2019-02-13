---
title: Juurdepääs keelatud töövoo vaatamisel
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918824"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="ddc3c-102">Juurdepääs keelatud töövoo vaatamisel</span><span class="sxs-lookup"><span data-stu-id="ddc3c-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="ddc3c-103">Saatmisel e-posti leviloendiga SharePointi rühm SharePointi 2013 töövoogude ebaõnnestuda kui SharePointi rühma liikmeid ei ole seatud kõigile tõrketeate "Juurdepääs keelatud".</span><span class="sxs-lookup"><span data-stu-id="ddc3c-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="ddc3c-104">**Probleemi lahendamiseks toimige järgmiselt.**</span><span class="sxs-lookup"><span data-stu-id="ddc3c-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="ddc3c-105">Luba SharePointi rühma liikmete vaatamiseks.</span><span class="sxs-lookup"><span data-stu-id="ddc3c-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="ddc3c-106">Eemaldage SharePointi rühm või koopia reale.</span><span class="sxs-lookup"><span data-stu-id="ddc3c-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="ddc3c-107">Kasutajate selgesõnaliselt lisamiseks või koopia kui liikmeks nähtavust ei saa muuta SharePointi rühma.</span><span class="sxs-lookup"><span data-stu-id="ddc3c-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="ddc3c-108">Et näha rohkem üksikasju vt [HTTP volitamata /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ddc3c-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

