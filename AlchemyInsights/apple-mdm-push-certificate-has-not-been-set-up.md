---
title: Apple MDM push ' i serti pole häälestatud
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
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439013"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="e15f7-102">Apple MDM push ' i serti pole häälestatud</span><span class="sxs-lookup"><span data-stu-id="e15f7-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="e15f7-103">Apple MDM push Certificate (tuntud ka kui Apple push Notification Service (APNS) sert) pole teie tellimuse jaoks konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="e15f7-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="e15f7-104">Kui Apple MDM push Certificate pole konfigureeritud, ei saa te iOS-i ja Mac OS-i seadmeid registreerida ja hallata.</span><span class="sxs-lookup"><span data-stu-id="e15f7-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="e15f7-105">Kui olete serdi lisamiseks Intune ' i lisanud, saavad kasutajad oma iOS-i seadmete registreerimiseks installida ettevõtte portaali rakenduse.</span><span class="sxs-lookup"><span data-stu-id="e15f7-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="e15f7-106">Valige **"Nõustun".**</span><span class="sxs-lookup"><span data-stu-id="e15f7-106">Select **"I agree."**</span></span> <span data-ttu-id="e15f7-107">anda Microsoftile luba andmete saatmiseks Apple ' i.</span><span class="sxs-lookup"><span data-stu-id="e15f7-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="e15f7-108">Valige **Laadi alla oma CSR** -i Intune ' i serdi allkirjastamise taotlus, mis on vajalik Apple MDM push-serdi loomiseks.</span><span class="sxs-lookup"><span data-stu-id="e15f7-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="e15f7-109">Seda faili kasutatakse Apple ' i push Certificates portaalis usalduse suhte serdi taotlemiseks.</span><span class="sxs-lookup"><span data-stu-id="e15f7-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="e15f7-110">Klõpsake nuppu **Loo MDM-push** ' i sert, et minna Apple Pushi sertide portaali.</span><span class="sxs-lookup"><span data-stu-id="e15f7-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="e15f7-111">Logige sisse oma ettevõtte Apple ID-ga ja seejärel valige **Loo sert**.</span><span class="sxs-lookup"><span data-stu-id="e15f7-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="e15f7-112">Valige Vali **pilt**, sirvige serdi allkirjastamise taotluse failini ja seejärel klõpsake käsku **Laadi üles**.</span><span class="sxs-lookup"><span data-stu-id="e15f7-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="e15f7-113">Serdi (. PEM) faili allalaadimiseks klõpsake lehel kinnitus nuppu **Laadi alla** ja salvestage faili kohalikult.</span><span class="sxs-lookup"><span data-stu-id="e15f7-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="e15f7-114">**Märkus**: sert on seotud selle loomiseks kasutatava Apple ID-ga.</span><span class="sxs-lookup"><span data-stu-id="e15f7-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="e15f7-115">Parima tavana Kasuta ettevõtte Apple ID-ga haldustoiminguid ja veenduge, et postkasti jälgitakse rohkem kui ühe isiku või leviloendi abil.</span><span class="sxs-lookup"><span data-stu-id="e15f7-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="e15f7-116">Ära kasuta isikliku Apple ' i ID-ga.</span><span class="sxs-lookup"><span data-stu-id="e15f7-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="e15f7-117">Apple Pushi serdi uuendamiseks iga 12 kuu järel kasutage sama Apple ' i ID-ga.</span><span class="sxs-lookup"><span data-stu-id="e15f7-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="e15f7-118">Apple MDM push ' i serdi loomiseks kasutatava Apple ' i ID sisestamine.</span><span class="sxs-lookup"><span data-stu-id="e15f7-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="e15f7-119">Registreerige see ID meeldetuletuseks, kui teil on vaja serti uuendada.</span><span class="sxs-lookup"><span data-stu-id="e15f7-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="e15f7-120">Avage faili sert (. PEM), valige **Ava**ja seejärel klõpsake nuppu **Laadi üles**.</span><span class="sxs-lookup"><span data-stu-id="e15f7-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="e15f7-121">Push Certificate abil saab Intune ' i registreeruda ja hallata Apple ' i seadmeid.</span><span class="sxs-lookup"><span data-stu-id="e15f7-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>