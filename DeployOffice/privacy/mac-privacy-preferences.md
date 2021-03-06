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
description: V tomto článku správcovia služieb Office získajú informácie o postupoch spravovania ovládacích prvkov na ochranu osobných údajov v balíku Office pre Mac pomocou predvolieb.
hideEdit: true
ms.openlocfilehash: b7beda7409cff00d54f36851eb21e4d66a8cacce
ms.sourcegitcommit: 9b5f18c543c286c95e546e22fc8edb60ef541030
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52578387"
---
# <a name="use-preferences-to-manage-privacy-controls-for-office-for-mac"></a>Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb

> [!NOTE]
> Ak si chcete pozrieť zoznam produktov balíka Office, na ktorý sa vzťahujú tieto informácie o ochrane osobných údajov, pozrite si tému [Ovládacie prvky na ochranu osobných údajov dostupné pre produkty balíka Office](products-versions-privacy-controls.md).

Od verzie 16.28 balíka Office pre Mac sú k dispozícii nové nastavenia predvolieb, ktoré umožňujú ovládať nastavenia týkajúce sa:

- ***Diagnostických údajov***, ktoré sa zhromažďujú a odosielajú spoločnosti Microsoft o používanom klientskom softvéri balíka Office.

- ***Online funkcií***, ktoré využívajú cloudové funkcie na poskytovanie rozšírených funkcií balíka Office vám a vašim používateľom.

Okrem toho je k dispozícii nové nastavenie predvolieb týkajúce sa dialógového okna **Oznámenie o požadovaných údajoch** pre službu Microsoft AutoUpdate (MAU).

Ďalšie informácie o diagnostických údajoch a online funkciách nájdete v téme [Prehľad ovládacích prvkov na ochranu osobných údajov](overview-privacy-controls.md).

> [!NOTE]
> - Ďalšie informácie o podobných nastaveniach balíka Office v počítačoch s Windowsom nájdete v téme [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie](manage-privacy-controls.md)
> - Ďalšie informácie o podobných nastaveniach balíka Office v zariadeniach so systémom iOS nájdete v téme [Spravovanie ovládacích prvkov ochrany osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb](ios-privacy-preferences.md).

## <a name="setting-preferences"></a>Nastavenie predvolieb

Tieto nové predvoľby sú kompatibilné s metódami CFPreferences rozhrania API a je možné ich nastaviť pomocou príkazu `defaults` v Termináli alebo ako vynútené predvoľby prostredníctvom konfiguračného profilu alebo servera Mobile Device Management (MDM). V prípade vynútených predvolieb používateľ nemôže zmeniť ich hodnoty a všetky ovládacie prvky v aplikácii budú zobrazené ako neaktívne.

> [!NOTE]
> Môžete použiť aj cloudovú službu politiky pre Office a týchto 5 nastavení politiky:
> - Konfigurácia úrovne diagnostických údajov o klientskom softvéri, ktoré služby Office odosielajú spoločnosti Microsoft
> - Povoliť používanie pripojených funkcií na analýzu obsahu v Office
> - Povoliť používanie pripojených funkcií na sťahovanie online obsahu v Office
> - Povoliť používanie dodatočných voliteľných pripojených funkcií v Office
> - Povoliť používanie pripojených funkcií v Office
>
> Ďalšie informácie o použití cloudovej služby politiky pre Office nájdete v téme [Prehľad cloudovej služby politiky pre Office](../overview-office-cloud-policy-service.md).


## <a name="preference-setting-for-diagnostic-data"></a>Nastavenia predvolieb pre diagnostické údaje

Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov. Ďalšie informácie nájdete v téme [Diagnostické údaje odoslané z Aplikácií Microsoft 365 pre veľké organizácie do spoločnosti Microsoft](overview-privacy-controls.md#diagnostic-data-sent-from-microsoft-365-apps-for-enterprise-to-microsoft).

|Kategória|Podrobnosti|
|:-----|:-----|
|**Doména predvolieb**  | `com.microsoft.office` |
|**Kód**  | `DiagnosticDataTypePreference`  |
|**Typ údajov**  | Reťazec |
|**Možné hodnoty**  | `BasicDiagnosticData` *(táto hodnota nastaví úroveň na možnosť Požadované)* <br/> `FullDiagnosticData` *(táto hodnota nastaví úroveň na možnosť Voliteľné)* <br/> `ZeroDiagnosticData` *(táto hodnota nastaví úroveň na možnosť Žiadne)* |
|**Dostupnosť** |Verzia 16.28 a novšie verzie |

Ak túto predvoľbu nenastavíte, v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta, alebo ak používatelia majú multilicenčnú verziu balíka Office 2019 pre Mac, spoločnosti Microsoft sa odosielajú požadované aj voliteľné diagnostické údaje. Títo používatelia si tiež nemôžu zmeniť úroveň diagnostických údajov, bez ohľadu na to, ako ste túto predvoľbu nastavili.

> [!NOTE]
> Aktualizovali sme predchádzajúci odsek, aby sme objasnili, že ak túto predvoľbu nenastavíte, spoločnosti Microsoft sa odošlú aj voliteľné diagnostické údaje.

V prípade ostatných používateľov, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), sa odosielajú iba požadované diagnostické údaje, pokiaľ si používateľ nezvolí možnosť odosielať aj voliteľné diagnostické údaje v okne **Predvoľby** > **Ochrana osobných údajov**.

