---
title: Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb
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
description: V tomto článku správcovia služieb Office získajú informácie o postupoch spravovania ovládacích prvkov na ochranu osobných údajov v balíku Office pre Mac pomocou predvolieb.
hideEdit: true
ms.openlocfilehash: 01bb31f3b6c307ec1dc4762b54fea17185dcf27d
ms.sourcegitcommit: 0fd23324ba1364fa1f8dd1578adf25946adde90f
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246322"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a><span data-ttu-id="75476-103">Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb</span><span class="sxs-lookup"><span data-stu-id="75476-103">Use preferences to manage privacy controls for Office for Mac</span></span>

<span data-ttu-id="75476-104">Od verzie 16.28 balíka Office pre Mac sú k dispozícii nové nastavenia predvolieb, ktoré umožňujú ovládať nastavenia týkajúce sa:</span><span class="sxs-lookup"><span data-stu-id="75476-104">Starting with Version 1904 of Office 365 ProPlus, there are new policy settings that will allow you to control settings related to the following:</span></span>

- <span data-ttu-id="75476-105">***Diagnostických údajov***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.</span><span class="sxs-lookup"><span data-stu-id="75476-105">***Diagnostic data*** that is collected and sent to Microsoft about Office client software being used</span></span>

- <span data-ttu-id="75476-106">***Online funkcií***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.</span><span class="sxs-lookup"><span data-stu-id="75476-106">***Connected experiences*** that use cloud-based functionality to provide enhanced Office features to you and your users.</span></span>

<span data-ttu-id="75476-107">Okrem toho je k dispozícii nové nastavenie predvolieb týkajúce sa dialógového okna **Oznámenie o požadovaných údajoch** pre službu Microsoft AutoUpdate (MAU).</span><span class="sxs-lookup"><span data-stu-id="75476-107">In addition, there is a new preference setting related to a **Required Data Notice** dialog for Microsoft AutoUpdate (MAU).</span></span>

<span data-ttu-id="75476-108">Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).</span><span class="sxs-lookup"><span data-stu-id="75476-108">For more information about diagnostic data and connected experiences, see [Overview of privacy controls](overview-privacy-controls.md).</span></span>

> [!NOTE]
> <span data-ttu-id="75476-109">Ďalšie informácie o podobných nastaveniach balíka Office v počítačoch s Windowsom nájdete v téme [Spravovanie ovládacích prvkov ochrany osobných údajov pre Office 365 ProPlus pomocou nastavení politiky](manage-privacy-controls.md)</span><span class="sxs-lookup"><span data-stu-id="75476-109">For information about similar settings for Office on computers running Windows, see [Use policy settings to manage privacy controls for Office 365 ProPlus](manage-privacy-controls.md)</span></span>

## <a name="setting-preferences"></a><span data-ttu-id="75476-110">Nastavenie predvolieb</span><span class="sxs-lookup"><span data-stu-id="75476-110">Setting preferences</span></span>

<span data-ttu-id="75476-111">Tieto nové predvoľby sú kompatibilné s metódami CFPreferences rozhrania API a je možné ich nastaviť pomocou príkazu `defaults` v Termináli alebo ako vynútené predvoľby prostredníctvom konfiguračného profilu alebo servera Mobile Device Management (MDM).</span><span class="sxs-lookup"><span data-stu-id="75476-111">These new preference settings are CFPreferences API compatible and can be set using the `defaults` command in Terminal, or enforced through a Configuration Profile or Mobile Device Management (MDM) server.</span></span> <span data-ttu-id="75476-112">V prípade vynútených predvolieb používateľ nemôže zmeniť ich hodnoty a všetky ovládacie prvky v aplikácii budú zobrazené ako neaktívne.</span><span class="sxs-lookup"><span data-stu-id="75476-112">When the preferences are enforced, the user cannot change the values, and any in-app controls will appear disabled.</span></span>

