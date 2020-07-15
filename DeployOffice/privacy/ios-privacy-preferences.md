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
ms.openlocfilehash: ac8b3428734649981f20a82be2f0793c857e09ee
ms.sourcegitcommit: 81295dff0f2fa474f0db39fd40560e3a23fff32a
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/09/2020
ms.locfileid: "45092169"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="e8949-103">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb</span><span class="sxs-lookup"><span data-stu-id="e8949-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

<span data-ttu-id="e8949-104">K dispozícii sú nové nastavenia predvolieb pre Office v zariadeniach so systémom iOS, ktoré umožňujú ovládať nastavenia pre:</span><span class="sxs-lookup"><span data-stu-id="e8949-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="e8949-105">***Diagnostické údaje***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.</span><span class="sxs-lookup"><span data-stu-id="e8949-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="e8949-106">***Online funkcie***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.</span><span class="sxs-lookup"><span data-stu-id="e8949-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="e8949-107">Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="e8949-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="e8949-108">Tieto nastavenia predvolieb sa týkajú aplikácií:</span><span class="sxs-lookup"><span data-stu-id="e8949-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="e8949-109">Word pre iOS, Excel pre iOS a PowerPoint pre iOS verzie 2.30 a novšej.</span><span class="sxs-lookup"><span data-stu-id="e8949-109">Version 2.30 and later of Word for iOS, Excel for iOS, and PowerPoint for iOS.</span></span>
- <span data-ttu-id="e8949-110">Outlook pre iOS verzie 4.30.0 a novšej.</span><span class="sxs-lookup"><span data-stu-id="e8949-110">Version 4.30.0 and later of Outlook for iOS</span></span>
- <span data-ttu-id="e8949-111">OneNote pre iOS verzie 16.30 a novšej.</span><span class="sxs-lookup"><span data-stu-id="e8949-111">Version 16.30 and later of OneNote for iOS.</span></span>
- <span data-ttu-id="e8949-112">OneDrive pre iOS verzie 11.19.11 a novšej.</span><span class="sxs-lookup"><span data-stu-id="e8949-112">Version 11.19.11 and later of OneDrive for iOS.</span></span>
- <span data-ttu-id="e8949-113">Visio Viewer pre iOS verzie 1.17 a novšej.</span><span class="sxs-lookup"><span data-stu-id="e8949-113">Version 1.17 and later of Visio Viewer for iOS.</span></span>
- <span data-ttu-id="e8949-114">Aplikácia Office pre iOS verzie 2.34 a novšej.</span><span class="sxs-lookup"><span data-stu-id="e8949-114">Version 2.34 and later of the Office app for iOS.</span></span>