## <a name="preference-setting-for-connected-experiences-that-analyze-your-content"></a>Nastavenia predvolieb pre online funkcie na analýzu obsahu

Online funkcie na analýzu obsahu sú funkcie, ktoré používajú obsah balíka Office na poskytovanie odporúčaní pre návrh, úprav návrhov, prehľadov údajov a podobných funkcií. Príkladmi sú PowerPoint Designer alebo Vyhľadávač vo Worde. Zoznam týchto online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).

|Kategória|Podrobnosti|
|:-----|:-----|
|**Doména predvolieb**  | `com.microsoft.office` |
|**Kód**  | `OfficeExperiencesAnalyzingContentPreference`  |
|**Typ údajov**  | Boolovská hodnota |
|**Možné hodnoty**  | `TRUE` *(povolené)* <br/> `FALSE` *(zakázané)*|
|**Dostupnosť** |Verzia 16.28 a novšie verzie |

Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na analýzu obsahu k dispozícii. 

Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, alebo ak majú multilicenčnú verziu balíka Office 2019 pre Mac, nemôžu online funkcie na analýzu obsahu vypnúť.

Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na analýzu obsahu vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.

## <a name="preference-setting-for-connected-experiences-that-download-online-content"></a>Nastavenie predvolieb pre online funkcie na sťahovanie online obsahu

Online funkcie na sťahovanie online obsahu sú funkcie, ktoré umožňujú vyhľadať a sťahovať online obsah vrátane šablón, obrázkov, 3D modelov, videí a referenčných materiálov na vylepšenie vašich dokumentov. Napríklad šablóny balíka Office alebo funkcia Rýchly štart pre PowerPoint. Zoznam týchto pripojených funkcií nájdete v téme [Pripojené funkcie v Office](connected-experiences.md).

|Kategória|Podrobnosti|
|:-----|:-----|
|**Doména predvolieb**  | `com.microsoft.office` |
|**Kód**  | `OfficeExperiencesDownloadingContentPreference`  |
|**Typ údajov**  | Boolovská hodnota |
|**Možné hodnoty**  | `TRUE` *(povolené)* <br/> `FALSE` *(zakázané)*|
|**Dostupnosť** |Verzia 16.28 a novšie verzie |

Ak túto predvoľbu nenastavíte, používatelia budú mať online funkcie na sťahovanie online obsahu k dispozícii.

Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, alebo ak majú multilicenčnú verziu balíka Office 2019 pre Mac, nemôžu online funkcie na sťahovanie online obsahu vypnúť.

Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť online funkcie na sťahovanie online obsahu vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.

## <a name="preference-setting-for-optional-connected-experiences"></a>Nastavenia predvolieb pre voliteľné online funkcie

Okrem online funkcií uvedených vyššie existujú aj voliteľné online funkcie, ku ktorým môžete používateľom povoliť prístup prostredníctvom ich konta organizácie, ktoré sa niekedy označuje ako pracovné alebo školské konto. Napríklad funkcie LinkedInu v asistentovi životopisu vo Worde alebo panel počasia v Outlooku, ktorý využíva službu MSN Počasie. Ďalšie príklady nájdete v téme [Prehľad voliteľných online funkcií v balíku Office](optional-connected-experiences.md).

|Kategória|Podrobnosti|
|:-----|:-----|
|**Doména predvolieb**  | `com.microsoft.office` |
|**Kód**  | `OptionalConnectedExperiencesPreference`  |
|**Typ údajov**  | Boolovská hodnota |
|**Možné hodnoty**  | `TRUE` *(povolené)* <br/> `FALSE` *(zakázané)*|
|**Dostupnosť** |Verzia 16.28 a novšie verzie |

Ak túto predvoľbu nenastavíte, voliteľné online funkcie sú používateľom k dispozícii v prípade, že sa používatelia s predplatným na Office 365 (alebo Microsoft 365) prihlásili pomocou pracovného alebo školského konta, alebo ak používatelia majú multilicenčnú verziu balíka Office 2019 pre Mac. Ako ste túto predvoľbu nenastavili na hodnotu `FALSE`, títo používatelia majú možnosť voliteľné online funkcie vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.

Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), nemajú možnosť vypnúť voliteľné online funkcie.