## <a name="preference-setting-for-diagnostic-data"></a><span data-ttu-id="75476-113">Nastavenia predvolieb pre diagnostické údaje</span><span class="sxs-lookup"><span data-stu-id="75476-113">Policy setting for diagnostic data</span></span>

<span data-ttu-id="75476-114">Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov.</span><span class="sxs-lookup"><span data-stu-id="75476-114">Diagnostic data is used to keep Office secure and up-to-date, detect, diagnose and remediate problems, and also make product improvements.</span></span> <span data-ttu-id="75476-115">Ďalšie informácie nájdete v téme [Diagnostické údaje odosielané zo služieb Office 365 ProPlus spoločnosti Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-office-365-proplus-to-microsoft).</span><span class="sxs-lookup"><span data-stu-id="75476-115">Diagnostic data sent from Office 365 ProPlus to Microsoft</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75476-116">**Doména predvolieb**</span><span class="sxs-lookup"><span data-stu-id="75476-116">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="75476-117">**Kód**</span><span class="sxs-lookup"><span data-stu-id="75476-117">**Key**</span></span>  | `DiagnosticDataTypePreference`  |
|<span data-ttu-id="75476-118">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="75476-118">**Data Type**</span></span>  | <span data-ttu-id="75476-119">Reťazec</span><span class="sxs-lookup"><span data-stu-id="75476-119">String</span></span> |
|<span data-ttu-id="75476-120">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="75476-120">**Possible values**</span></span>  | <span data-ttu-id="75476-121">`BasicDiagnosticData` *(nastaví sa úroveň Požadované)*</span><span class="sxs-lookup"><span data-stu-id="75476-121">`BasicDiagnosticData` *(this sets the level to Required)*</span></span> <br/> <span data-ttu-id="75476-122">`FullDiagnosticData` *(nastaví sa úroveň Voliteľné)*</span><span class="sxs-lookup"><span data-stu-id="75476-122">`FullDiagnosticData` *(this sets the level to Optional)*</span></span> <br/> <span data-ttu-id="75476-123">`ZeroDiagnosticData` *(nastaví sa úroveň Žiadne)*</span><span class="sxs-lookup"><span data-stu-id="75476-123">`ZeroDiagnosticData` *(this sets the level to Neither)*</span></span> |
|<span data-ttu-id="75476-124">**Dostupnosť**</span><span class="sxs-lookup"><span data-stu-id="75476-124">**Availability**</span></span> |<span data-ttu-id="75476-125">Verzia 16.28 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="75476-125">16.28 and later</span></span> |

> [!NOTE]
> <span data-ttu-id="75476-126">Ak nastavíte túto predvoľbu, použije sa aj v nasledujúcich produktoch:</span><span class="sxs-lookup"><span data-stu-id="75476-126">If you set this preference, it also will apply to the following products:</span></span>
> - <span data-ttu-id="75476-127">Verzia 1.00.217856 a novšie verzie aplikácie Teams pre Mac</span><span class="sxs-lookup"><span data-stu-id="75476-127">Version 1.00.217856 and later of Teams for Mac</span></span>
> - <span data-ttu-id="75476-128">Verzia 16.28 a novšie verzie Skypu for Business pre Mac</span><span class="sxs-lookup"><span data-stu-id="75476-128">Version 16.28 and later of Skype for Business for Mac</span></span>

<span data-ttu-id="75476-129">Ak túto predvoľbu nenastavíte, v prípade, že sa používatelia s predplatným na Office 365 prihlásili pomocou pracovného alebo školského konta, alebo ak majú používatelia multilicenčnú verziu balíka Office 2019 pre Mac, spoločnosti Microsoft sa odošlú voliteľné aj požadované diagnostické údaje.</span><span class="sxs-lookup"><span data-stu-id="75476-129">If you don't set this preference, both optional and required diagnostic data is sent to Microsoft if users with an Office 365 subscription are signed in with a work or school account or if users have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="75476-130">Títo používatelia si tiež nemôžu zmeniť úroveň diagnostických údajov, bez ohľadu na to, ako ste túto predvoľbu nastavili.</span><span class="sxs-lookup"><span data-stu-id="75476-130">Also, these users can't change the level of diagnostic data regardless of how you set this preference.</span></span>

