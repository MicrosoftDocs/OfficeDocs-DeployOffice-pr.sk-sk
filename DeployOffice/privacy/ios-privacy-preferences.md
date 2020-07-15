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
# <a name="use-preferences-to-manage-privacy-controls-for-office-on-ios-devices"></a>Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb

K dispozícii sú nové nastavenia predvolieb pre Office v zariadeniach so systémom iOS, ktoré umožňujú ovládať nastavenia pre:

- ***Diagnostické údaje***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.

- ***Online funkcie***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.

Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).

Tieto nastavenia predvolieb sa týkajú aplikácií:
- Word pre iOS, Excel pre iOS a PowerPoint pre iOS verzie 2.30 a novšej.
- Outlook pre iOS verzie 4.30.0 a novšej.
- OneNote pre iOS verzie 16.30 a novšej.
- OneDrive pre iOS verzie 11.19.11 a novšej.
- Visio Viewer pre iOS verzie 1.17 a novšej.
- Aplikácia Office pre iOS verzie 2.34 a novšej.

> [!NOTE]
> Ďalšie informácie o podobných nastaveniach balíka Office v počítačoch so systémom macOS nájdete v téme [Spravovanie ovládacích prvkov ochrany osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md).


## <a name="setting-device-preferences"></a>Nastavenie predvolieb zariadenia
Tieto nové nastavenia predvolieb je možné nastaviť aj na úrovni zariadenia prostredníctvom servera správy mobilných zariadení (MDM), keď je aplikácia balíka Office už nainštalovaná. Mnohé MDM servery umožňujú správcom IT pridať voliteľný konfiguračný slovník, keď server odošle MDM príkaz `InstallApplication` do zariadenia so systémom iOS. Ďalšie informácie nájdete v dokumentácii k MDM serveru.

Slovník je vyjadrený ako množina dvojíc kľúča a hodnoty vo formáte XML. Príklad:

```xml
<dict>
    <key>DiagnosticDataTypePreference</key>
    <string>BasicDiagnosticData</string>
</dict>
```

Po odoslaní do zariadenia sa konfiguračný slovník bude nachádzať v kľúči `com.apple.managed.configuration`, kde sa prečíta, keď sa spustí aplikácia balíka Office.

> [!NOTE]
> Môžete použiť aj cloudovú službu politiky pre Office a tieto 4 nastavenia politiky:
> - Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft
> - Povoliť používanie pripojených funkcií na analýzu obsahu v Office
> - Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office
> - Povoliť používanie dodatočných voliteľných pripojených funkcií v Office
>
> Nastavenia ochrany osobných údajov pre Outlook pre iOS a OneDrive pre iOS je možné nakonfigurovať iba pomocou cloudovej služby politiky pre Office.
>
> Ďalšie informácie o použití cloudovej služby politiky pre Office nájdete v téme [Prehľad cloudovej služby politiky pre Office](../overview-office-cloud-policy-service.md).

## <a name="preference-setting-for-diagnostic-data"></a>Nastavenia predvolieb pre diagnostické údaje

Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov. Ďalšie informácie nájdete v téme [Diagnostické údaje odoslané z Aplikácií Microsoft 365 pre veľké organizácie do spoločnosti Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).

|||
|:-----|:-----|
|**Kód**  | `DiagnosticDataTypePreference`  |
|**Typ údajov**  | Reťazec |
|**Možné hodnoty**  | `BasicDiagnosticData` *(nastaví sa úroveň Požadované)* <br/> `FullDiagnosticData` *(nastaví sa úroveň Voliteľné)* <br/> `ZeroDiagnosticData` *(nastaví sa úroveň Žiadne)* |

Ak túto predvoľbu nenastavíte, v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta, spoločnosti Microsoft sa odošlú len požadované diagnostické údaje. Títo používatelia si tiež nemôžu zmeniť úroveň diagnostických údajov, bez ohľadu na to, ako ste túto predvoľbu nastavili.

V prípade ostatných používateľov, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), sa odosielajú iba požadované diagnostické údaje, pokiaľ si používateľ nezvolí možnosť odosielať aj voliteľné diagnostické údaje v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.


## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Nastavenia predvolieb pre online funkcie na analýzu obsahu

Online funkcie na analýzu obsahu sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií. Napríklad Návrhy vzhľadu v PowerPointe. Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).

|||
|:-----|:-----|
|**Kód**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Typ údajov**  | Boolovská hodnota |
|**Možné hodnoty**  | `TRUE` *(povolené)* <br/> `FALSE` *(zakázané)*|


Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na analýzu obsahu k dispozícii.

Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na analýzu obsahu vypnúť.

Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na analýzu obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Nastavenie predvolieb pre online funkcie na sťahovanie online obsahu

Online funkcie na sťahovanie online obsahu sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, videí a referenčných materiálov na vylepšenie vašich dokumentov. Napríklad šablóny balíka Office alebo funkcia vloženie online ikony. Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).

|||
|:-----|:-----|
|**Kód**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Typ údajov**  | Boolovská hodnota |
|**Možné hodnoty**  | `TRUE` *(povolené)* <br/> `FALSE` *(zakázané)*|


Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na sťahovanie online obsahu k dispozícii.

Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, nemôžu online funkcie na sťahovanie online obsahu vypnúť.

Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na sťahovanie online obsahu vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Nastavenia predvolieb pre voliteľné online funkcie

Okrem online funkcií uvedených vyššie existujú aj voliteľné online funkcie, ku ktorým môžete používateľom povoliť prístup prostredníctvom ich konta organizácie, ktoré sa niekedy označuje ako pracovné alebo školské konto. Napríklad doplnky balíka Office, ktoré sa do zariadenia sťahujú cez Office Obchod. Ďalšie príklady nájdete v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md)

|||
|:-----|:-----|
|**Kód**  | `OptionalConnectedExperiencesPreference`  |
|**Typ údajov**  | Boolovská hodnota |
|**Možné hodnoty**  | `TRUE` *(povolené)* <br/> `FALSE` *(zakázané)*|


Ak túto predvoľbu nenastavíte, voliteľné online funkcie sú používateľom k dispozícii v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta. Ako ste túto predvoľbu nenastavili na hodnotu FALSE, títo používatelia majú možnosť voliteľné online funkcie vypnúť v okne **Nastavenia** > **Nastavenia ochrany osobných údajov**.

Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), nemajú možnosť vypnúť voliteľné online funkcie.