## <a name="preference-setting-for-most-connected-experiences"></a>Nastavenia predvolieb pre väčšinu online funkcií

Pomocou tejto možnosti môžete určiť, či budú mať vaši používatelia k dispozícii väčšinu online funkcií.

|Kategória|Podrobnosti|
|:-----|:-----|
|**Doména predvolieb**  | `com.microsoft.office` |
|**Kód**  | `ConnectedOfficeExperiencesPreference`  |
|**Typ údajov**  | Boolovská hodnota |
|**Možné hodnoty**  | `TRUE` *(povolené)* <br/> `FALSE` *(zakázané)*|
|**Dostupnosť** |Verzia 16.28 a novšie verzie |

Ak túto predvoľbu nenastavíte, vaši používatelia majú k dispozícii všetky online funkcie, pokiaľ ste nenastavili niektorú z ďalších predvolieb pre online funkcie, ktoré sú spomenuté vyššie, ako napríklad predvoľbu `OfficeExperiencesAnalyzingContentPreference`.

Ak napríklad túto predvoľbu nastavíte na hodnotu `FALSE`, tieto typy online funkcií nebudú vašim používateľom k dispozícii:
- Funkcie na analýzu obsahu
- Funkcie na sťahovanie online obsahu
- Voliteľné pripojené funkcie

Okrem toho platí, že ak túto predvoľbu nastavíte na hodnou `FALSE`, vypne sa aj väčšina ostatných online funkcií, ako sú napríklad spolutvorba dokumentov a online ukladací priestor súborov. Zoznam týchto ostatných online funkcií nájdete v téme [Online funkcie v Office](connected-experiences.md).

Aj keď túto predvoľbu nastavíte na hodnotu `FALSE`, niektoré funkcie balíka Office zostanú dostupné, napríklad synchronizácia poštovej schránky v Outlooku, a aplikácie Teams a Skype for Business budú aj naďalej fungovať. [Nevyhnutné služby](essential-services.md), ako je napríklad licenčná služba, ktorá potvrdzuje, že máte správnu licenciu na používanie služieb Office, takisto zostanú k dispozícii.

Ak používatelia majú predplatné na Office 365 (alebo Microsoft 365) a sú prihlásení s pracovným alebo školským kontom, alebo ak majú multilicenčnú verziu balíka Office 2019 pre Mac, nemôžu väčšinu online funkcií vypnúť.

Ostatní používatelia, ako sú napríklad používatelia v domácnosti s predplatným na Office 365 (alebo Microsoft 365), majú možnosť väčšinu online funkcií vypnúť v okne **Predvoľby** > **Ochrana osobných údajov**.

## <a name="preference-setting-for-the-required-data-notice-dialog-for-microsoft-autoupdate"></a>Nastavenie predvolieb pre dialógové okno Oznámenie o požadovaných údajoch pre službu Microsoft AutoUpdate

Pri prvom spustení verzie 4.12 alebo novšej verzie služby Microsoft AutoUpdate (MAU) sa používateľom zobrazí dialógové okno **Oznámenie o požadovaných údajoch** s informáciami o tom, aké údaje služby MAU sa odosielajú spoločnosti Microsoft.

Ak nechcete, aby sa používateľom dialógové okno **Oznámenie o požadovaných údajoch** pre službu Microsoft AutoUpdate zobrazilo, môžete nastaviť nasledujúcu predvoľbu. Dialógové okno sa používateľom nezobrazí bez ohľadu na to, ktorú hodnotu nastavíte.

|Kategória|Podrobnosti|
|:-----|:-----|
|**Doména predvolieb**  | `com.microsoft.autoupdate2` |
|**Kód**  | `AcknowledgedDataCollectionPolicy`  |
|**Typ údajov**  | Reťazec |
|**Možné hodnoty**  | `RequiredDataOnly` <br/> `RequiredAndOptionalData`|
|**Dostupnosť** |Verzia 4.12 a novšie verzie |

Ak umožníte, aby sa toto dialógové okno používateľom zobrazilo, používatelia môžu kliknutím na tlačidlo **OK** zapísať do politiky `AcknowledgedDataCollectionPolicy` hodnotu `RequiredDataOnly` a tým nastaviť, aby sa im dialógové okno nezobrazovalo znova.


## <a name="related-articles"></a>Súvisiace články

- [Informácie o konfiguračnom profile (dokumentácia pre vývojárov Apple)](https://go.microsoft.com/fwlink/p/?linkid=852998)
- [Nasadenie predvolieb pre Office pre Mac](../mac/deploy-preferences-for-office-for-mac.md)
- [Nastavenia ochrany osobných údajov konta](https://support.office.com/article/3e7bc183-bf52-4fd0-8e6b-78978f7f121b#ID0EAADAAA=Mac)
