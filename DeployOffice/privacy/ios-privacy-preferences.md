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
ms.openlocfilehash: 40fc1ec1f5b2abc587e1b5224dc7fe0a5a656f33
ms.sourcegitcommit: 3890a23390edd0b5fdb2cf33613ec0778566cf97
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/01/2020
ms.locfileid: "43992121"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a><span data-ttu-id="244a5-103">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb</span><span class="sxs-lookup"><span data-stu-id="244a5-103">Use preferences to manage privacy controls for Office on iOS devices</span></span>

<span data-ttu-id="244a5-104">K dispozícii sú nové nastavenia predvolieb pre Office v zariadeniach so systémom iOS, ktoré umožňujú ovládať nastavenia pre:</span><span class="sxs-lookup"><span data-stu-id="244a5-104">There are new preference settings for Office on iOS devices that allow you to control settings related to the following:</span></span>

- <span data-ttu-id="244a5-105">***Diagnostické údaje***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.</span><span class="sxs-lookup"><span data-stu-id="244a5-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used.</span></span>

- <span data-ttu-id="244a5-106">***Online funkcie***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.</span><span class="sxs-lookup"><span data-stu-id="244a5-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="244a5-107">Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="244a5-107">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

<span data-ttu-id="244a5-108">Tieto nastavenia predvolieb sa týkajú aplikácií:</span><span class="sxs-lookup"><span data-stu-id="244a5-108">These preference settings apply to the following applications:</span></span>
- <span data-ttu-id="244a5-109">Word pre iOS, Excel pre iOS a PowerPoint pre iOS verzie 2.30 a novšej.</span><span class="sxs-lookup"><span data-stu-id="244a5-109">Version 2.30 and later of Word for iOS, Excel for iOS, and PowerPoint for iOS.</span></span>
- <span data-ttu-id="244a5-110">OneNote pre iOS verzie 16.30 a novšej.</span><span class="sxs-lookup"><span data-stu-id="244a5-110">Version 16.30 and later of OneNote for iOS.</span></span>
- <span data-ttu-id="244a5-111">Visio Viewer pre iOS verzie 1.17 a novšej.</span><span class="sxs-lookup"><span data-stu-id="244a5-111">Version 1.17 and later of Visio Viewer for iOS.</span></span>

> [!NOTE]
> <span data-ttu-id="244a5-112">Ďalšie informácie o podobných nastaveniach balíka Office v počítačoch so systémom macOS nájdete v téme [Spravovanie ovládacích prvkov ochrany osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md).</span><span class="sxs-lookup"><span data-stu-id="244a5-112">For information about similar settings for Office on computers running macOS, see [Use preferences to manage privacy controls for Office for Mac](mac-privacy-preferences.md)</span></span>


## <a name="setting-device-preferences"></a><span data-ttu-id="244a5-113">Nastavenie predvolieb zariadenia</span><span class="sxs-lookup"><span data-stu-id="244a5-113">Setting device preferences</span></span>
<span data-ttu-id="244a5-114">Tieto nové nastavenia predvolieb je možné nastaviť aj na úrovni zariadenia prostredníctvom servera správy mobilných zariadení (MDM), keď je aplikácia balíka Office už nainštalovaná.</span><span class="sxs-lookup"><span data-stu-id="244a5-114">These new preference settings can also be set at the device level by a Mobile Device Management (MDM) server when the Office application is installed.</span></span> <span data-ttu-id="244a5-115">Mnohé MDM servery umožňujú správcom IT pridať voliteľný konfiguračný slovník, keď server odošle MDM príkaz `InstallApplication` do zariadenia so systémom iOS.</span><span class="sxs-lookup"><span data-stu-id="244a5-115">Many MDM servers allow IT administrators to add an optional configuration dictionary when the server sends the `InstallApplication` MDM command to an iOS device.</span></span> <span data-ttu-id="244a5-116">Ďalšie informácie nájdete v dokumentácii k MDM serveru.</span><span class="sxs-lookup"><span data-stu-id="244a5-116">Refer to your MDM server documentation for more details.</span></span>

<span data-ttu-id="244a5-117">Slovník je vyjadrený ako množina dvojíc kľúča a hodnoty vo formáte XML.</span><span class="sxs-lookup"><span data-stu-id="244a5-117">The dictionary is represented as a set of key/value pairs in XML format.</span></span> <span data-ttu-id="244a5-118">Príklad:</span><span class="sxs-lookup"><span data-stu-id="244a5-118">For example:</span></span>

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

<span data-ttu-id="244a5-119">Po odoslaní do zariadenia sa konfiguračný slovník bude nachádzať v kľúči `com.apple.managed.configuration`, kde sa prečíta, keď sa spustí aplikácia balíka Office.</span><span class="sxs-lookup"><span data-stu-id="244a5-119">Once sent to the device, the configuration dictionary will reside under the `com.apple.managed.configuration` key, where it will be read when the Office application is launched.</span></span>

