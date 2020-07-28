---
title: Mitmel objektil on sama meiliaadress identiteedina
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438931"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="4cc7f-102">Mitmel objektil on sama meiliaadress identiteedina</span><span class="sxs-lookup"><span data-stu-id="4cc7f-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="4cc7f-103">**Mitu objekti**</span><span class="sxs-lookup"><span data-stu-id="4cc7f-103">**Multiple objects**</span></span>

<span data-ttu-id="4cc7f-104">Üks selle tõrke levinumatest põhjustest ei saa Outlook Web Accessi taotlust õigesti marsruutida, kui esineb mitu objekti, millel on sama meiliaadress identiteedina.</span><span class="sxs-lookup"><span data-stu-id="4cc7f-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="4cc7f-105">Nende objektide leidmiseks käivitage järgmised käsud.</span><span class="sxs-lookup"><span data-stu-id="4cc7f-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="4cc7f-106">· Get-adressaat<email address></span><span class="sxs-lookup"><span data-stu-id="4cc7f-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="4cc7f-107">· Get-User<email address></span><span class="sxs-lookup"><span data-stu-id="4cc7f-107">· Get-User <email address></span></span>

<span data-ttu-id="4cc7f-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="4cc7f-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="4cc7f-109">· Get-Contact<email address></span><span class="sxs-lookup"><span data-stu-id="4cc7f-109">· Get-Contact <email address></span></span>

<span data-ttu-id="4cc7f-110">· Hankimine-postkast <email address> – PublicFolder</span><span class="sxs-lookup"><span data-stu-id="4cc7f-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="4cc7f-111">· Hankimine-postkast <email address> – IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="4cc7f-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="4cc7f-112">· Hankimine-postkast <email address> – InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="4cc7f-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="4cc7f-113">Probleemi lahendamiseks eemaldage mitu sama e-posti identiteedi objekti ja veenduge, et kindla meili identiteediga on üks objekt ja selle adressaadi tüüp on UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="4cc7f-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="4cc7f-114">**Sama aadressi kasutatakse nii ärikasutajate kui ka klientide postkastide jaoks**</span><span class="sxs-lookup"><span data-stu-id="4cc7f-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="4cc7f-115">Teine põhjus on see, kui sama aadressi kasutatakse nii ärikasutajate kui ka klientide postkastide jaoks.</span><span class="sxs-lookup"><span data-stu-id="4cc7f-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="4cc7f-116">Sellisel juhul peab kasutaja muutma oma esmase tarbija pseudonüümi, kuni Cafe selle stsenaariumi toetab.</span><span class="sxs-lookup"><span data-stu-id="4cc7f-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="4cc7f-117">See on püsiv viga, mis ei kao ilma sekkumiseta.</span><span class="sxs-lookup"><span data-stu-id="4cc7f-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="4cc7f-118">Lisateavet leiate teemast [Microsofti konto meiliaadressi või telefoninumbri muutmine](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="4cc7f-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>