<span data-ttu-id="75476-131">V prípade ostatných používateľov, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, sa odošlú iba požadované diagnostické údaje, pokiaľ si používateľ nezvolí možnosť odosielať aj voliteľné diagnostické údaje v okne **Predvoľby** > **Ochrana osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="75476-131">For other users, such as home users with an Office 365 subscription, only required diagnostic data is sent, unless the user chooses to also send optional diagnostic data by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a><span data-ttu-id="75476-132">Nastavenia predvolieb pre online funkcie na analýzu obsahu</span><span class="sxs-lookup"><span data-stu-id="75476-132">Policy setting for connected experiences that analyze your content</span></span>

<span data-ttu-id="75476-133">Online funkcie na analýzu obsahu sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií.</span><span class="sxs-lookup"><span data-stu-id="75476-133">Connected experiences that analyze your content are experiences that use your Office content to provide you with design recommendations, editing suggestions, data insights, and similar features.</span></span> <span data-ttu-id="75476-134">Príkladmi sú PowerPoint Designer alebo Vyhľadávač vo Worde.</span><span class="sxs-lookup"><span data-stu-id="75476-134">For example, PowerPoint Designer or Editor in Word.</span></span> <span data-ttu-id="75476-135">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="75476-135">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75476-136">**Doména predvolieb**</span><span class="sxs-lookup"><span data-stu-id="75476-136">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="75476-137">**Kód**</span><span class="sxs-lookup"><span data-stu-id="75476-137">**Key**</span></span>  | `OfficeExperiencesAnalyzingContentPreference`  |
|<span data-ttu-id="75476-138">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="75476-138">**Data Type**</span></span>  | <span data-ttu-id="75476-139">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="75476-139">Boolean</span></span> |
|<span data-ttu-id="75476-140">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="75476-140">**Possible values**</span></span>  | <span data-ttu-id="75476-141">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="75476-141">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="75476-142">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="75476-142">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="75476-143">**Dostupnosť**</span><span class="sxs-lookup"><span data-stu-id="75476-143">**Availability**</span></span> |<span data-ttu-id="75476-144">Verzia 16.28 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="75476-144">16.28 and later</span></span> |

<span data-ttu-id="75476-145">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na analýzu obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="75476-145">If you don't set this preference, connected experiences that analyze content are available to users.</span></span> 

<span data-ttu-id="75476-146">Ak používatelia majú predplatné na Office 365 a sú prihlásení s pracovným alebo školským kontom, alebo ak majú multilicenčnú verziu balíka Office 2019 pre Mac, nemôžu online funkcie na analýzu obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="75476-146">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that analyze content.</span></span>

<span data-ttu-id="75476-147">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, majú možnosť online funkcie na analýzu obsahu vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="75476-147">For other users, such as home users with an Office 365 subscription, the user can choose to turn off connected experiences that analyze content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a><span data-ttu-id="75476-148">Nastavenie predvolieb pre online funkcie na sťahovanie online obsahu</span><span class="sxs-lookup"><span data-stu-id="75476-148">Policy setting for connected experiences that download online content</span></span>

