---
title: Kalendri õigused
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862057"
---
# <a name="calendar-permissions"></a><span data-ttu-id="34ee1-102">Kalendri õigused</span><span class="sxs-lookup"><span data-stu-id="34ee1-102">Calendar Permissions</span></span>

<span data-ttu-id="34ee1-103">Kasutajad saavad muuta oma kalendriõigusi Outlooki veebirakenduse või muude klientidega, kuid administraatorina peate võib-olla uurima ka.</span><span class="sxs-lookup"><span data-stu-id="34ee1-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="34ee1-104">Exchange PowerShelli cmdlet-käsuga kuvatakse kasutaja kalendris olev õigus.</span><span class="sxs-lookup"><span data-stu-id="34ee1-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="34ee1-105">Lisateabe saamiseks vaadake järgmist.</span><span class="sxs-lookup"><span data-stu-id="34ee1-105">To see more information see the following:</span></span>

- [<span data-ttu-id="34ee1-106">Get-MailboxFolderPermission (Get-MailboxFolderPermission)</span><span class="sxs-lookup"><span data-stu-id="34ee1-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="34ee1-107">Set-MailboxFolderPermission (Set-MailboxFolderPermission)</span><span class="sxs-lookup"><span data-stu-id="34ee1-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="34ee1-108">Add-MailboxFolderPermission (Add-MailboxFolderPermission)</span><span class="sxs-lookup"><span data-stu-id="34ee1-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="34ee1-109">Kalendriõigusi kasutatakse kalendrite ühiskasutuses, et näha lisateavet Outlooki kalendri ühiskasutuse kohta, lugege järgmisi artikleid.</span><span class="sxs-lookup"><span data-stu-id="34ee1-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="34ee1-110">Outlooki kalendri ühiskasutus</span><span class="sxs-lookup"><span data-stu-id="34ee1-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="34ee1-111">Kalendri ühiskasutusse andmine Outlooki veebirakenduses ettevõttejaoks</span><span class="sxs-lookup"><span data-stu-id="34ee1-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="34ee1-112">Kalendriõiguste tõrkeotsinguks saate kasutada [tugi- ja taasteabimehe](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tööriista.</span><span class="sxs-lookup"><span data-stu-id="34ee1-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>