---
title: Organisatsiooni globaalse aadressiloendi ja ühenduseta aadressiraamatu haldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022436"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="1a051-102">Organisatsiooni globaalse aadressiloendi (GAL) ja ühenduseta aadressiraamatu (OAB) haldamine</span><span class="sxs-lookup"><span data-stu-id="1a051-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="1a051-103">Globaalne aadressiloend (GAL) on organisatsiooni meililoaga objektide loend (mis tahes adressaadi tüüp, mis saab meilisõnumeid vastu võtta).</span><span class="sxs-lookup"><span data-stu-id="1a051-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="1a051-104">Igas organisatsioonis luuakse üks GAL automaatselt.</span><span class="sxs-lookup"><span data-stu-id="1a051-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="1a051-105">Saate luua täiendavaid GAL-e, et eraldada kasutajad organisatsiooni või asukoha järgi, kuid üks kasutaja saab korraga kasutada ja kuvada ühte GAL-i.</span><span class="sxs-lookup"><span data-stu-id="1a051-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="1a051-106">Osad meilikliendid (nt Windowsi Outlook) laadivad GAL-i võrguühenduseta kasutamiseks alla.</span><span class="sxs-lookup"><span data-stu-id="1a051-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="1a051-107">Seda tuntakse ühenduseta aadressiraamatuna (OAB).</span><span class="sxs-lookup"><span data-stu-id="1a051-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="1a051-108">Exchange Online’is värskendatakse OAB ainult üks kord 8 tunni jooksul ja kliendid peavad selle siis alla laadima, et värskendada oma kohalikku OAB eksemplari.</span><span class="sxs-lookup"><span data-stu-id="1a051-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="1a051-109">Kõik saajate muudatused peavad esmalt olema nähtavad GAL-is, et hiljem jõuda OAB-sse.</span><span class="sxs-lookup"><span data-stu-id="1a051-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="1a051-110">Siin on mõned sagedamini kasutatavad GAL-i ja OAB toimingud.</span><span class="sxs-lookup"><span data-stu-id="1a051-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="1a051-111">Erinevatel põhjustel võite tahta osad objektid GAL-is peita.</span><span class="sxs-lookup"><span data-stu-id="1a051-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="1a051-112">Vaadake teemat [Saajate peitmine aadressiloendites](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="1a051-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="1a051-113">Kui soovite anda konkreetsetele kasutajagruppidele organisatsiooni GAL-i kohandatud vaate, vaadake teemat [Exchange Online’i aadressiraamatu poliitikad](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="1a051-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="1a051-114">[Looge Exchange Online’is globaalne aadressiloend](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) ja vaadake teavet GAL-i lubadega töötamise kohta teemast [Exchange Online’i aadressiloendid](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="1a051-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="1a051-115">Arvestage sellega, et kui loote uue GAL-i, võite soovida tahta ka luua OAB.</span><span class="sxs-lookup"><span data-stu-id="1a051-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="1a051-116">Vaadake teemat [Ühenduseta aadressiraamatu toimingud](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="1a051-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