<span data-ttu-id="75476-149">Online funkcie na sťahovanie online obsahu sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, 3D modelov, videí a referenčných materiálov na vylepšenie vašich dokumentov.</span><span class="sxs-lookup"><span data-stu-id="75476-149">Connected experiences that download online content are experiences that allow you to search and download online content including templates, images, 3D models, videos, and reference materials to enhance your documents.</span></span> <span data-ttu-id="75476-150">Napríklad šablóny balíka Office alebo funkcia Rýchly štart pre PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="75476-150">For example, Office templates or PowerPoint QuickStarter.</span></span> <span data-ttu-id="75476-151">Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="75476-151">For a list of these connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75476-152">**Doména predvolieb**</span><span class="sxs-lookup"><span data-stu-id="75476-152">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="75476-153">**Kód**</span><span class="sxs-lookup"><span data-stu-id="75476-153">**Key**</span></span>  | `OfficeExperiencesDownloadingContentPreference`  |
|<span data-ttu-id="75476-154">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="75476-154">**Data Type**</span></span>  | <span data-ttu-id="75476-155">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="75476-155">Boolean</span></span> |
|<span data-ttu-id="75476-156">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="75476-156">**Possible values**</span></span>  | <span data-ttu-id="75476-157">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="75476-157">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="75476-158">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="75476-158">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="75476-159">**Dostupnosť**</span><span class="sxs-lookup"><span data-stu-id="75476-159">**Availability**</span></span> |<span data-ttu-id="75476-160">Verzia 16.28 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="75476-160">16.28 and later</span></span> |

<span data-ttu-id="75476-161">Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na sťahovanie online obsahu k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="75476-161">If you don't set this preference, connected experiences that download online content are available to users.</span></span>

<span data-ttu-id="75476-162">Ak používatelia majú predplatné na Office 365 a sú prihlásení s pracovným alebo školským kontom, alebo ak majú multilicenčnú verziu balíka Office 2019 pre Mac, nemôžu online funkcie na sťahovanie online obsahu vypnúť.</span><span class="sxs-lookup"><span data-stu-id="75476-162">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off connected experiences that download online content.</span></span>

<span data-ttu-id="75476-163">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, majú možnosť online funkcie na sťahovanie online obsahu vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="75476-163">For other users, such as home users with an Office 365 subscription, a user can choose to turn off connected experiences that download online content by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-optional-connected-experiences"></a><span data-ttu-id="75476-164">Nastavenia predvolieb pre voliteľné online funkcie</span><span class="sxs-lookup"><span data-stu-id="75476-164">Policy setting for optional connected experiences</span></span>

<span data-ttu-id="75476-165">Okrem online funkcií uvedených vyššie existujú aj voliteľné online funkcie, ku ktorým môžete používateľom povoliť prístup prostredníctvom ich konta organizácie, ktoré sa niekedy označuje ako pracovné alebo školské konto.</span><span class="sxs-lookup"><span data-stu-id="75476-165">In addition to the connected experiences mentioned above, there are some optional connected experiences that you may choose to allow your users to access with their organization account, which is sometimes referred to as a work or school account.</span></span> <span data-ttu-id="75476-166">Napríklad funkcie LinkedInu v asistentovi životopisu vo Worde alebo panel počasia v Outlooku, ktorý využíva službu MSN Počasie.</span><span class="sxs-lookup"><span data-stu-id="75476-166">For example, the LinkedIn features of the Resume Assistant in Word or the 3D Maps feature in Excel, which uses Bing.</span></span> <span data-ttu-id="75476-167">Ďalšie príklady nájdete v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="75476-167">For more examples, see [Overview of optional connected experiences in Office](optional-connected-experiences.md).</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75476-168">**Doména predvolieb**</span><span class="sxs-lookup"><span data-stu-id="75476-168">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="75476-169">**Kód**</span><span class="sxs-lookup"><span data-stu-id="75476-169">**Key**</span></span>  | `OptionalConnectedExperiencesPreference`  |
|<span data-ttu-id="75476-170">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="75476-170">**Data Type**</span></span>  | <span data-ttu-id="75476-171">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="75476-171">Boolean</span></span> |
|<span data-ttu-id="75476-172">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="75476-172">**Possible values**</span></span>  | <span data-ttu-id="75476-173">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="75476-173">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="75476-174">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="75476-174">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="75476-175">**Dostupnosť**</span><span class="sxs-lookup"><span data-stu-id="75476-175">**Availability**</span></span> |<span data-ttu-id="75476-176">Verzia 16.28 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="75476-176">16.28 and later</span></span> |

