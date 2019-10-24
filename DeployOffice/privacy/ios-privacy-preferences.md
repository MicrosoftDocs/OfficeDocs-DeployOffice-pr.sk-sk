---
title: Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb
ms.author: danbrown
author: pbowden-msft
manager: laurawi
audience: ITPro
ms.topic: article
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
- Ent_Office_Mac
description: V tomto článku správcovia služieb Office získajú informácie o postupoch spravovania nastavení ochrany osobných údajov v zariadeniach so systémom iOS.
hideEdit: true
ms.openlocfilehash: d1a14d2e1bfe45710255467fcbce9ac4af2c9cb7
ms.sourcegitcommit: 903d6bac7d8b7d8003863ac778c0b5bbdfa7a62a
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/21/2019
ms.locfileid: "37604298"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="84d62-103">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb</span><span class="sxs-lookup"><span data-stu-id="84d62-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

<span data-ttu-id="84d62-104">K dispozícii sú nové nastavenia predvolieb pre Office v zariadeniach so systémom iOS, ktoré umožňujú ovládať nastavenia pre:</span><span class="sxs-lookup"><span data-stu-id="84d62-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="84d62-105">***Diagnostické údaje***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.</span><span class="sxs-lookup"><span data-stu-id="84d62-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="84d62-106">***Online funkcie***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.</span><span class="sxs-lookup"><span data-stu-id="84d62-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="84d62-107">Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="84d62-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="84d62-108">Tieto nastavenia predvolieb sa týkajú aplikácií:</span><span class="sxs-lookup"><span data-stu-id="84d62-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="84d62-109">Word pre iOS, Excel pre iOS a PowerPoint pre iOS verzie 2.30 a novšej.</span><span class="sxs-lookup"><span data-stu-id="84d62-109">Version 2.30 and later of Word for iOS, Excel for iOS, and PowerPoint for iOS.</span></span>
- <span data-ttu-id="84d62-110">OneNote pre iOS verzie 16.30 a novšej.</span><span class="sxs-lookup"><span data-stu-id="84d62-110">Version 16.30 and later of OneNote for iOS.</span></span>
- <span data-ttu-id="84d62-111">Visio Viewer pre iOS verzie 1.17 a novšej.</span><span class="sxs-lookup"><span data-stu-id="84d62-111">Version 1.17 and later of Visio Viewer for iOS.</span></span>