> [!NOTE]
> <span data-ttu-id="244a5-120">Môžete použiť aj cloudovú službu politiky pre Office a tieto 4 nastavenia politiky:</span><span class="sxs-lookup"><span data-stu-id="244a5-120">You can also use the Office cloud policy service and these 4 policy settings:</span></span>
> - <span data-ttu-id="244a5-121">Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="244a5-121">Configure the level of client software diagnostic data sent by Office to Microsoft</span></span>
> - <span data-ttu-id="244a5-122">Povoliť používanie pripojených funkcií na analýzu obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="244a5-122">Allow the use of connected experiences in Office that analyze content</span></span>
> - <span data-ttu-id="244a5-123">Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office</span><span class="sxs-lookup"><span data-stu-id="244a5-123">Allow the use of connected experiences in Office that download online content</span></span>
> - <span data-ttu-id="244a5-124">Povoliť používanie dodatočných voliteľných pripojených funkcií v Office</span><span class="sxs-lookup"><span data-stu-id="244a5-124">Allow the use of additional optional connected experiences in Office</span></span>
>
> <span data-ttu-id="244a5-125">Ďalšie informácie o použití cloudovej služby politiky pre Office nájdete v téme [Prehľad cloudovej služby politiky pre Office](../overview-office-cloud-policy-service.md).</span><span class="sxs-lookup"><span data-stu-id="244a5-125">For more information on using the Office cloud policy service, see [Overview of the Office cloud policy service](../overview-office-cloud-policy-service.md).</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="244a5-126">Nastavenia predvolieb pre diagnostické údaje</span><span class="sxs-lookup"><span data-stu-id="244a5-126">Preference setting for diagnostic data</span></span>