<span data-ttu-id="75476-177">Ak túto predvoľbu nenastavíte, voliteľné online funkcie sú používateľom k dispozícii v prípade, že sa používatelia s predplatným na Office 365 prihlásili pomocou pracovného alebo školského konta, alebo ak používatelia majú multilicenčnú verziu balíka Office 2019 pre Mac.</span><span class="sxs-lookup"><span data-stu-id="75476-177">If you don't set this preference, optional connected experiences are available to users with an Office 365 subscription that are signed in with a work or school account or users who have a volume licensed version of Office 2019 for Mac.</span></span> <span data-ttu-id="75476-178">Ako ste túto predvoľbu nenastavili na hodnotu `FALSE`, títo používatelia majú možnosť voliteľné online funkcie vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="75476-178">Unless you have set this preference to `FALSE`, these users can choose to turn off optional connected experiences by going to **Preferences** > **Privacy**.</span></span>

<span data-ttu-id="75476-179">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, nemajú možnosť vypnúť voliteľné online funkcie.</span><span class="sxs-lookup"><span data-stu-id="75476-179">For other users, such as home users with an Office 365 subscription, there isn't an option to turn off optional connected experiences.</span></span>

## <a name="preference-setting-for-most-connected-experiences"></a><span data-ttu-id="75476-180">Nastavenia predvolieb pre väčšinu online funkcií</span><span class="sxs-lookup"><span data-stu-id="75476-180">Policy setting for most connected experiences</span></span>

<span data-ttu-id="75476-181">Pomocou tejto možnosti môžete určiť, či budú mať vaši používatelia k dispozícii väčšinu online funkcií.</span><span class="sxs-lookup"><span data-stu-id="75476-181">You can use this preference to control whether most connected experiences are available to your users.</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75476-182">**Doména predvolieb**</span><span class="sxs-lookup"><span data-stu-id="75476-182">**Preference Domain**</span></span>  | `com.microsoft.office` |
|<span data-ttu-id="75476-183">**Kód**</span><span class="sxs-lookup"><span data-stu-id="75476-183">**Key**</span></span>  | `ConnectedOfficeExperiencesPreference`  |
|<span data-ttu-id="75476-184">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="75476-184">**Data Type**</span></span>  | <span data-ttu-id="75476-185">Boolovská hodnota</span><span class="sxs-lookup"><span data-stu-id="75476-185">Boolean</span></span> |
|<span data-ttu-id="75476-186">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="75476-186">**Possible values**</span></span>  | <span data-ttu-id="75476-187">`TRUE` *(povolené)*</span><span class="sxs-lookup"><span data-stu-id="75476-187">`TRUE` *(enabled)*</span></span> <br/> <span data-ttu-id="75476-188">`FALSE` *(zakázané)*</span><span class="sxs-lookup"><span data-stu-id="75476-188">`FALSE` *(disabled)*</span></span>|
|<span data-ttu-id="75476-189">**Dostupnosť**</span><span class="sxs-lookup"><span data-stu-id="75476-189">**Availability**</span></span> |<span data-ttu-id="75476-190">Verzia 16.28 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="75476-190">16.28 and later</span></span> |

<span data-ttu-id="75476-191">Ak túto predvoľbu nenastavíte, vaši používatelia majú k dispozícii všetky online funkcie, pokiaľ ste nenastavili niektorú z ďalších predvolieb pre online funkcie, ktoré sú spomenuté vyššie, ako napríklad predvoľbu `OfficeExperiencesAnalyzingContentPreference`.</span><span class="sxs-lookup"><span data-stu-id="75476-191">If you don't set this preference, all connected experiences are available to your users, unless you have set one of the other preferences for connected experiences previously mentioned, such as `OfficeExperiencesAnalyzingContentPreference`.</span></span>

