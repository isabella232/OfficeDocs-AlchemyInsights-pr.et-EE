---
title: OneDrive for Businessi saitidele juurdepääsu keelamise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670612"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="3c86d-102">OneDrive for Businessi saitidele juurdepääsu keelamise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="3c86d-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="3c86d-103">See probleem ilmneb kõige sagedamini siis, kui kasutaja kustutatakse ja luuakse uuesti sama kasutaja põhinimega (UPN).</span><span class="sxs-lookup"><span data-stu-id="3c86d-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3c86d-104">Uue konto loomisel kasutatakse mõnda muud PUID (passi kordumatu ID).</span><span class="sxs-lookup"><span data-stu-id="3c86d-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3c86d-105">Kui kasutaja proovib juurde pääseda saidikogumile või nende OneDrive ' i, on kasutajal vale PUID.</span><span class="sxs-lookup"><span data-stu-id="3c86d-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3c86d-106">Teine stsenaarium hõlmab kataloogi sünkroonimist Active Directory organisatsiooniüksuse (OU) abil.</span><span class="sxs-lookup"><span data-stu-id="3c86d-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3c86d-107">Kui kasutajad on juba SharePointi sisse loginud ja seejärel teisaldatakse need teise OU ja sünkroonitakse SharePointiga, võivad nad seda probleemi kogeda.</span><span class="sxs-lookup"><span data-stu-id="3c86d-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="3c86d-108">Selle probleemi lahendamiseks peate taastama algse UPN-i artikli juhistega, [taastama kasutaja Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="3c86d-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="3c86d-109">Kui te ei saa algset kasutajat taastada, peate vana kasutaja nende juhiste abil OneDrive ' i saidilt eemaldama, [eemaldage kasutaja kasutaja teabe loendist]().</span><span class="sxs-lookup"><span data-stu-id="3c86d-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="3c86d-110">Kui see on tehtud, saate kontrollida, kas kasutajal on OneDrive ' i saidi administraatori õigused, järgides juhiseid [kasutaja OneDrive ' i jaoks administraatorile lisamiseks](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="3c86d-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="3c86d-111">Lisateavet õiguste tasemete kohta leiate artiklist, [õiguste tasemete mõistmine SharePointis](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="3c86d-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
