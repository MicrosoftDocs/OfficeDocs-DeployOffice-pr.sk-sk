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
ms.openlocfilehash: ed24ac934625bba61eac25e764a892d48365c005
ms.sourcegitcommit: 596a0a60394011aafe1119f353ac76f27e1a4d1b
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48794672"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="27c64-103">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb</span><span class="sxs-lookup"><span data-stu-id="27c64-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

> [!NOTE]
> <span data-ttu-id="27c64-104">Ak si chcete pozrieť zoznam produktov balíka Office, na ktorý sa vzťahujú tieto informácie o ochrane osobných údajov, pozrite si tému [Ovládacie prvky na ochranu osobných údajov dostupné pre produkty balíka Office](products-versions-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="27c64-104">For a list of Office products covered by this privacy information, see [Privacy controls available for Office products](products-versions-privacy-controls.md).</span></span>

<span data-ttu-id="27c64-105">K dispozícii sú nové nastavenia predvolieb pre Office v zariadeniach so systémom iOS, ktoré umožňujú ovládať nastavenia pre:</span><span class="sxs-lookup"><span data-stu-id="27c64-105">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="27c64-106">\***Diagnostické údaje** _, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.</span><span class="sxs-lookup"><span data-stu-id="27c64-106">\***Diagnostic data** _ that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="27c64-107">_*_Online funkcie_*_ , ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.</span><span class="sxs-lookup"><span data-stu-id="27c64-107">_*_Connected experiences_*_ that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="27c64-108">Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="27c64-108">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

> [!NOTE]
> <span data-ttu-id="27c64-109">Ďalšie informácie o podobných nastaveniach balíka Office v počítačoch so systémom macOS nájdete v téme [Spravovanie ovládacích prvkov ochrany osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="27c64-109">For information about similar settings for Office on computers running macOS, see [Use preferences to manage privacy controls for Office for Mac](mac-privacy-preferences.md)</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="27c64-110">Nastavenie predvolieb zariadenia</span><span class="sxs-lookup"><span data-stu-id="27c64-110">Setting device preferences</span></span>
<span data-ttu-id="27c64-111">Tieto nové nastavenia predvolieb je možné nastaviť aj na úrovni zariadenia prostredníctvom servera správy mobilných zariadení (MDM), keď je aplikácia balíka Office už nainštalovaná.</span><span class="sxs-lookup"><span data-stu-id="27c64-111">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="27c64-112">Mnohé MDM servery umožňujú správcom IT pridať voliteľný konfiguračný slovník, keď server odošle MDM príkaz `InstallApplication` do zariadenia so systémom iOS.</span><span class="sxs-lookup"><span data-stu-id="27c64-112">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="27c64-113">Ďalšie informácie nájdete v dokumentácii k MDM serveru.</span><span class="sxs-lookup"><span data-stu-id="27c64-113">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="27c64-114">Slovník je vyjadrený ako množina dvojíc kľúča a hodnoty vo formáte XML.</span><span class="sxs-lookup"><span data-stu-id="27c64-114">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="27c64-115">Príklad:</span><span class="sxs-lookup"><span data-stu-id="27c64-115">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="27c64-116">Po odoslaní do zariadenia sa konfiguračný slovník bude nachádzať v kľúči `com.apple.managed.configuration`, kde sa prečíta, keď sa spustí aplikácia balíka Office.</span><span class="sxs-lookup"><span data-stu-id="27c64-116">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

> [!NOTE]
> <span data-ttu-id="27c64-117">Môžete použiť aj cloudovú službu politiky pre Office a tieto 4 nastavenia politiky:</span><span class="sxs-lookup"><span data-stu-id="27c64-117">You can also use the Office cloud policy service and these 4 policy settings:</span></span>
> - <span data-ttu-id="27c64-118">Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="27c64-118">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>
> - <span data-ttu-id="27c64-119">Povoliť používanie pripojených funkcií na analýzu obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="27c64-119">Allow the use of connected experiences in Office that analyze content</span></span>
> - <span data-ttu-id="27c64-120">Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="27c64-120">Allow the use of connected experiences in Office that download online content</span></span>
> - <span data-ttu-id="27c64-121">Povoliť používanie dodatočných voliteľných pripojených funkcií v Office</span><span class="sxs-lookup"><span data-stu-id="27c64-121">Allow the use of additional optional connected experiences in Office</span></span>
>
> <span data-ttu-id="27c64-122">Nastavenia ochrany osobných údajov pre Outlook pre iOS a OneDrive pre iOS je možné nakonfigurovať iba pomocou cloudovej služby politiky pre Office.</span><span class="sxs-lookup"><span data-stu-id="27c64-122">Privacy settings for Outlook for iOS and OneDrive for iOS can only be configured by using the Office cloud policy service.</span></span>
>
> <span data-ttu-id="27c64-123">Ďalšie informácie o použití cloudovej služby politiky pre Office nájdete v téme [Prehľad cloudovej služby politiky pre Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="27c64-123">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="27c64-124">Nastavenia predvolieb pre diagnostické údaje</span><span class="sxs-lookup"><span data-stu-id="27c64-124">Preference setting for diagnostic data</span></span>

<span data-ttu-id="27c64-125">Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov.</span><span class="sxs-lookup"><span data-stu-id="27c64-125">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="27c64-126">Ďalšie informácie nájdete v téme [Diagnostické údaje odoslané z Aplikácií Microsoft 365 pre veľké organizácie do spoločnosti Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="27c64-126">For more information, see [Diagnostic data sent from Microsoft 365 Apps for enterprise to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27c64-127">_ *Kód*\*</span><span class="sxs-lookup"><span data-stu-id="27c64-127">_ *Key*\*</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="27c64-128">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="27c64-128">**Data Type**</span></span>  | <span data-ttu-id="27c64-129">Reťazec</span><span class="sxs-lookup"><span data-stu-id="27c64-129">String</span></span> |
|<span data-ttu-id="27c64-130">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="27c64-130">**Possible values**</span></span>  | <span data-ttu-id="27c64-131">`BasicDiagnosticData` *(nastaví sa úroveň Požadované)*</span><span class="sxs-lookup"><span data-stu-id="27c64-131">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="27c64-132">`FullDiagnosticData` *(nastaví sa úroveň Voliteľné)*</span><span class="sxs-lookup"><span data-stu-id="27c64-132">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="27c64-133">`ZeroDiagnosticData` *(nastaví sa úroveň Žiadne)*</span><span class="sxs-lookup"><span data-stu-id="27c64-133">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="27c64-134">Ak túto predvoľbu nenastavíte, v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta, spoločnosti Microsoft sa odošlú len požadované diagnostické údaje.</span><span class="sxs-lookup"><span data-stu-id="27c64-134">If you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 (or Microsoft 365) subscription are signed in with a work or school account.</span></span> <span data-ttu-id="27c64-135">Títo používatelia si tiež nemôžu zmeniť úroveň diagnostických údajov, bez ohľadu na to, ako ste túto predvoľbu nastavili.</span><span class="sxs-lookup"><span data-stu-id="27c64-135">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="27c64-136">V prípade ostatných používateľov, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), sa odosielajú iba požadované diagnostické údaje, pokiaľ si používateľ nezvolí možnosť odosielať aj voliteľné diagnostické údaje v okne **Nastavenia** > **Nastavenia ochrany osobných údajov** .</span><span class="sxs-lookup"><span data-stu-id="27c64-136">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Settings** > **Privacy Settings** .</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="27c64-137">Nastavenia predvolieb pre online funkcie na analýzu obsahu</span><span class="sxs-lookup"><span data-stu-id="27c64-137">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="27c64-138">Online funkcie na analýzu obsahu sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií.</span><span class="sxs-lookup"><span data-stu-id="27c64-138">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="27c64-139">Napríklad Návrhy vzhľadu v PowerPointe.</span><span class="sxs-lookup"><span data-stu-id="27c64-139">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="27c64-140">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="27c64-140">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27c64-141">**Kód**</span><span class="sxs-lookup"><span data-stu-id="27c64-141">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="27c64-142">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="27c64-142">**Data Type**</span></span>  | <span data-ttu-id="27c64-143">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="27c64-143">Boolean</span></span> |
|<span data-ttu-id="27c64-144">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="27c64-144">**Possible values**</span></span>  | <span data-ttu-id="27c64-145">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="27c64-145">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="27c64-146">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="27c64-146">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="27c64-147">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na analýzu obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="27c64-147">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="27c64-148">Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na analýzu obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="27c64-148">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="27c64-149">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na analýzu obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov** .</span><span class="sxs-lookup"><span data-stu-id="27c64-149">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that analyze content by going to **Settings** > **Privacy Settings** .</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="27c64-150">Nastavenie predvolieb pre online funkcie na sťahovanie online obsahu</span><span class="sxs-lookup"><span data-stu-id="27c64-150">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="27c64-151">Online funkcie na sťahovanie online obsahu sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, videí a referenčných materiálov na vylepšenie vašich dokumentov.</span><span class="sxs-lookup"><span data-stu-id="27c64-151">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="27c64-152">Napríklad šablóny balíka Office alebo funkcia vloženie online ikony.</span><span class="sxs-lookup"><span data-stu-id="27c64-152">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="27c64-153">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="27c64-153">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27c64-154">**Kód**</span><span class="sxs-lookup"><span data-stu-id="27c64-154">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="27c64-155">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="27c64-155">**Data Type**</span></span>  | <span data-ttu-id="27c64-156">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="27c64-156">Boolean</span></span> |
|<span data-ttu-id="27c64-157">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="27c64-157">**Possible values**</span></span>  | <span data-ttu-id="27c64-158">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="27c64-158">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="27c64-159">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="27c64-159">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="27c64-160">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na sťahovanie online obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="27c64-160">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="27c64-161">Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na sťahovanie online obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="27c64-161">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="27c64-162">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na sťahovanie online obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov** .</span><span class="sxs-lookup"><span data-stu-id="27c64-162">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that download online content by going to **Settings** > **Privacy Settings** .</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="27c64-163">Nastavenia predvolieb pre voliteľné online funkcie</span><span class="sxs-lookup"><span data-stu-id="27c64-163">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="27c64-164">Okrem online funkcií uvedených vyššie existujú aj voliteľné online funkcie, ku ktorým môžete používateľom povoliť prístup prostredníctvom ich konta organizácie, ktoré sa niekedy označuje ako pracovné alebo školské konto.</span><span class="sxs-lookup"><span data-stu-id="27c64-164">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="27c64-165">Napríklad doplnky balíka Office, ktoré sa do zariadenia sťahujú cez Office Obchod.</span><span class="sxs-lookup"><span data-stu-id="27c64-165">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="27c64-166">Ďalšie príklady nájdete v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="27c64-166">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27c64-167">**Kód**</span><span class="sxs-lookup"><span data-stu-id="27c64-167">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="27c64-168">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="27c64-168">**Data Type**</span></span>  | <span data-ttu-id="27c64-169">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="27c64-169">Boolean</span></span> |
|<span data-ttu-id="27c64-170">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="27c64-170">**Possible values**</span></span>  | <span data-ttu-id="27c64-171">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="27c64-171">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="27c64-172">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="27c64-172">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="27c64-173">Ak túto predvoľbu nenastavíte, voliteľné online funkcie sú používateľom k dispozícii v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="27c64-173">If you don't set this preference, optional connected experiences are available to users with an Office 365 (or Microsoft 365) subscription that are signed in with a work or school account.</span></span> <span data-ttu-id="27c64-174">Ako ste túto predvoľbu nenastavili na hodnotu FALSE, títo používatelia majú možnosť voliteľné online funkcie vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov** .</span><span class="sxs-lookup"><span data-stu-id="27c64-174">Unless you have set this preference to FALSE, these users can choose to turn off optional connected experiences by going to **Settings** > **Privacy Settings** .</span></span>

<span data-ttu-id="27c64-175">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), nemajú možnosť vypnúť voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="27c64-175">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, there isn't an option to turn off optional connected experiences.</span></span>