<span data-ttu-id="75476-192">Ak napríklad túto predvoľbu nastavíte na hodnotu `FALSE`, tieto typy online funkcií nebudú vašim používateľom k dispozícii:</span><span class="sxs-lookup"><span data-stu-id="75476-192">For example, if you set this preference to `FALSE`, the following types of connected experiences won't be available to your users:</span></span>
- <span data-ttu-id="75476-193">Funkcie na analýzu obsahu</span><span class="sxs-lookup"><span data-stu-id="75476-193">Experiences that analyze your content</span></span>
- <span data-ttu-id="75476-194">Funkcie na sťahovanie online obsahu</span><span class="sxs-lookup"><span data-stu-id="75476-194">Experiences that download online content</span></span>
- <span data-ttu-id="75476-195">Voliteľné online funkcie</span><span class="sxs-lookup"><span data-stu-id="75476-195">Optional connected experiences</span></span>

<span data-ttu-id="75476-196">Okrem toho platí, že ak túto predvoľbu nastavíte na hodnou `FALSE`, vypne sa aj väčšina ostatných online funkcií, ako sú napríklad spolutvorba dokumentov a online ukladací priestor súborov.</span><span class="sxs-lookup"><span data-stu-id="75476-196">In addition, if you disable this policy setting, most other connected experiences are also turned off, such as co-authoring and online file storage.</span></span> <span data-ttu-id="75476-197">Zoznam týchto ostatných online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="75476-197">For a list of these other connected experiences, see [Connected experiences in Office](connected-experiences.md).</span></span>

<span data-ttu-id="75476-198">Aj keď túto predvoľbu nastavíte na hodnotu `FALSE`, niektoré funkcie balíka Office zostanú dostupné, napríklad synchronizácia poštovej schránky v Outlooku, a aplikácie Teams a Skype for Business budú aj naďalej fungovať.</span><span class="sxs-lookup"><span data-stu-id="75476-198">But even if you disable this policy setting, limited Office functionality will remain available, such as synching a mailbox in Outlook, and Teams and Skype for Business will continue to work.</span></span> <span data-ttu-id="75476-199">[Nevyhnutné služby](essential-services.md), ako je napríklad licenčná služba, ktorá potvrdzuje, že máte správnu licenciu na používanie služieb Office, takisto zostanú k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="75476-199">[Essential services](essential-services.md), such as the licensing service that confirms that you’re properly licensed to use Office, will also remain available.</span></span>

<span data-ttu-id="75476-200">Ak používatelia majú predplatné na Office 365 a sú prihlásení s pracovným alebo školským kontom, alebo ak majú multilicenčnú verziu balíka Office 2019 pre Mac, nemôžu väčšinu online funkcií vypnúť.</span><span class="sxs-lookup"><span data-stu-id="75476-200">If the user has an Office 365 subscription and is signed in with a work or school account or if the user has a volume licensed version of Office 2019 for Mac, then the user can't turn off most connected experiences.</span></span>

<span data-ttu-id="75476-201">Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365, majú možnosť väčšinu online funkcií vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.</span><span class="sxs-lookup"><span data-stu-id="75476-201">For other users, such as home users with an Office 365 subscription, a user can choose to turn off most connected experiences by going to **Preferences** > **Privacy**.</span></span>

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a><span data-ttu-id="75476-202">Nastavenie predvolieb pre dialógové okno Oznámenie o požadovaných údajoch pre službu Microsoft AutoUpdate</span><span class="sxs-lookup"><span data-stu-id="75476-202">Preference setting for the Required Data Notice dialog for Microsoft AutoUpdate</span></span>

