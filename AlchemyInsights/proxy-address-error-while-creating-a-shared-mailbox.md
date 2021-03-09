---
title: Puhverserveri aadressi tõrge ühiskasutatava postkasti loomisel
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568286"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="96fc1-102">Puhverserveri aadressi tõrge postkasti või muu meili lubatud objekti loomisel</span><span class="sxs-lookup"><span data-stu-id="96fc1-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="96fc1-103">Kui proovisite luua e-posti loaga objekti (postkast, ühiskasutuses postkast jne) ja sai tõrketeate "puhverserveri aadress" SMTP:alias@domain.com "on juba kasutusel...", on teie valitud meiliaadress juba mõne muu teie asutuse jaoks loodud e-posti toega objekt.</span><span class="sxs-lookup"><span data-stu-id="96fc1-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="96fc1-104">Peate leidma kasutaja, rühma, ühiskasutatava postkasti või ühiskausta, millel on see meiliaadress, ja kustutama või muutma selle meiliaadressi.</span><span class="sxs-lookup"><span data-stu-id="96fc1-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="96fc1-105">Siis saad luua uue e-posti toega objekti koos vabanenud meiliaadressiga.</span><span class="sxs-lookup"><span data-stu-id="96fc1-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="96fc1-106">Selle leidmiseks kasutage avalehel otsingut.</span><span class="sxs-lookup"><span data-stu-id="96fc1-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="96fc1-107">Selle otsimiseks saate kasutada ka järgmist Exchange Online PowerShelli käsku.</span><span class="sxs-lookup"><span data-stu-id="96fc1-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="96fc1-108">Kui te ei soovi olemasolevat meiliaadressi kustutada, valige loodava uue objekti jaoks uus meiliaadress.</span><span class="sxs-lookup"><span data-stu-id="96fc1-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  