<span data-ttu-id="244a5-127">Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov.</span><span class="sxs-lookup"><span data-stu-id="244a5-127">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="244a5-128">Ďalšie informácie nájdete v téme [Diagnostické údaje odoslané z Aplikácií Microsoft 365 pre veľké organizácie do spoločnosti Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="244a5-128">For more information, see [Diagnostic data sent from Microsoft 365 Apps for enterprise to Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="244a5-129">**Kód**</span><span class="sxs-lookup"><span data-stu-id="244a5-129">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="244a5-130">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="244a5-130">**Data Type**</span></span>  | <span data-ttu-id="244a5-131">Reťazec</span><span class="sxs-lookup"><span data-stu-id="244a5-131">String</span></span> |
|<span data-ttu-id="244a5-132">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="244a5-132">**Possible values**</span></span>  | <span data-ttu-id="244a5-133">`BasicDiagnosticData` *(nastaví sa úroveň Požadované)*</span><span class="sxs-lookup"><span data-stu-id="244a5-133">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="244a5-134">`FullDiagnosticData` *(nastaví sa úroveň Voliteľné)*</span><span class="sxs-lookup"><span data-stu-id="244a5-134">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="244a5-135">`ZeroDiagnosticData` *(nastaví sa úroveň Žiadne)*</span><span class="sxs-lookup"><span data-stu-id="244a5-135">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |

<span data-ttu-id="244a5-136">Ak túto predvoľbu nenastavíte, v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta, spoločnosti Microsoft sa odošlú len požadované diagnostické údaje.</span><span class="sxs-lookup"><span data-stu-id="244a5-136">If you don't set this preference, only required diagnostic data is sent to Microsoft if users with an Office 365 (or Microsoft 365) subscription are signed in with a work or school account.</span></span> <span data-ttu-id="244a5-137">Títo používatelia si tiež nemôžu zmeniť úroveň diagnostických údajov, bez ohľadu na to, ako ste túto predvoľbu nastavili.</span><span class="sxs-lookup"><span data-stu-id="244a5-137">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="244a5-138">V prípade ostatných používateľov, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), sa odosielajú iba požadované diagnostické údaje, pokiaľ si používateľ nezvolí možnosť odosielať aj voliteľné diagnostické údaje v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="244a5-138">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Settings** > **Privacy Settings**.</span></span>


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="244a5-139">Nastavenia predvolieb pre online funkcie na analýzu obsahu</span><span class="sxs-lookup"><span data-stu-id="244a5-139">Preference setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="244a5-140">Online funkcie na analýzu obsahu sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií.</span><span class="sxs-lookup"><span data-stu-id="244a5-140">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="244a5-141">Napríklad Návrhy vzhľadu v PowerPointe.</span><span class="sxs-lookup"><span data-stu-id="244a5-141">For example, Design Ideas in PowerPoint.</span></span> <span data-ttu-id="244a5-142">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="244a5-142">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="244a5-143">**Kód**</span><span class="sxs-lookup"><span data-stu-id="244a5-143">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="244a5-144">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="244a5-144">**Data Type**</span></span>  | <span data-ttu-id="244a5-145">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="244a5-145">Boolean</span></span> |
|<span data-ttu-id="244a5-146">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="244a5-146">**Possible values**</span></span>  | <span data-ttu-id="244a5-147">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="244a5-147">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="244a5-148">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="244a5-148">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="244a5-149">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na analýzu obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="244a5-149">If you don't set this preference, connected experiences that analyze content are available to users.</span></span>

<span data-ttu-id="244a5-150">Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na analýzu obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="244a5-150">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="244a5-151">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na analýzu obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="244a5-151">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that analyze content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="244a5-152">Nastavenie predvolieb pre online funkcie na sťahovanie online obsahu</span><span class="sxs-lookup"><span data-stu-id="244a5-152">Preference setting for connected experiences that download online content</span></span>

<span data-ttu-id="244a5-153">Online funkcie na sťahovanie online obsahu sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, videí a referenčných materiálov na vylepšenie vašich dokumentov.</span><span class="sxs-lookup"><span data-stu-id="244a5-153">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="244a5-154">Napríklad šablóny balíka Office alebo funkcia vloženie online ikony.</span><span class="sxs-lookup"><span data-stu-id="244a5-154">For example, Office templates or inserting an online icon.</span></span> <span data-ttu-id="244a5-155">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="244a5-155">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="244a5-156">**Kód**</span><span class="sxs-lookup"><span data-stu-id="244a5-156">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="244a5-157">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="244a5-157">**Data Type**</span></span>  | <span data-ttu-id="244a5-158">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="244a5-158">Boolean</span></span> |
|<span data-ttu-id="244a5-159">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="244a5-159">**Possible values**</span></span>  | <span data-ttu-id="244a5-160">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="244a5-160">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="244a5-161">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="244a5-161">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="244a5-162">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na sťahovanie online obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="244a5-162">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="244a5-163">Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na sťahovanie online obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="244a5-163">If the user has an Office 365 (or Microsoft 365) subscription and is signed in with a work or school account, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="244a5-164">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na sťahovanie online obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="244a5-164">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, the user can choose to turn off connected experiences that download online content by going to **Settings** > **Privacy Settings**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="244a5-165">Nastavenia predvolieb pre voliteľné online funkcie</span><span class="sxs-lookup"><span data-stu-id="244a5-165">Preference setting for optional connected experiences</span></span>

<span data-ttu-id="244a5-166">Okrem online funkcií uvedených vyššie existujú aj voliteľné online funkcie, ku ktorým môžete používateľom povoliť prístup prostredníctvom ich konta organizácie, ktoré sa niekedy označuje ako pracovné alebo školské konto.</span><span class="sxs-lookup"><span data-stu-id="244a5-166">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="244a5-167">Napríklad doplnky balíka Office, ktoré sa do zariadenia sťahujú cez Office Obchod.</span><span class="sxs-lookup"><span data-stu-id="244a5-167">For example, Office add-ins that are downloaded through the Office Store to your device.</span></span> <span data-ttu-id="244a5-168">Ďalšie príklady nájdete v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="244a5-168">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="244a5-169">**Kód**</span><span class="sxs-lookup"><span data-stu-id="244a5-169">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="244a5-170">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="244a5-170">**Data Type**</span></span>  | <span data-ttu-id="244a5-171">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="244a5-171">Boolean</span></span> |
|<span data-ttu-id="244a5-172">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="244a5-172">**Possible values**</span></span>  | <span data-ttu-id="244a5-173">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="244a5-173">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="244a5-174">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="244a5-174">`FALSE` *(disabled)*</span></span>|


<span data-ttu-id="244a5-175">Ak túto predvoľbu nenastavíte, voliteľné online funkcie sú používateľom k dispozícii v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="244a5-175">If you don't set this preference, optional connected experiences are available to users with an Office 365 (or Microsoft 365) subscription that are signed in with a work or school account.</span></span> <span data-ttu-id="244a5-176">Ako ste túto predvoľbu nenastavili na hodnotu FALSE, títo používatelia majú možnosť voliteľné online funkcie vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="244a5-176">Unless you have set this preference to FALSE, these users can choose to turn off optional connected experiences by going to **Settings** > **Privacy Settings**.</span></span>

<span data-ttu-id="244a5-177">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), nemajú možnosť vypnúť voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="244a5-177">For other users, such as home users with an Office 365 (or Microsoft 365) subscription, there isn't an option to turn off optional connected experiences.</span></span>