<span data-ttu-id="75476-203">Pri prvom spustení verzie 4.12 alebo novšej verzie služby Microsoft AutoUpdate (MAU) sa používateľom zobrazí dialógové okno **Oznámenie o požadovaných údajoch** s informáciami o tom, aké údaje služby MAU sa odosielajú spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="75476-203">The first time Version 4.12 or later of Microsoft AutoUpdate (MAU) is launched, users will see a **Required Data Notice** dialog which provides them with information about what data from MAU is sent to Microsoft.</span></span>

<span data-ttu-id="75476-204">Ak nechcete, aby sa používateľom dialógové okno **Oznámenie o požadovaných údajoch** pre službu Microsoft AutoUpdate zobrazilo, môžete nastaviť nasledujúcu predvoľbu.</span><span class="sxs-lookup"><span data-stu-id="75476-204">If you don't want your users to see this **Required Data Notice** dialog for Microsoft AutoUpdate, you can set the following preference.</span></span> <span data-ttu-id="75476-205">Dialógové okno sa používateľom nezobrazí bez ohľadu na to, ktorú hodnotu nastavíte.</span><span class="sxs-lookup"><span data-stu-id="75476-205">Regardless of which value you set, the dialog won't be shown to your users.</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75476-206">**Doména predvolieb**</span><span class="sxs-lookup"><span data-stu-id="75476-206">**Preference Domain**</span></span>  | `com.microsoft.autoupdate2` |
|<span data-ttu-id="75476-207">**Kód**</span><span class="sxs-lookup"><span data-stu-id="75476-207">**Key**</span></span>  | `AcknowledgedDataCollectionPolicy`  |
|<span data-ttu-id="75476-208">**Typ údajov**</span><span class="sxs-lookup"><span data-stu-id="75476-208">**Data Type**</span></span>  | <span data-ttu-id="75476-209">Reťazec</span><span class="sxs-lookup"><span data-stu-id="75476-209">String</span></span> |
|<span data-ttu-id="75476-210">**Možné hodnoty**</span><span class="sxs-lookup"><span data-stu-id="75476-210">**Possible values**</span></span>  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|<span data-ttu-id="75476-211">**Dostupnosť**</span><span class="sxs-lookup"><span data-stu-id="75476-211">**Availability**</span></span> |<span data-ttu-id="75476-212">Verzia 4.12 a novšie verzie</span><span class="sxs-lookup"><span data-stu-id="75476-212">4.12 and later</span></span> |

<span data-ttu-id="75476-213">Ak umožníte, aby sa toto dialógové okno používateľom zobrazilo, používatelia môžu kliknutím na tlačidlo **OK** zapísať do politiky `AcknowledgedDataCollectionPolicy` hodnotu `RequiredDataOnly` a tým nastaviť, aby sa im dialógové okno nezobrazovalo znova.</span><span class="sxs-lookup"><span data-stu-id="75476-213">If you let your users see this dialog, then when the user chooses **OK**, the value `RequiredDataOnly` is written to `AcknowledgedDataCollectionPolicy` and the dialog is not shown to the user again.</span></span>


## <a name="related-topics"></a><span data-ttu-id="75476-214">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="75476-214">Related topics</span></span>

- [<span data-ttu-id="75476-215">Informácie o konfiguračnom profile (dokumentácia pre vývojárov Apple)</span><span class="sxs-lookup"><span data-stu-id="75476-215">Configuration Profile Reference (Apple developer documentation)</span></span>](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [<span data-ttu-id="75476-216">Nasadenie predvolieb pre Office pre Mac</span><span class="sxs-lookup"><span data-stu-id="75476-216">Deploy preferences for Office for Mac</span></span>](../mac/deploy-preferences-for-office-for-mac.md)
- [<span data-ttu-id="75476-217">Nastavenia ochrany osobných údajov konta</span><span class="sxs-lookup"><span data-stu-id="75476-217">Account Privacy Settings</span></span>](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)