> [!NOTE]
> <span data-ttu-id="e8949-115">Ďalšie informácie o podobných nastaveniach balíka Office v počítačoch so systémom macOS nájdete v téme [Spravovanie ovládacích prvkov ochrany osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="e8949-115">For information about similar settings for Office on computers running macOS, see [Use preferences to manage privacy controls for Office for Mac](mac-privacy-preferences.md)</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="e8949-116">Nastavenie predvolieb zariadenia</span><span class="sxs-lookup"><span data-stu-id="e8949-116">Setting device preferences</span></span>
<span data-ttu-id="e8949-117">Tieto nové nastavenia predvolieb je možné nastaviť aj na úrovni zariadenia prostredníctvom servera správy mobilných zariadení (MDM), keď je aplikácia balíka Office už nainštalovaná.</span><span class="sxs-lookup"><span data-stu-id="e8949-117">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="e8949-118">Mnohé MDM servery umožňujú správcom IT pridať voliteľný konfiguračný slovník, keď server odošle MDM príkaz `InstallApplication` do zariadenia so systémom iOS.</span><span class="sxs-lookup"><span data-stu-id="e8949-118">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="e8949-119">Ďalšie informácie nájdete v dokumentácii k MDM serveru.</span><span class="sxs-lookup"><span data-stu-id="e8949-119">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="e8949-120">Slovník je vyjadrený ako množina dvojíc kľúča a hodnoty vo formáte XML.</span><span class="sxs-lookup"><span data-stu-id="e8949-120">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="e8949-121">Príklad:</span><span class="sxs-lookup"><span data-stu-id="e8949-121">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="e8949-122">Po odoslaní do zariadenia sa konfiguračný slovník bude nachádzať v kľúči `com.apple.managed.configuration`, kde sa prečíta, keď sa spustí aplikácia balíka Office.</span><span class="sxs-lookup"><span data-stu-id="e8949-122">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

> [!NOTE]
> <span data-ttu-id="e8949-123">Môžete použiť aj cloudovú službu politiky pre Office a tieto 4 nastavenia politiky:</span><span class="sxs-lookup"><span data-stu-id="e8949-123">You can also use the Office cloud policy service and these 4 policy settings:</span></span>
> - <span data-ttu-id="e8949-124">Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="e8949-124">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>
> - <span data-ttu-id="e8949-125">Povoliť používanie pripojených funkcií na analýzu obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="e8949-125">Allow the use of connected experiences in Office that analyze content</span></span>
> - <span data-ttu-id="e8949-126">Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="e8949-126">Allow the use of connected experiences in Office that download online content</span></span>
> - <span data-ttu-id="e8949-127">Povoliť používanie dodatočných voliteľných pripojených funkcií v Office</span><span class="sxs-lookup"><span data-stu-id="e8949-127">Allow the use of additional optional connected experiences in Office</span></span>
>
> <span data-ttu-id="e8949-128">Nastavenia ochrany osobných údajov pre Outlook pre iOS a OneDrive pre iOS je možné nakonfigurovať iba pomocou cloudovej služby politiky pre Office.</span><span class="sxs-lookup"><span data-stu-id="e8949-128">Privacy settings for Outlook for iOS and OneDrive for iOS can only be configured by using the Office cloud policy service.</span></span>
>
> <span data-ttu-id="e8949-129">Ďalšie informácie o použití cloudovej služby politiky pre Office nájdete v téme [Prehľad cloudovej služby politiky pre Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="e8949-129">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="e8949-130">Nastavenia predvolieb pre diagnostické údaje</span><span class="sxs-lookup"><span data-stu-id="e8949-130">Preference setting for diagnostic data</span></span>

<span data-ttu-id="e8949-131">Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov.</span><span class="sxs-lookup"><span data-stu-id="e8949-131">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="e8949-132">Ďalšie informácie nájdete v téme [Diagnostické údaje odoslané z Aplikácií Microsoft 365 pre veľké organizácie do spoločnosti Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="e8949-132">For more information, see [Diagnostic data sent from Microsoft 365 Apps for enterprise to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8949-133">**Kód**</span><span class="sxs-lookup"><span data-stu-id="e8949-133">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="e8949-134">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="e8949-134">**Data Type**</span></span>  | <span data-ttu-id="e8949-135">Reťazec</span><span class="sxs-lookup"><span data-stu-id="e8949-135">String</span></span> |
|<span data-ttu-id="e8949-136">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="e8949-136">**Possible values**</span></span>  | <span data-ttu-id="e8949-137">`BasicDiagnosticData` *(nastaví sa úroveň Požadované)*</span><span class="sxs-lookup"><span data-stu-id="e8949-137">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="e8949-138">`FullDiagnosticData` *(nastaví sa úroveň Voliteľné)*</span><span class="sxs-lookup"><span data-stu-id="e8949-138">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="e8949-139">`ZeroDiagnosticData` *(nastaví sa úroveň Žiadne)*</span><span class="sxs-lookup"><span data-stu-id="e8949-139">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="e8949-140">Ak túto predvoľbu nenastavíte, v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta, spoločnosti Microsoft sa odošlú len požadované diagnostické údaje.</span><span class="sxs-lookup"><span data-stu-id="e8949-140">If you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 (or Microsoft 365) subscription are signed in with a work or school account.</span></span> <span data-ttu-id="e8949-141">Títo používatelia si tiež nemôžu zmeniť úroveň diagnostických údajov, bez ohľadu na to, ako ste túto predvoľbu nastavili.</span><span class="sxs-lookup"><span data-stu-id="e8949-141">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="e8949-142">V prípade ostatných používateľov, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), sa odosielajú iba požadované diagnostické údaje, pokiaľ si používateľ nezvolí možnosť odosielať aj voliteľné diagnostické údaje v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="e8949-142">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Settings** > **Privacy Settings**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="e8949-143">Nastavenia predvolieb pre online funkcie na analýzu obsahu</span><span class="sxs-lookup"><span data-stu-id="e8949-143">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="e8949-144">Online funkcie na analýzu obsahu sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií.</span><span class="sxs-lookup"><span data-stu-id="e8949-144">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="e8949-145">Napríklad Návrhy vzhľadu v PowerPointe.</span><span class="sxs-lookup"><span data-stu-id="e8949-145">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="e8949-146">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="e8949-146">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8949-147">**Kód**</span><span class="sxs-lookup"><span data-stu-id="e8949-147">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="e8949-148">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="e8949-148">**Data Type**</span></span>  | <span data-ttu-id="e8949-149">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="e8949-149">Boolean</span></span> |
|<span data-ttu-id="e8949-150">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="e8949-150">**Possible values**</span></span>  | <span data-ttu-id="e8949-151">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="e8949-151">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="e8949-152">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="e8949-152">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="e8949-153">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na analýzu obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="e8949-153">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="e8949-154">Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na analýzu obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="e8949-154">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="e8949-155">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na analýzu obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="e8949-155">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that analyze content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="e8949-156">Nastavenie predvolieb pre online funkcie na sťahovanie online obsahu</span><span class="sxs-lookup"><span data-stu-id="e8949-156">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="e8949-157">Online funkcie na sťahovanie online obsahu sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, videí a referenčných materiálov na vylepšenie vašich dokumentov.</span><span class="sxs-lookup"><span data-stu-id="e8949-157">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="e8949-158">Napríklad šablóny balíka Office alebo funkcia vloženie online ikony.</span><span class="sxs-lookup"><span data-stu-id="e8949-158">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="e8949-159">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="e8949-159">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8949-160">**Kód**</span><span class="sxs-lookup"><span data-stu-id="e8949-160">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="e8949-161">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="e8949-161">**Data Type**</span></span>  | <span data-ttu-id="e8949-162">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="e8949-162">Boolean</span></span> |
|<span data-ttu-id="e8949-163">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="e8949-163">**Possible values**</span></span>  | <span data-ttu-id="e8949-164">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="e8949-164">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="e8949-165">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="e8949-165">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="e8949-166">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na sťahovanie online obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="e8949-166">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="e8949-167">Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na sťahovanie online obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="e8949-167">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="e8949-168">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na sťahovanie online obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="e8949-168">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that download online content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="e8949-169">Nastavenia predvolieb pre voliteľné online funkcie</span><span class="sxs-lookup"><span data-stu-id="e8949-169">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="e8949-170">Okrem online funkcií uvedených vyššie existujú aj voliteľné online funkcie, ku ktorým môžete používateľom povoliť prístup prostredníctvom ich konta organizácie, ktoré sa niekedy označuje ako pracovné alebo školské konto.</span><span class="sxs-lookup"><span data-stu-id="e8949-170">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="e8949-171">Napríklad doplnky balíka Office, ktoré sa do zariadenia sťahujú cez Office Obchod.</span><span class="sxs-lookup"><span data-stu-id="e8949-171">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="e8949-172">Ďalšie príklady nájdete v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="e8949-172">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8949-173">**Kód**</span><span class="sxs-lookup"><span data-stu-id="e8949-173">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="e8949-174">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="e8949-174">**Data Type**</span></span>  | <span data-ttu-id="e8949-175">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="e8949-175">Boolean</span></span> |
|<span data-ttu-id="e8949-176">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="e8949-176">**Possible values**</span></span>  | <span data-ttu-id="e8949-177">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="e8949-177">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="e8949-178">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="e8949-178">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="e8949-179">Ak túto predvoľbu nenastavíte, voliteľné online funkcie sú používateľom k dispozícii v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="e8949-179">If you don't set this preference, optional connected experiences are available to users with an Office 365 (or Microsoft 365) subscription that are signed in with a work or school account.</span></span> <span data-ttu-id="e8949-180">Ako ste túto predvoľbu nenastavili na hodnotu FALSE, títo používatelia majú možnosť voliteľné online funkcie vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="e8949-180">Unless you have set this preference to FALSE, these users can choose to turn off optional connected experiences by going to **Settings** > **Privacy Settings**.</span></span>

<span data-ttu-id="e8949-181">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), nemajú možnosť vypnúť voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="e8949-181">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, there isn't an option to turn off optional connected experiences.</span></span>