> [!NOTE]
> <span data-ttu-id="84d62-112">Ďalšie informácie o podobných nastaveniach balíka Office v počítačoch so systémom macOS nájdete v téme [Spravovanie ovládacích prvkov ochrany osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="84d62-112">For information about similar settings for Office on computers running Windows, see [Use policy settings to manage privacy controls for Office 365 ProPlus](mac-privacy-preferences.md).</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="84d62-113">Nastavenie predvolieb zariadenia</span><span class="sxs-lookup"><span data-stu-id="84d62-113">Setting device preferences</span></span>
<span data-ttu-id="84d62-114">Tieto nové nastavenia predvolieb je možné nastaviť aj na úrovni zariadenia prostredníctvom servera správy mobilných zariadení (MDM), keď je aplikácia balíka Office už nainštalovaná.</span><span class="sxs-lookup"><span data-stu-id="84d62-114">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="84d62-115">Mnohé MDM servery umožňujú správcom IT pridať voliteľný konfiguračný slovník, keď server odošle MDM príkaz `InstallApplication` do zariadenia so systémom iOS.</span><span class="sxs-lookup"><span data-stu-id="84d62-115">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="84d62-116">Ďalšie informácie nájdete v dokumentácii k MDM serveru.</span><span class="sxs-lookup"><span data-stu-id="84d62-116">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="84d62-117">Slovník je vyjadrený ako množina dvojíc kľúča a hodnoty vo formáte XML.</span><span class="sxs-lookup"><span data-stu-id="84d62-117">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="84d62-118">Príklad:</span><span class="sxs-lookup"><span data-stu-id="84d62-118">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="84d62-119">Po odoslaní do zariadenia sa konfiguračný slovník bude nachádzať v kľúči `com.apple.managed.configuration`, kde sa prečíta, keď sa spustí aplikácia balíka Office.</span><span class="sxs-lookup"><span data-stu-id="84d62-119">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="84d62-120">Nastavenia predvolieb pre diagnostické údaje</span><span class="sxs-lookup"><span data-stu-id="84d62-120">Preference setting for diagnostic data</span></span>

<span data-ttu-id="84d62-121">Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov.</span><span class="sxs-lookup"><span data-stu-id="84d62-121">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="84d62-122">Ďalšie informácie nájdete v téme [Diagnostické údaje odosielané zo služieb Office 365 ProPlus spoločnosti Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="84d62-122">For more information, see [Diagnostic data sent from Office 365 ProPlus to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84d62-123">**Kód**</span><span class="sxs-lookup"><span data-stu-id="84d62-123">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="84d62-124">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="84d62-124">**Data Type**</span></span>  | <span data-ttu-id="84d62-125">Reťazec</span><span class="sxs-lookup"><span data-stu-id="84d62-125">String</span></span> |
|<span data-ttu-id="84d62-126">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="84d62-126">**Possible values**</span></span>  | <span data-ttu-id="84d62-127">`BasicDiagnosticData` *(nastaví sa úroveň Požadované)*</span><span class="sxs-lookup"><span data-stu-id="84d62-127">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="84d62-128">`FullDiagnosticData` *(nastaví sa úroveň Voliteľné)*</span><span class="sxs-lookup"><span data-stu-id="84d62-128">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="84d62-129">`ZeroDiagnosticData` *(nastaví sa úroveň Žiadne)*</span><span class="sxs-lookup"><span data-stu-id="84d62-129">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="84d62-130">Ak túto predvoľbu nenastavíte, v prípade, že sa používatelia s predplatným na Office 365 prihlásili pomocou pracovného alebo školského konta, spoločnosti Microsoft sa odošlú len požadované diagnostické údaje.</span><span class="sxs-lookup"><span data-stu-id="84d62-130">Starting with new installations of Version 16.30, if you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 subscription are signed in with a work or school account or if users have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="84d62-131">Títo používatelia si tiež nemôžu zmeniť úroveň diagnostických údajov, bez ohľadu na to, ako ste túto predvoľbu nastavili.</span><span class="sxs-lookup"><span data-stu-id="84d62-131">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="84d62-132">V prípade ostatných používateľov, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, sa odosielajú iba požadované diagnostické údaje, pokiaľ si používateľ nezvolí možnosť odosielať aj voliteľné diagnostické údaje v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="84d62-132">For other users, such as home users with an Office 365 subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Preferences** > **Privacy**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="84d62-133">Nastavenia predvolieb pre online funkcie na analýzu obsahu</span><span class="sxs-lookup"><span data-stu-id="84d62-133">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="84d62-134">Online funkcie na analýzu obsahu sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií.</span><span class="sxs-lookup"><span data-stu-id="84d62-134">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="84d62-135">Napríklad Návrhy vzhľadu v PowerPointe.</span><span class="sxs-lookup"><span data-stu-id="84d62-135">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="84d62-136">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="84d62-136">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84d62-137">**Kód**</span><span class="sxs-lookup"><span data-stu-id="84d62-137">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="84d62-138">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="84d62-138">**Data Type**</span></span>  | <span data-ttu-id="84d62-139">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="84d62-139">Boolean</span></span> |
|<span data-ttu-id="84d62-140">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="84d62-140">**Possible values**</span></span>  | <span data-ttu-id="84d62-141">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="84d62-141">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="84d62-142">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="84d62-142">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="84d62-143">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na analýzu obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="84d62-143">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="84d62-144">Ak používatelia majú predplatné na Office 365 a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na analýzu obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="84d62-144">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="84d62-145">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, majú možnosť online funkcie na analýzu obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="84d62-145">For other users, such as home users with an Office 365 subscription, the user can choose to turn off connected experiences that analyze content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="84d62-146">Nastavenie predvolieb pre online funkcie na sťahovanie online obsahu</span><span class="sxs-lookup"><span data-stu-id="84d62-146">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="84d62-147">Online funkcie na sťahovanie online obsahu sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, videí a referenčných materiálov na vylepšenie vašich dokumentov.</span><span class="sxs-lookup"><span data-stu-id="84d62-147">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, 3D models, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="84d62-148">Napríklad šablóny balíka Office alebo funkcia vloženie online ikony.</span><span class="sxs-lookup"><span data-stu-id="84d62-148">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="84d62-149">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="84d62-149">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84d62-150">**Kód**</span><span class="sxs-lookup"><span data-stu-id="84d62-150">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="84d62-151">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="84d62-151">**Data Type**</span></span>  | <span data-ttu-id="84d62-152">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="84d62-152">Boolean</span></span> |
|<span data-ttu-id="84d62-153">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="84d62-153">**Possible values**</span></span>  | <span data-ttu-id="84d62-154">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="84d62-154">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="84d62-155">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="84d62-155">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="84d62-156">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na sťahovanie online obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="84d62-156">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="84d62-157">Ak používatelia majú predplatné na Office 365 a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na sťahovanie online obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="84d62-157">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="84d62-158">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, majú možnosť online funkcie na sťahovanie online obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="84d62-158">For other users, such as home users with an Office 365 subscription, a user can choose to turn off connected experiences that download online content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="84d62-159">Nastavenia predvolieb pre voliteľné online funkcie</span><span class="sxs-lookup"><span data-stu-id="84d62-159">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="84d62-160">Okrem online funkcií uvedených vyššie existujú aj voliteľné online funkcie, ku ktorým môžete používateľom povoliť prístup prostredníctvom ich konta organizácie, ktoré sa niekedy označuje ako pracovné alebo školské konto.</span><span class="sxs-lookup"><span data-stu-id="84d62-160">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="84d62-161">Napríklad doplnky balíka Office, ktoré sa do zariadenia sťahujú cez Office Obchod.</span><span class="sxs-lookup"><span data-stu-id="84d62-161">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="84d62-162">Ďalšie príklady nájdete v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="84d62-162">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84d62-163">**Kód**</span><span class="sxs-lookup"><span data-stu-id="84d62-163">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="84d62-164">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="84d62-164">**Data Type**</span></span>  | <span data-ttu-id="84d62-165">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="84d62-165">Boolean</span></span> |
|<span data-ttu-id="84d62-166">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="84d62-166">**Possible values**</span></span>  | <span data-ttu-id="84d62-167">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="84d62-167">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="84d62-168">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="84d62-168">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="84d62-169">Ak túto predvoľbu nenastavíte, voliteľné online funkcie sú používateľom k dispozícii v prípade, že sa používatelia s predplatným na Office 365 prihlásili pomocou pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="84d62-169">If you don't set this preference, optional connected experiences are available to users with an Office 365 subscription that are signed in with a work or school account or users who have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="84d62-170">Ako ste túto predvoľbu nenastavili na hodnotu FALSE, títo používatelia majú možnosť voliteľné online funkcie vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="84d62-170">Unless you have set this preference to , these users can choose to turn off optional connected experiences by going to Preferences  Privacy.</span></span>

<span data-ttu-id="84d62-171">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, nemajú možnosť vypnúť voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="84d62-171">For other users, such as home users with an Office 365 subscription, there isn't an option to turn off optional connected experiences.</span></span>