---
title: Office ' i rakenduste kinnitamine teie konto on vigane oleku sõnum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969385"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="8e022-102">Office ' i rakenduste kinnitamine "teie konto on vigane olekus"</span><span class="sxs-lookup"><span data-stu-id="8e022-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="8e022-103">Selle tõrke lahendamiseks proovige mõjutatud arvutis järgmisi suvandeid.</span><span class="sxs-lookup"><span data-stu-id="8e022-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="8e022-104">Avage Office ' i rakendus, valige **fail** > **konto** > **Logi välja kõik kontod**.</span><span class="sxs-lookup"><span data-stu-id="8e022-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="8e022-105">Logige uuesti sisse, kasutades sobivat litsentsi kasutajakontot.</span><span class="sxs-lookup"><span data-stu-id="8e022-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="8e022-106">Üksikasjaliku teabe saamiseks vaadake [Office ' i kontosid](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8e022-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8e022-107">[Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.</span><span class="sxs-lookup"><span data-stu-id="8e022-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="8e022-108">**Märkus:** Office 2016 registri teed on muutunud 16,0.</span><span class="sxs-lookup"><span data-stu-id="8e022-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8e022-109">Näiteks \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="8e022-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="8e022-110">Mõjutatud arvuti, seadke EnableADAL = 0, kasutades järgmisi samme:</span><span class="sxs-lookup"><span data-stu-id="8e022-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="8e022-111">Paremklõpsake Windowsi nuppu ja valige **Käivita**.</span><span class="sxs-lookup"><span data-stu-id="8e022-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="8e022-112">Väljale **Ava** tippige **käsk regedit**ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="8e022-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="8e022-113">Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige **Jah** .</span><span class="sxs-lookup"><span data-stu-id="8e022-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="8e022-114">Registriredaktori, lisage DWORD-väärtus EnableADAL sätte 0 all HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="8e022-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="8e022-115">Kui tõrge ilmneb samal ajal Office 365, kasutades Office 2013, [lubage kaasaegne autentimine](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) Office ' i kliendi.</span><span class="sxs-lookup"><span data-stu-id="8e022-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="8e022-116">Lisateabe saamiseks vaadake, [Kuidas teha tõrkeotsingut mitte-brauseri rakendused, mis ei saa sisse logida Office 365, Azure või Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="8e022-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

