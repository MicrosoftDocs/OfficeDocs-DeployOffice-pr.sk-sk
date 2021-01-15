---
title: Povinné diagnostické údaje pre Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
audience: ITPro
ms.topic: reference
ms.service: o365-proplus-itpro
localization_priority: Priority
ms.collection: Ent_O365
ms.custom:
- Ent_Office_ProPlus
- Ent_Office_Privacy
description: Správcom balíka Office sú poskytované informácie o požadovaných diagnostických údajoch v Office a zoznam udalostí a údajových polí.
hideEdit: true
ms.openlocfilehash: b7993abbca401d65cc99ed9fdd7960bae03e89a3
ms.sourcegitcommit: c891622923aecf9afd3ba61e008501cb0c374b73
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/13/2021
ms.locfileid: "49841731"
---
# <a name="required-diagnostic-data-for-office"></a>Povinné diagnostické údaje pre Office

> [!NOTE]
> Ak si chcete pozrieť zoznam produktov balíka Office, na ktorý sa vzťahujú tieto informácie o ochrane osobných údajov, pozrite si tému [Ovládacie prvky na ochranu osobných údajov dostupné pre produkty balíka Office](products-versions-privacy-controls.md).

Diagnostické údaje sa používajú na zabezpečenie a aktualizovanie balíka Office, zisťovanie, diagnostiku a riešenie problémov, ako aj na vylepšenia produktov. Tieto údaje neobsahujú meno ani e-mailovú adresu používateľa, obsah súborov používateľa ani informácie o aplikáciách, ktoré nesúvisia s balíkom Office.

Tieto diagnostické údaje sa zhromažďujú a odosielajú spoločnosti Microsoft o klientskom softvéri balíka Office, ktorý sa používa v zariadení používateľa. Niektoré diagnostické údaje sú povinné, a iné diagnostické údaje sú voliteľné. Máte možnosť si vybrať, či nám budete odosielať povinné alebo voliteľné diagnostické údaje, pomocou ovládacích prvkov ochrany osobných údajov, ako sú nastavenia politiky pre organizácie. Nám odoslané diagnostické údaje môžete zobraziť pomocou Zobrazovača diagnostických údajov.

***Povinné diagnostické údaje** _ sú minimom potrebným na očakávané zabezpečenie balíka Office, jeho aktualizáciu a výkonnosť v zariadení, v ktorom je nainštalovaný.

Povinné diagnostické údaje pomáhajú identifikovať problémy s balíkom Office, ktoré môžu súvisieť s konfiguráciou zariadenia alebo softvéru. Pomáhajú napríklad určiť, či funkcia balíka Office zlyháva častejšie pri konkrétnej verzii operačného systému, či ide o novo zavedené funkcie alebo či sa to stáva, ak sú niektoré funkcie balíka Office vypnuté. Povinné diagnostické údaje pomáhajú zistiť, diagnostikovať a riešiť tieto problémy rýchlejšie, čím sa znižuje ich vplyv na používateľov alebo organizácie.

Ďalšie informácie o diagnostických údajoch sa nachádzajú v článkoch:

- [Voliteľné diagnostické údaje pre Office](optional-diagnostic-data.md)
- [Používanie nástroja Diagnostic Data Viewer s balíkom Office](https://support.microsoft.com/office/cf761ce9-d805-4c60-a339-4e07f3182855)

Ak ste správcom v organizácii, možno vás budú zaujímať aj nasledovné články:

- [Prehľad ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie](overview-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Aplikácie Microsoft 365 pre veľké organizácie](manage-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb](ios-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre zariadenia s Androidom s nastaveniami politiky](android-privacy-controls.md)

## <a name="categories-data-subtypes-events-and-data-fields-for-required-diagnostic-data"></a>Kategórie, podtypy údajov, udalosti a údajové polia povinných diagnostických údajov

Povinné diagnostické údaje sú usporiadané do kategórií a podtypov údajov. Každý podtyp údajov obsahuje udalosti, ktoré obsahujú údajové polia, ktoré sú špecifické pre danú udalosť.

Nasledujúca tabuľka obsahuje zoznam kategórií povinných diagnostických údajov. Podtypy údajov v každej kategórii sú uvedené aj s popisom zamerania daného podtypu údajov. Sú tu prepojenia na každú sekciu podtypu údajov, kde nájdete tieto informácie:

- Zoznam udalostí v danom podtype údajov
- Popis každej udalosti
- Zoznam údajových polí v každej udalosti
- Popis každého údajového poľa

| _ *Kategória**       | **Podtyp údajov**| **Popis**    |
| ---------- | ------------- | ---- |
| **Inštalácia softvéru a inventár** | [Inštalácia balíka Office a inventár](#office-setup-and-inventory-subtype)   | Nainštalovaný produkt a verzia a stav inštalácie.  |
| | [Konfigurácia doplnkov balíka Office](#office-add-in-configuration-subtype)  | Softvérové doplnky a ich nastavenia     |
| | [Zabezpečenie](#security-subtype)  | Chybové stavy dokumentu, funkcie a doplnku, ktoré môže ohroziť zabezpečenie, vrátane pripravenosti na aktualizáciu produktu.  |
| **Používanie produktov a služieb**    | [Úspešnosť funkcie aplikácie](#application-feature-success-subtype)   | Úspešnosť fungovania aplikácie. Obmedzené na otvorenie a zatvorenie aplikácie a dokumentov, úpravu súborov a zdieľanie súborov (spoluprácu). |
| | [Stav a spustenie aplikácie](#application-status-and-boot-subtype)    | Určenie, či sa vyskytli konkrétne udalosti funkcie, napríklad spustenie alebo ukončenie a či je funkcia spustená.   |
| | [Konfigurácia zjednodušenia ovládania balíka Office](#office-accessibility-configuration-subtype)  | Funkcie zjednodušenia ovládania balíka Office       |
| | [Ochrana osobných údajov](#privacy-subtype)| Nastavenia ochrany osobných údajov v Office|
| **Výkon produktov a služieb**       | [Neočakávané ukončenie (zlyhanie) aplikácie](#unexpected-application-exit-crash-subtype)  | Neočakávané ukončenia aplikácie a stav aplikácie, keď sa to stane.    |
|  | [Výkon funkcie aplikácie](#application-feature-performance-subtype)  | Dlhý čas odozvy alebo nízky výkon v prípadoch ako spustenie aplikácie alebo otvorenie súboru. |
|  | [Chyba aktivity aplikácie](#application-activity-error-subtype)   | Chyby funkčnosti funkcie alebo používateľského rozhrania.  |
| **Pripojiteľnosť a konfigurácia zariadenia** | [Pripojiteľnosť a konfigurácia zariadenia](#device-connectivity-and-configuration-subtype) | Stav sieťového pripojenia a nastavenia zariadenia, napríklad pamäte. |


> [!NOTE]
> - Zobrazovač diagnostických údajov zobrazuje kategórie, ale nezobrazuje podtypy údajov.
> - Údajové pole označené ako *zastarané* je alebo čoskoro bude odstránené z povinných diagnostických údajov. Niektoré z týchto údajových polí sú duplicitné položky, ktoré vznikli pri modernizácii diagnostických údajov a používali sa na zabezpečenie toho, aby nedošlo k žiadnemu prerušeniu služby pri zostavách živého diagnostického monitorovania.

## <a name="categories-and-data-fields-that-are-common-for-all-events"></a>Kategórie a údajové polia, ktoré sú spoločné pre všetky udalosti

Existuje niekoľko informácií o udalostiach, ktoré sú spoločné pre všetky udalosti bez ohľadu na kategóriu alebo podtyp údajov. Tieto spoločné informácie, ktoré sa niekedy označujú ako *údajové zmluvy*, sú usporiadané do kategórií. Každá kategória obsahuje polia. Tieto polia sú metaúdaje a vlastnosti jednotlivých udalostí. Tieto informácie môžete zobraziť pomocou Zobrazovača diagnostických údajov.

Kategórie informácií, ktoré sa o udalostiach zhromažďujú, možno rozdeliť do dvoch skupín:

  - [Informácie spoločné pre všetky udalosti](#information-common-to-all-events)
  - [Informácie, ktoré konkrétne podporujú zber diagnostických údajov](#information-that-specifically-supports-diagnostic-data-collection)

### <a name="information-common-to-all-events"></a>*Informácie spoločné pre všetky udalosti*

Informácie, ktoré sú spoločné pre všetky udalosti, sa zhromažďujú v nasledujúcich kategóriách.

#### <a name="app"></a>Aplikácia 

Informácie o aplikácii. Všetky polia sú konštantné pre všetky relácie danej verzie aplikácie.

Táto kategória obsahuje tieto polia:

  - **Branch** – vetva, z ktorej pochádza daná zostava. Umožňuje určiť, z akého typu vetvy daná zostava pochádza, aby sme mohli správne zacieliť opravy.
  - **InstallType** – enumerátor, ktorý identifikuje spôsob, akým používateľ nainštaloval aplikácie. Umožňuje určiť, či konkrétne inštalačné mechanizmy vytvárajú problémy, ktoré nie sa nezobrazia v iných inštalačných mechanizmoch.
  - **Name** – názov aplikácie, ktorá poskytuje údaje. Umožňuje identifikovať, ktorá aplikácia zobrazuje chybu, aby sme vedeli, ako problém riešiť.
  - **Platform** – široká klasifikácia platformy, na ktorej je aplikácia spustená. Umožňuje identifikovať, na ktorých platformách sa môže vyskytnúť chyba, aby sme správne určili prioritu problému.
  - **Version** – verzia aplikácie. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby správne určili jeho prioritu.

#### <a name="client"></a>Klient 

Identifikátor týkajúci sa inštancie balíka Office v zariadení. Konštanta pre všetky relácie všetkých aplikácií danej verzie inštalácie pre balíky viacerých aplikácií alebo konštantu pre všetky relácie danej verzie aplikácie.

Táto kategória obsahuje tieto polia:

  - **Id** – jedinečný identifikátor priradený klientovi v čase inštalácie balíka Office. Umožňuje identifikovať, či problémy majú vplyv na konkrétnu množinu inštalácií a koľko používateľov je ovplyvnených.

#### <a name="consent"></a>Súhlas

Informácie o súhlase používateľov týkajúcom sa diagnostických údajov a online funkcií.

Táto kategória obsahuje tieto polia:

  - **ControllerConnectedServicesSourceLocation** – označuje, ako používateľ uskutočnil výber voliteľných online funkcií.

  - **ControllerConnectedServicesState** – označuje, či má používateľ prístup k voliteľným online funkciám.

  - **ControllerConnectedServicesStateConsentTime** – označuje, kedy používateľ zvolil stav voliteľných online funkcií. Dátum sa zobrazí buď ako dátum čitateľný človekom, alebo ako strojovo kódovaný dátum, ktorý vyzerá ako veľké číslo.

  - **DiagnosticConsentConsentTime** – označuje, kedy používateľ poskytol súhlas s diagnostickými údajmi. Dátum sa zobrazí buď ako dátum čitateľný človekom, alebo ako strojovo kódovaný dátum, ktorý vyzerá ako veľké číslo.

  - **DiagnosticConsentLevel** – označuje úroveň súhlasu ohľadom diagnostických údajov, ktorý používateľ udelil.

  - **DiagnosticConsentLevelSourceLocation** – označuje, ako používateľ poskytol súhlas s diagnostickými údajmi.

  - **DownloadContentSourceLocation** – označuje, ako používateľ uskutočnil rozhodnutie zapnúť alebo vypnúť online funkcie, ktoré sťahujú online obsah.

  - **DownloadContentState** – označuje, či sa používateľ rozhodol zapnúť alebo vypnúť online funkcie, ktoré sťahujú online obsah.

  - **DownloadContentStateConsentTime** – označuje, kedy používateľ uskutočnil rozhodnutie zapnúť alebo vypnúť online funkcie, ktoré sťahujú online obsah. Dátum sa zobrazí buď ako dátum čitateľný človekom, alebo ako strojovo kódovaný dátum, ktorý vyzerá ako veľké číslo.

  - **ServiceConnectionState** – označuje, či sa používateľ rozhodol použiť alebo nepoužiť všetky online funkcie.

  - **ServiceConnectionStateConsentTime** – označuje, kedy sa používateľ rozhodol, či použiť všetky online funkcie. Dátum sa zobrazí buď ako dátum čitateľný človekom, alebo ako strojovo kódovaný dátum, ktorý vyzerá ako veľké číslo.

  - **ServiceConnectionStateSourceLocation** – označuje, ako sa používateľ rozhodol, či použiť všetky online funkcie.

  - **UserCategoryValue** – identifikuje typ používateľa, od ktorého pochádza súhlas. Môže to byť MSAUser, AADUser alebo LocalDeviceUser.

  - **UserContentDependentSourceLocation** – označuje, ako používateľ uskutočnil rozhodnutie zapnúť alebo vypnúť online funkcie, ktoré analyzujú obsah.

  - **UserContentDependentState** – označuje, či sa používateľ rozhodol zapnúť alebo vypnúť online funkcie na analýzu obsahu.

  - **UserContentDependentStateConsentTime** – označuje, kedy sa používateľ rozhodol zapnúť alebo vypnúť online funkcie, ktoré analyzujú obsah. Dátum sa zobrazí buď ako dátum čitateľný človekom, alebo ako strojovo kódovaný dátum, ktorý vyzerá ako veľké číslo.

#### <a name="device"></a>Zariadenie 

Informácie o operačnom systéme a zostave.

Táto kategória obsahuje tieto polia:

  - **OsBuild** – číslo zostavy operačného systému v zariadení. Umožňuje určiť, či problémy majú na jednotlivé balíky Service Pack alebo verzie daného operačného systému iný vplyv ako na ostatné, aby sme mohli určiť prioritu problémov.

  - **OsVersion** – hlavná verzia operačného systému nainštalovaného v zariadení. Umožňuje určiť, či problémy majú na konkrétnu verziu operačného systému väčší vplyv ako na ostatné, aby sme mohli určiť prioritu problémov.

#### <a name="legacy"></a>Staršia verzia 

Poskytuje ID aplikácie a verziu operačného systému z dôvodu kompatibility s existujúcimi staršími postupmi zhromažďovania údajov.

Táto kategória obsahuje tieto polia:

  - **AppId** – hodnota enumerátora predstavujúca aplikáciu, ktorá odosiela údaje. Umožňuje identifikovať, ktorá aplikácia zobrazuje chybu, aby sme vedeli, ako problém riešiť.

  - **OsEnv** – enumerátor označujúci operačný systém, v ktorom je relácia spustená. Umožňuje identifikovať, v ktorom operačnom systéme sa problém vyskytuje, aby sme mohli určiť prioritu problémov.

#### <a name="release"></a>Vydanie 

Informácie týkajúce sa kanála vydania. Všetky polia sú konštantné pre všetky relácie všetkých aplikácií danej verzie inštalácie. Určuje skupinu zariadení v jednej fáze cyklu vydania produktu.

Táto kategória obsahuje tieto polia:

  - **Audience** – identifikuje cieľovú podskupinu danej cieľovej skupiny. Umožňuje vysledovať podmnožiny cieľových skupín na vyhodnotenie výskytu a priority problémov.

  - **AudienceGroup** – identifikuje okruh, odkiaľ údaje pochádzajú. Umožňuje distribuovať funkcie vo fázach a identifikovať potenciálne problémy skôr, než sa dostanú k väčšine používateľov.

  - **Channel** – kanál, prostredníctvom ktorého sa produkt vydáva. Umožňuje identifikovať, či má problém na niektorý z našich distribučných kanálov iný vplyv ako na ostatné.

  - **Fork**  – identifikuje rozvetvenie produktu. Umožňuje mechanizmu zhrnúť údaje v rámci množiny čísel zostáv na identifikáciu problémov týkajúcich sa daného vydania.

#### <a name="session"></a>Relácia 

Informácie o relácii procesu. Všetky polia sú konštantné pre túto reláciu.

Táto kategória obsahuje tieto polia:

  - **ABConfigs** – identifikuje množinu skupiny funkcií, ktoré sú spustené v danej relácii. Umožňuje identifikovať, ktoré jednotlivé skupiny funkcií sú spustené v relácii, aby sme mohli určiť, či skupina funkcií je zdrojom problému, ktoré má vplyv na používateľov.

  - **EcsETag** – indikátor systému testovania funkcií, ktorý predstavuje skupiny funkcií odoslané do zariadenia. Umožňuje identifikovať, ktoré skupiny funkcií majú nepriaznivý vplyv na danú reláciu.

  - **Flags** – príznaky sledovania bitovej masky vzťahujúce sa na celú reláciu, aktuálne s primárnym zameraním na možnosti vzoriek a diagnostických údajov. Umožňuje ovládať spôsob správania danej relácie vo vzťahu k diagnostickým údajom, ktoré relácia vytvára.

  - **HostAppName** – Identifikuje názov hostiteľskej aplikácie, ktorá spúšťa podaplikáciu. Aplikácie ako Office Mobile (Android) môžu spúšťať podaplikácie Word, Excel a PowerPoint. Pre takéto podaplikácie je hostiteľskou aplikáciou OfficeMobile

  - **HostSessionId** – Jedinečne identifikuje reláciu hostiteľskej aplikácie pre podaplikáciu

  - **Id** – jedinečne identifikuje danú reláciu údajov. Umožňuje identifikovať vplyv problémov vyhodnotením počtu ovplyvnených relácií a toho, či existujú spoločné prvky týchto relácií.

  - **ImpressionId** – identifikuje množinu skupiny funkcií, ktoré sú spustené v danej relácii. Umožňuje identifikovať, ktoré jednotlivé skupiny funkcií sú spustené v relácii, aby sme mohli určiť, či skupina funkcií je zdrojom problému, ktoré má vplyv na používateľov.

  - **MeasuresEnabled** – príznak, ktorý označuje, či sú údaje aktuálnych relácií vzorkované alebo nie. Umožňuje určiť, ako sa štatisticky vyhodnotia údaje, ktoré zhromažďujú z danej relácie.

  - **SamplingClientIdValue** – ID klienta na určenie, či je súčasťou vzorkovania. Umožňuje určiť, prečo jednotlivé relácie boli alebo neboli súčasťou vzorkovania.
  
 - **SubAppName** – pre aplikáciu Office Mobile toto pole predstavuje základnú aplikáciu, ktorá sa používa na otvorenie dokumentu. Ak napríklad otvárate wordový dokument v aplikácii Office, v tomto poli sa bude nachádzať hodnota „Word“.

 - **VirtualizationType** – typ virtualizácie, ak je Office spustený v niektorej z nich. Možné hodnoty sú: 
    - 0 = Žiadne
    - 1 = Windows Virtual Desktop
    - 2 = Windows Defender Application Guard
    - 3 = Windows Core OS

#### <a name="user"></a>Používateľ

Poskytuje informácie o nájomníkovi pre komerčné jednotky SKU softvéru.

Táto kategória obsahuje tieto polia:

  - **PrimaryIdentityHash** – pseudoidentifikátor, ktorý predstavuje aktuálneho používateľa.

  - **PrimaryIdentitySpace** – typ identity v pseudoidentifikátore PrimaryIdentityHash. Môže to byť MASCID, OrgIdCID alebo UserObjectId.

  - **TenantGroup** – typ nájomníka, ktorému patrí predplatné. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov.

  - **TenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

### <a name="information-that-specifically-supports-diagnostic-data-collection"></a>*Informácie, ktoré konkrétne podporujú zber diagnostických údajov*

Informácie, ktoré konkrétne podporujú zber diagnostických údajov, sa zbierajú v nasledujúcich kategóriách.

#### <a name="activity"></a>Aktivita

Informácie na pochopenie úspešnosti samotnej udalosti zberu údajov.

Táto kategória obsahuje tieto polia:

  - **AggMode** – určuje, ako má systém agregovať výsledky aktivity. Umožňuje obmedziť množstvo informácií nahratých zo zariadenia používateľa agregáciou výsledkov aktivity do jednej udalosti, ktorá sa odosiela pravidelne.

  - **Count** – označuje, koľkokrát sa aktivita vyskytla, ak počet pochádza z agregovanej udalosti. Umožňuje určiť, ako často bola aktivita úspešná alebo neúspešná na základe agregačného režimu aktivity.

  - **CV** – hodnota, ktorá identifikuje vzťah medzi aktivitami a podradenými aktivitami. Umožňuje znova vytvoriť vzťah medzi vnorenými aktivitami.

  - **Duration** – časový úsek, ktorý bol potrebný na vykonanie aktivity. Umožňuje nám identifikovať problémy s výkonom, ktoré majú negatívny vplyv na používateľa.

  - **Result.Code** – aplikáciou definovaný kód na identifikáciu daného výsledku. Umožňuje určiť konkrétnejšie podrobností o danom zlyhaní, ako je napríklad kód zlyhania, pomocou ktorého je možné klasifikovať a riešiť problémy.

  - **Result.Tag** – značka celého čísla, ktorá identifikuje miesto v kóde, kde bol výsledok vytvorený. Umožňuje jednoznačne určiť miesto v kóde, kde bol výsledok vytvorený, vďaka čomu je možné klasifikovať zlyhania.

  - **Result.Type** – typ kódu výsledku. Identifikuje, aký typ kódu výsledku bol odoslaný, aby bolo možné hodnotu správne interpretovať.

  - **Success** – príznak označujúci úspešnosť alebo zlyhanie aktivity. Umožňuje určiť, či akcie, ktoré používateľ v produktoch vykoná, sú úspešné alebo neúspešné. Umožňuje to identifikovať problémy, ktoré majú vplyv na používateľa.

#### <a name="application"></a>Aplikácia 

Informácie o inštalácii aplikácie, z ktorej sa zhromažďujú udalosti.

Táto kategória obsahuje tieto polia:

  - **Architecture** – architektúra aplikácie. Umožňuje klasifikovať chyby, ktoré môžu byť špecifické pre architektúru aplikácie.

  - **Click2RunPackageVersion** – číslo verzie balíka Klikni a spusti, z ktorého bola aplikácia nainštalovaná. Umožňuje identifikovať, ktorá verzia programu sa použila na inštaláciu balíka Office, aby sme mohli identifikovať problémy súvisiace s inštaláciou.

  - **DistributionChannel** – kanál, v ktorom bola aplikácia nasadená. Umožňuje rozdeliť prichádzajúce údaje, aby sme mohli určiť, či majú problémy vplyv na cieľové skupiny.

  - **InstallMethod** – označuje, či bola aktuálna zostava balíka Office inovovaná zo staršej zostavy, vrátená na staršiu zostavu alebo nanovo nainštalovaná.

  - **IsClickToRunInstall** – príznak, ktorý označuje, či išlo o inštaláciu Klikni a spusti. Umožňuje identifikovať problémy, ktoré môžu byť špecifické pre mechanizmus inštalácie Klikni a spusti.

  - **IsDebug** – príznak označujúci, či je zostava balíka Office zostavou ladenia. Umožňuje identifikovať, či problémy pochádzajú zo zostáv ladenia, ktoré sa môžu správať odlišne.

  - **IsInstalledOnExternalStorage** – príznak, ktorý označuje, či bol balík Office nainštalovaný v externom úložnom zariadení. Umožňuje určiť, či problémy možno vysledovať do externého umiestnenia ukladacieho priestoru.

  - **IsOEMInstalled** – príznak, ktorý označuje, či bol balík Office nainštalovaný výrobcom OEM. Umožňuje určiť, či bola aplikácia nainštalovaná výrobcom OEM, čo nám pomáha klasifikovať a identifikovať problémy.

  - **PreviousVersion** – verzia balíka Office, ktorý bol predtým nainštalovaný v počítači. Umožňuje vrátiť sa späť na predchádzajúcu verziu, ak je aktuálna verzia problematická.

  - **ProcessFileName** – názov súboru aplikácie. Umožňuje identifikovať názov spustiteľného súboru, ktorý generuje údaje, pretože viaceré rôzne názvy súborov procesov môžu byť uvádzané ako názov rovnakej aplikácie.

#### <a name="client"></a>Klient

Informácie o klientovi balíka Office.

Táto kategória obsahuje tieto polia:

  - **FirstRunTime** – čas prvého spustenia klienta. Umožňuje pochopiť, ako dlho má klient nainštalovaný balík Office.

#### <a name="device"></a>Zariadenie

Informácie o konfigurácii a možnostiach zariadenia.

Táto kategória obsahuje tieto polia:

  - **DigitizerInfo** – informácie o digitalizátore používanom zariadením. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **FormFactor** – identifikuje, aký je činiteľ tvaru zariadenia, ktoré odosiela informácie. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **FormFactorFamily** – identifikuje, aký je činiteľ tvaru zariadenia, ktoré odosiela informácie. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **HorizontalResolution** – vodorovné rozlíšenie obrazovky zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Id** – jedinečný identifikátor zariadenia. Umožňuje identifikovať rozšírenie problémov v množine zariadení.

  - **IsEDPPolicyEnabled** – príznak, ktorý označuje, či je v počítači zapnutá rozšírená ochrana údajov. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **IsTerminalServer** – príznak určujúci, či je počítač terminálový server. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Manufacturer** – výrobca zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Model** – model zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **MotherboardUUIDHash** – hodnota hash jedinečného identifikátora základnej dosky. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **Name** – názov zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.
  
  - **NetworkCost** – označuje náklady na sieť alebo typ siete, napríklad účtované podľa objemu údajov alebo účtované podľa objemu údajov nad limit.
  
  - **NetworkCountry** – kód krajiny odosielateľa, na základe neočistenej IP adresy klienta.

  - **NumProcPhysCores** – počet fyzických jadier v počítači. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **OsLocale** – miestne nastavenie operačného systému, ktorý je spustený. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ProcessorArchitecture** – architektúra procesora. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ProcessorCount** – počet procesorov v počítači. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ProcSpeedMHz** – rýchlosť procesora. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **RamMB** – množstvo pamäte v zariadení. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ScreenDepth** – umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **ScreenDPI** – hodnota DPI obrazovky. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **SusClientId** – ID služby Windows Update zariadenia, v ktorom je balík Office spustený.

  - **SystemVolumeFreeSpaceMB** – množstvo voľného miesta v systémovom zväzku. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **SystemVolumeSizeMB** – veľkosť systémového zväzku v počítači. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **VerticalResolution** – zvislé rozlíšenie obrazovky zariadenia. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **WindowErrorReportingMachineId** – jedinečný identifikátor počítača poskytnutý technológiou hlásenia chýb systému Windows. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

  - **WindowSqmMachineId** – jedinečný identifikátor počítača poskytnutý technológiou SQM systému Windows. Umožňuje klasifikovať údaje na základe kontingenčného ovládacieho prvku zariadenia.

#### <a name="event"></a>Udalosť 

Informácie špecifické pre udalosť vrátane jedinečného identifikátora v relácii.

Táto kategória obsahuje tieto polia:

  - **Contract** – zoznam všetkých zmlúv, ktoré udalosť implementuje. Umožňuje vyhodnotiť, aké údaje sú súčasťou jednotlivých udalostí, aby sme ich mohli efektívne spracovať.

  - **CV** – hodnota, ktorá umožňuje identifikovať udalosti, ktoré navzájom súvisia. Slúži na diagnostiku, ktorá umožňuje identifikovať vzory súvisiaceho správania alebo súvisiacich udalostí.

  - **Flags** – informácia používaná na zmenu spôsobu, akým daná udalosť odpovedá. Slúži na spravovanie toho, ako sa s danou udalosťou zaobchádza na účely nahratia údajov pre spoločnosť Microsoft.

  - **Id** – jedinečný identifikátor udalosti. Umožňuje jedinečnú identifikáciu prijatých udalostí.

  - **Level** – označuje typ udalosti.

  - **Name** – názov udalosti. Umožňuje nám identifikovať udalosť, ktorá bola odoslaná z klienta.

  - **Rule** – identifikátor pravidla, ktoré vygenerovalo údaje, ak boli vygenerované podľa pravidla. Umožňuje identifikovať zdroj údajov, aby sme mohli overiť a spravovať parametre daných udalostí.

  - **RuleId** – identifikátor pravidla, ktoré vygenerovalo údaje, ak boli vygenerované podľa pravidla. Umožňuje identifikovať zdroj údajov, aby sme mohli overiť a spravovať parametre daných udalostí.

  - **RuleInterfaces** – všetky rozhrania, ktoré sú implementované podľa konkrétneho pravidla. Umožňuje klasifikovať a importovať údaje na základe štruktúry, čo zjednodušuje spracovanie údajov.

  - **RuleVersion** – identifikátor pravidla, ktoré vygenerovalo údaje, ak boli vygenerované podľa pravidla. Umožňuje identifikovať zdroj údajov, aby sme mohli overiť a spravovať parametre daných udalostí.

  - **SampleRate** – označenie percentuálneho podielu používateľov, ktorí odosielajú tento údaj. Umožňuje to vykonať štatistickú analýzu údajov a pri veľmi bežných údajových bodoch nevyžaduje, aby ho odosielali všetci používatelia.

  - **SchemaVersion** – verzia schémy použitá na generovanie diagnostických údajov. Vyžaduje sa na spravovanie údajov odoslaných z klienta. Umožňuje to neskôr zmeniť, aké údaje sú odosielané z každého klienta.

  - **Sequence** – počítadlo, ktoré označuje poradie, v akom bola udalosť vytvorená na strane klienta. Umožňuje zoradiť prijaté údaje, aby sme mohli identifikovať, aké kroky mohli viesť k problému, ktorý má vplyv na klientov.

  - **Source** – zdrojový kanál, ktorý sa použil na nahratie údajov. Vyžaduje sa na monitorovanie všetkých našich kanálov nahrávania a ich celkového stavu a pomáha identifikovať problémy s kanálom nahrávania. Umožňuje monitorovať jednotlivé kanály nahrávania, aby sa zaistila ich kompatibilita.

  - **Time** – čas vygenerovania udalosti na strane klienta. Umožňuje synchronizovať a overiť poradie udalostí vygenerovaných na strane klienta a vytvoriť metriky výkonu pre používateľské pokyny. 

#### <a name="host"></a>Hostiteľ

Informácie o aplikácii, ktorá hosťuje vstavanú aplikáciu.

Táto kategória obsahuje tieto polia:

  - **Id** – jedinečný identifikátor priradený hostiteľskej aplikácii vstavanou aplikáciou.

  - **SessionId** – globálne jedinečný identifikátor relácie hostiteľa.

  - **Version** – identifikátor verzie primárneho spustiteľného súboru hostiteľa.

#### <a name="legacy"></a>Staršia verzia

Informácie potrebné na kompatibilitu starších systémov.

Táto kategória obsahuje tieto polia:

  - **OsBuild** – špecifické číslo zostavy operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

  - **OsBuildRevision** – číslo revízie zostavy operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

  - **OsMinorVersion** – vedľajšia verzia operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

  - **OsVersionString** – zjednotený reťazec predstavujúci číslo zostavy operačného systému. Umožňuje zistiť, z ktorej verzie operačného systému diagnostické údaje pochádzajú, aby sa určila priorita problémov.

#### <a name="session"></a>Relácia

Informácie o relácii procesu.

Táto kategória obsahuje tieto polia:

  - **ABConfigsDelta** – sleduje rozdiel medzi aktuálnymi údajmi ABConfigs a predchádzajúcu hodnotu. Umožňuje sledovať, aké nové skupiny funkcií sú v počítači, čo pomáha určiť, či je za problém zodpovedná nová skupina funkcií.

  - **CollectibleClassification** – triedy informácií, ktoré môže relácia zhromaždiť. Umožňuje filtrovať relácie na základe údajov, ktoré obsahujú.

  - **DisableTelemetry** – príznak, ktorý označuje či je nastavený kľúč DisableTelemetry. Umožňuje zistiť, či relácia nehlásila diagnostické údaje iné ako EssentialServiceMetadata.

  - **SamplingClientIdValue** – hodnota kľúča použitého na určenie vzorkovania. Umožňuje určiť, prečo relácia bola alebo nebola vzorkovaná.

  - **SamplingDeviceIdValue** – hodnota kľúča použitého na určenie vzorkovania. Umožňuje určiť, prečo relácia bola alebo nebola vzorkovaná.

  - **SamplingKey** – kľúč používaný na určenie, či relácia je alebo nie je vzorkovaná. Umožňuje pochopiť, ako pri jednotlivých reláciách prebieha voľba toho, či budú alebo nebudú vzorkované.

  - **SamplingMethod** – metóda použitá na určenie politiky vzorkovania. Umožňuje pochopiť, aké údaje pochádzajú z relácie.

  - **SamplingSessionKValue** – rozšírené metaúdaje vzorkovania. Pomáhajú vyhodnotiť štatistický význam prijatých údajov.

  - **SamplingSessionNValue** – rozšírené metaúdaje vzorkovania. Pomáhajú vyhodnotiť štatistický význam prijatých údajov.

  - **Sequence** – jedinečný číselný identifikátor relácie. Umožňuje vytvoriť poradie relácií na analýzu problémov, ktoré sa mohli vyskytnúť.

  - **Start** – čas spustenia relácie procesu. Umožňuje stanoviť, kedy relácia začala.

  - **TelemetryPermissionLevel** – hodnota označujúca úroveň diagnostických údajov, s ktorými používateľ explicitne súhlasil. Umožňuje pochopiť, akú úroveň diagnostických údajov môžete od relácie očakávať.

  - **TimeZoneBiasInMinutes** -rozdiel v minútach medzi časom UTC a miestnym časom. Umožňuje normalizáciu času UTC späť na miestny čas.

## <a name="data-fields-that-are-common-for-onenote-events"></a>Údajové polia, ktoré sú spoločné pre udalosti OneNotu

Nasledujúce údajové polia sú spoločné pre všetky udalosti OneNotu v systémoch Mac, iOS a Android.

> [!NOTE]
> Pri používaní Zobrazovača diagnostických údajov zobrazujú udalosti OneNotu v systémoch Mac, iOS a Android názov Aktivita, Údaje zostavy alebo Neočakávané. Ak chcete nájsť skutočný názov udalosti, vyberte udalosť a potom sa pozrite na pole EventName.

- **Activity_ActivityType** – označuje typ tejto udalosti aktivity. Aktivita môže byť bežná aktivita alebo aktivita s vysokou hodnotou.

- **Activity_AggMode** – určuje, ako má systém agregovať výsledky aktivity. Umožňuje obmedziť množstvo informácií nahratých zo zariadenia používateľa agregáciou výsledkov aktivity do jednej udalosti, ktorá sa odosiela pravidelne.

- **Activity_Count** – označuje, koľkokrát sa aktivita vyskytla, ak počet pochádza z agregovanej udalosti. Umožňuje určiť, ako často bola aktivita úspešná alebo neúspešná na základe agregačného režimu aktivity.

- **Activity_CV** – hodnota, ktorá identifikuje vzťah medzi aktivitami a podradenými aktivitami. Umožňuje znova vytvoriť vzťah medzi vnorenými aktivitami.

- **Activity_DetachedDurationInMicroseconds** – čas, keď aktivita je nečinná a v skutočnosti nerobí nič, ale čas sa stále započítava do celkového času trvania aktivity.

- **Activity_DurationInMicroseconds** – časový úsek, ktorý bol potrebný na vykonanie aktivity. Umožňuje nám identifikovať problémy s výkonom, ktoré majú negatívny vplyv na používateľa.

- **Activity_Expiration** – dátum v číselnom formáte označuje, kedy sa táto udalosť prestane odosielať z klientov.

- **Activity_FailCount** – počet zlyhaní tejto aktivity

- **Activity_Name** – krátky názov udalosti. Umožňuje nám identifikovať udalosť, ktorá bola odoslaná z klienta.

- **Activity_Namespace** – priestor názvov udalosti. Umožňuje nám zoskupovať udalosť do skupín.

- **Activity_Reason** – reťazec označujúci dôvod skončenia aktivity s určitým výsledkom.

- **Activity_Result** – príznak označujúci úspešnosť, zlyhanie alebo neočakávané zlyhanie aktivity. Umožňuje určiť, či akcie, ktoré používateľ v produktoch vykoná, sú úspešné alebo neúspešné. Umožňuje to identifikovať problémy, ktoré majú vplyv na používateľa.

- **Activity_State** – príznak označujúci, či udalosť predstavuje začiatok aktivity používateľa alebo koniec aktivity používateľa.

- **Activity_SucceedCount** – počet úspešností tejto aktivity.

- **ErrorCode** – označuje kód chyby, ak je k dispozícii.

- **ErrorCode2** – označuje druhý kód chyby, ak je k dispozícii.

- **ErrorCode3** – označuje tretí kód chyby, ak je k dispozícii.

- **ErrorTag** – označuje značku priradenú v kóde chyby, ak je k dispozícii.

- **ErrorType** – označuje typ chyby, ak je k dispozícii.

- **EventName** – jedinečný názov udalosti OneNotu. Udalosti OneNotu používajú toto vlastné pole na zadanie jedinečného názvu z dôvodu technického obmedzenia v minulosti.

- **ExpFeatures** – označuje, či má používateľ v aplikácii OneNote zapnutý prepínač experimentálnych funkcií alebo nie.

- **ExpirationDate** – dátum v číselnom formáte označuje, kedy sa táto udalosť prestane odosielať z klientov.

- **IsConsumer** – označuje, či ide o používateľa v programe Consumer alebo nie.

- **IsEdu** – označuje, či ide o používateľa v nájomníkovi programu Education alebo nie.

- **IsIW** – označuje, či ide o používateľa v programe Enterprise alebo nie.

- **IsMsftInternal** – označuje, či je používateľ zamestnancom spoločnosti Microsoft alebo nie.

- **IsPremiumUser** – označuje, či má používateľ prémiovú licenciu alebo nie.

- **Namespace** – priestor názvov udalosti. Umožňuje nám zoskupovať udalosť do skupín.

- **Release_AppStore** – príznak označujúci, či zostava pochádza z obchodu s aplikáciami alebo nie.

- **Release_Audience** – identifikuje cieľovú podskupinu danej cieľovej skupiny. Umožňuje vysledovať podmnožiny cieľových skupín na vyhodnotenie výskytu a priority problémov.

- **Release_AudienceGroup** – identifikuje okruh, odkiaľ údaje pochádzajú. Umožňuje distribuovať funkcie vo fázach a identifikovať potenciálne problémy skôr, než sa dostanú k väčšine používateľov.

- **Release_Channel** – kanál, prostredníctvom ktorého sa produkt vydáva. Umožňuje identifikovať, či má problém na niektorý z našich distribučných kanálov iný vplyv ako na ostatné.

- **RunningMode** – označuje spôsob spustenia aplikácie používateľom alebo procesom systému.

- **SchemaVersion** – označuje aktuálnu verziu schémy telemetrie v kanáli telemetrie vo OneNote.

- **Session_EcsETag** – indikátor systému testovania funkcií, ktorý predstavuje skupiny funkcií odoslané do zariadenia. Umožňuje identifikovať, ktoré skupiny funkcií majú nepriaznivý vplyv na danú reláciu.

- **Session_ImpressionId** – identifikuje množinu skupiny funkcií, ktoré sú spustené v danej relácii. Umožňuje identifikovať, ktoré jednotlivé skupiny funkcií sú spustené v relácii, aby sme mohli určiť, či skupina funkcií je zdrojom problému, ktoré má vplyv na používateľov.

- **SessionCorrelationId** – globálne jedinečný identifikátor relácie hostiteľa.

- **SH_ErrorCode** – označuje kód chyby, ak je k dispozícii, keď aktivita zlyhá.

- **Tag** – značka celého čísla, ktorá identifikuje miesto v kóde, kde bola udalosť telemetrie vytvorená.

- **UserInfo_IdType** – reťazec označujúci typ konta používateľa.

- **UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **UserInfo_OtherId** – zoznam neprimárnych pseudonymných identifikátorov, ktoré predstavujú kontá používateľa.

- **UserInfo_OtherIdType** – zoznam neprimárnych typov kont.

## <a name="data-fields-that-are-common-for-outlook-mobile-events"></a>Údajové polia, ktoré sú spoločné pre udalosti služby Outlook Mobile

Outlook Mobile zhromažďuje spoločné polia pre každú z našich udalostí, aby sme mohli zabezpečiť aktualizovanie, zabezpečenie a funkčnosť aplikácie podľa očakávaní. 

Nasledujúce údajové polia sú spoločné pre všetky udalosti Outlooku pre iOS a Android.

- **aad_tenant_id** – ID nájomníka zákazníka, ak je k dispozícii

- **account_cid** – pseudoidentifikátor, ktorý predstavuje aktuálneho používateľa

- **account_domain** – názov domény konta

- **account_puid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft

- **account_type** – sleduje typ konta, napríklad Office 365, Google Cloud Cache, Outlook.com atď.

- **action** – názov akcie udalosti (napríklad archivovanie, odstránenie atď.), aby sme mohli zistiť problémy vykonaním konkrétnych akcií

- **ad_id** – jedinečný identifikátor reklamy

- **app_version** – aktuálna verzia nainštalovanej aplikácie, pomocou ktorej zistíme problémy ovplyvňujúce určitú verziu aplikácie

- **AppInfo.ETag** – jedinečný identifikátor na spravovanie vydaní našich funkcií, ktorý pomáha zisťovať problémy ovplyvňujúce určité funkcie, ktoré vydávame

- **AppInfo.Language** – aktuálne nastavenie jazyka zariadenia, ktoré pomáha pri zisťovaní problémov ovplyvňujúcich určité jazyky

- **AppInfo.Version** – aktuálna verzia nainštalovanej aplikácie, pomocou ktorej zistíme problémy ovplyvňujúce určité verzie aplikácie

- **ci** – jedinečný pseudoidentifikátor zariadenia špecifického pre konkrétnu aplikáciu

- **cid_type** – označuje typ konta, ako je napríklad obchodné konto alebo konto Outlook.com.

- **cloud** – označuje miesto, kde sa nachádza poštová schránka konta v tomto zariadení, a pomáha zisťovať konkrétne problémy poštovej schránky v konkrétnom cloude, ako je napríklad Office 365 alebo GCC.

- **customer_type** – označuje typ zákazníka (spotrebiteľský, komerčný, tretia strana atď.), aby sme mohli zistiť problémy ovplyvňujúce určité typy zákazníkov

- **device_category** – označuje, o aký typ zariadenia ide (telefón, tablet atď.), aby sme mohli zistiť špecifické problémy podľa kategórie zariadenia

- **DeviceInfo.Id** – jedinečný identifikátor zariadenia, ktorý nám pomáha zisťovať problémy s konkrétnym zariadením

- **DeviceInfo.Make** – označuje značku zariadenia (napr. Apple, Samsung atď.) a pomáha zisťovať problémy s konkrétnou značkou zariadenia

- **DeviceInfo.Model** – označuje model zariadenia (napr. iPhone 6s) a pomáha zisťovať problémy s konkrétnym modelom zariadenia

- **DeviceInfo.NetworkType** – označuje aktuálne používanú sieť zariadenia (WiFi, mobilná atď.) a pomáha zisťovať problémy s konkrétnou sieťou zariadenia

- **DeviceInfo.OsBuild** – označuje aktuálnu zostavu operačného systému zariadenia a pomáha zisťovať problémy ovplyvňujúce určité zostavy operačného systému

- **DeviceInfo.OsName** – označuje názov operačného systému (napríklad iOS) a pomáha zisťovať problémy ovplyvňujúce určité platformy

- **DeviceInfo.OsVersion** – označuje aktuálnu verziu operačného systému zariadenia a pomáha zisťovať problémy ovplyvňujúce určité verzie operačného systému

- **DeviceInfo.SDKUid** – jedinečný identifikátor zariadenia (podobný ako DeviceInfo.Id)

- **EventInfo.InitId** – ID, ktoré sa používa ako súčasť postupnosti pre poradie udalosti prostredníctvom nášho kanála telemetrie a pomáha zistiť prvotnú príčinu problému s kanálom

- **EventInfo.SdkVersion** – verzia SDK, ktorú používame na odoslanie telemetrie a tisťovanie prvotnej príčiny problému s kanálom

- **EventInfo.Sequence** – postupnosť pre poradie udalosti prostredníctvom nášho kanála telemetrie, ktorá pomáha zistiť prvotnú príčinu problému s kanálom

- **EventInfo.Source** – oznamuje, aká časť kódu odoslala udalosť, a pomáha zistiť prvotnú príčinu problému

- **EventInfo.Time** – čas a dátum, kedy sa udalosť emitovala zo zariadenia, aby naše systémy mohli úspešne spravovať prichádzajúce udalosti

- **eventpriority** – priorita udalosti telemetrie vzhľadom na iné udalosti, aby naše systémy mohli úspešne spravovať prichádzajúce udalosti

- **first_launch_date** – označuje čas prvého spustenia aplikácie a pomáha zisťovať čas prvého výskytu problému

- **hashed_email** – pseudoidentifikátor, ktorý predstavuje e-mail aktuálneho používateľa

- **is_first_session** – sleduje, či ide o prvú reláciu aplikácie na účely ladenia

- **origin** – pôvod akcie. Napríklad označenie správy ako prečítanej môže pochádzať zo zoznamu správ alebo z oznámenia o novom e-maile. Pomáha nám to zisťovať problémy na základe pôvodu akcie

- **PipelineInfo.AccountId** – pseudoidentifikátor, ktorý predstavuje aktuálneho používateľa

- **PipelineInfo.ClientCountry** – aktuálna krajina zariadenia na zisťovanie problémov a výpadkov v konkrétnych krajinách alebo oblastiach

- **PipelineInfo.ClientIp** – IP adresa pripojenia zariadenia na ladenie problémov s pripojením

- **PipelineInfo.IngestionTime** – časová pečiatka uskutočnenia príjmu telemetrie pre túto udalosť

- **Session.Id** – jedinečný identifikátor relácie aplikácie na pomoc pri identifikácii problémov súvisiacich s reláciou

- **Session.ImpressionId** – jedinečný identifikátor na spravovanie vydaní našich funkcií a zabezpečenie úspešného vydania funkcií pre všetkých používateľov a zariadenia.

- **ui_mode** – označuje, či je používateľ v svetlom alebo tmavom režime, a pomáha pri triedení chýb používateľskej skúsenosti v tmavom režime

- **UserInfo.Language** – označuje jazyk používateľa a pomáha pri ladení problémov s textom prekladu

- **UserInfo.TimeZone** – časové pásmo používateľa na pomoc pri ladení problémov s kalendárom


Okrem toho nasledujúce polia sú spoločné pre všetky udalosti Outlooku pre iOS.

- **DeviceInfo.NetworkProvider** – poskytovateľ siete zariadenia (napr. Verizon)

- **gcc_restrictions_enabled** – informuje o tom, či boli v aplikácii použité obmedzenia GCC, aby sme mohli zabezpečiť zákazníkom GCC bezpečné využívanie našej aplikácie
 
- **multi_window_mode** – uvádza, či používateľ s iPadom používa viacero okien, aby sme mohli zistiť problémy týkajúce sa používania viacerých okien.

- **office_session_id** – jedinečný identifikátor na sledovanie relácie pripojených služieb balíka Office, ktorý pomáha pri zisťovaní konkrétnych problémov s integráciou služieb balíka Office v Outlooku, ako je napríklad Word

- **state** – označuje, či aplikácia bola aktívna pri odoslaní tejto udalosti, a pomáha pri zisťovaní konkrétnych problémov s aktívnym alebo neaktívnym stavom aplikácie


Okrem toho nasledujúce polia sú spoločné pre všetky udalosti Outlooku pre Android.

- **aad_id** – pseudonymné identifikátor služby Azure Active Directory

- **DeviceInfo.NetworkCost** – označuje aktuálne sieťové náklady zariadenia, čo odráža stav WiFi/mobilnej siete/roamingu, a pomáha pri zisťovaní konkrétnych problémov so sieťou zariadenia

- **is_app_in_duo_split_view_mode** – oznamuje, že aplikácia bola v režime rozdelenej obrazovky Duo.  Táto vlastnosť je nastavená len pre zariadenia Duo (iba pre Android).

- **is_dex_mode_enabled** – označuje, či je režim Samsung DeX povolený, a pomáha pri zisťovaní konkrétnych problémov s režimom DeX v zariadeniach Samsung

- **is_sliding_drawer_enabled** – označuje, či je zapnuté rozhranie posuvnej ponuky, a pomáha zisťovať problémy spôsobené naším rozhraním posuvnej ponuky

- **orientation** – označuje fyzickú orientáciu obrazovky (na výšku alebo na šírku) a pomáha pri zisťovaní konkrétnych problémov s orientáciou zariadenia

- **os_arch** – architektúra operačného systému zariadenia na pomoc pri zisťovaní problémov s konkrétnymi operačnými systémami zariadení

- **process_bitness** – označuje bitovosť procesov (32 alebo 64 bitov) aplikácie a pomáha pri zisťovaní konkrétnych problémov s bitovosťou zariadenia

- **webview_kernel_version**: verzia jadra platformy Chromium webového zobrazenia v zariadení, aby sme mohli zistiť problémy s kompatibilitou týkajúce sa verzie webového zobrazenia.

- **webview_package_name**: názov balíka webového zobrazenia v zariadení, aby sme mohli zistiť problémy s kompatibilitou týkajúce sa verzie webového zobrazenia.

- **webview_package_version**: vewrzia balíka webového zobrazenia v zariadení, aby sme mohli zistiť problémy s kompatibilitou týkajúce sa verzie webového zobrazenia.


## <a name="software-setup-and-inventory-data-events"></a>Údajové udalosti v kategórii Inštalácia softvéru a inventár

Toto sú podtypy údajov v tejto kategórii:
- [Inštalácia balíka Office a inventár](#office-setup-and-inventory-subtype)
- [Konfigurácia doplnkov balíka Office](#office-add-in-configuration-subtype)
- [Zabezpečenie](#security-subtype)  

### <a name="office-setup-and-inventory-subtype"></a>*Podtyp Inštalácia balíka Office a inventár*

Nainštalovaný produkt a verzia a stav inštalácie.

#### <a name="addssoaccount"></a>add.sso.account

Týmto sa spoločnosť Microsoft upozorní na úspech alebo zlyhanie pridania konta prostredníctvom jediného prihlásenia (SSO).

Zhromažďujú sa tieto polia: 

- **account_type** – typ konta pridaného pomocou SSO.

- **action_origin** – uvádza, odkiaľ sa vygenerovala táto udalosť. (príklad hodnoty: sso_drawer, sso_add_account, sso_add_account_prompt, sso_settings, sso_oobe).

- **provider** – identifikátor softvérového balíka poskytovateľa pre jediné prihlásenie.

- **state** – aktuálny stav konta (príklad hodnoty: FAILED, PENDING, ADDED atď.)


#### <a name="installreferral"></a>install.referral

Táto udalosť sa spustí pri prvej inštalácii aplikácie a zaznamenáva, odkiaľ bol používateľ odkázaný (ak je to k dispozícii).

Zhromažďujú sa tieto polia:

- **install_referrer** – produkt alebo prostredie, odkiaľ bol používateľ odkázaný

 
#### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Platí pre všetky aplikácie win32. Pomáha pochopiť stav procesu aktualizácie balíka Office (úspešná alebo neúspešná s podrobnosťami chyby).

Zhromažďujú sa tieto polia:

- **build** – aktuálne nainštalovaná verzia balíka Office

- **channel** – kanál, cez ktorý bol distribuovaný balík Office

- **errorCode** – kód chyby s informáciou o zlyhaní

- **errorMessage** – ďalšie informácie o chybe

- **status** – aktuálny stav aktualizácie

- **targetBuild** – verzia, na ktorú sa balík Office aktualizuje

#### <a name="officecompliancefileformatballotdisplayedonfirstboot"></a>Office.Compliance.FileFormatBallotDisplayedOnFirstBoot

Označuje, či sa používateľovi zobrazilo dialógové okno výberu formátu súboru balíka Office pri prvom alebo druhom štarte Wordu, Excelu, PowerPointu vo Win32.  Sleduje, či sa zobrazí dialógové okno voľby formátu súboru – udalosť sa odošle pri prvom alebo druhom spustení Wordu, Excelu alebo PPT Win32.

Zhromažďujú sa tieto polia:

- **CountryRegion** – nastavenie oblasti krajiny používateľov v systéme Windows

- **FileFormatBallotBoxAppIDBootedOnce** – v ktorej aplikácii (Word, Excel, PPT) sa spracovala logika zobrazenia voľby formátu súboru.

- **FileFormatBallotBoxDisplayedOnFirstBoot** – aký je výsledok zobrazenia voľby formátu súboru (zobrazuje sa/nezobrazuje sa ako neočakávaný/nezobrazený z dôvodu licencie/nezobrazený z dôvodu polohy).

#### <a name="officecompliancefileformatballotoption"></a>Office.Compliance.FileFormatBallotOption

Sleduje, či sa zobrazí dialógové okno voľby formátu súboru – udalosť sa odošle pri prvom alebo druhom spustení Wordu, Excelu alebo PPT Win32.  Označuje, či sa zobrazuje dialógové okno výberu formátu súboru balíka Office pri prvom alebo druhom štarte Wordu, Excelu, PowerPointu vo Win32.

Zhromažďujú sa tieto polia:

- **FileFormatBallotSelectedOption** – identifikuje možnosť formátu súboru (OOXML/ODF), ktorú používateľ vybral prostredníctvom dialógového okna voľby formátu súboru.


#### <a name="officecorrelationmetadatautccorrelationmetadata"></a>Office.CorrelationMetadata.UTCCorrelationMetadata

Zhromažďuje metaúdaje balíka Office prostredníctvom UTC na porovnanie s ekvivalentnými údajmi zhromaždenými prostredníctvom kanála telemetrie balíka Office a kontrolu správnosti a úplnosti údajov.

Zhromažďujú sa tieto polia:

- **abConfigs** – zoznam ID funkcií na určenie, ktoré funkcie sú zapnuté v klientovi alebo prázdne, keď tieto údaje nie sú zhromažďované.

- **abFlights** – hodnota „NoNL:NoFlights“, keď skupiny funkcií nie sú nastavené. V opačnom prípade hodnota „holdoutinfo=unknown“.

- **AppSessionGuid** – identifikátor konkrétnej relácie aplikácie, ktorá začína v čase vytvorenia procesu a pretrváva až do konca procesu. Je formátovaný ako štandardný 128-bitový identifikátor GUID, ale skladá sa zo štyroch častí. Tieto štyri časti sú v poradí 1. ID procesu 32-bitovej verzie, 2. ID relácie 16-bitovej verzie, 3. ID spustenia 16-bitovej verzie, 4. čas vytvorenia procesu 64-bitovej verzie v UTC 100 ns.

- **appVersionBuild** – číslo verzie zostavy aplikácie.

- **appVersionMajor** – číslo hlavnej verzie aplikácie.

- **appVersionMinor** – číslo vedľajšej verzie aplikácie.

- **appVersionRevision** – číslo verzie revízie aplikácie.

- **audienceGroup** – názov cieľovej skupiny používateľov vydania

- **audienceId** – názov cieľovej skupiny vydania

- **channel** – kanál, cez ktorý bol distribuovaný balík Office

- **deviceClass** – činiteľ tvaru zariadenia z operačného systému

- **ecsETag** – identifikátor experimentu procesu

- **impressionId** – identifikátor GUID označujúci aktuálnu množinu funkcií.

- **languageTag** -aktuálna značka jazyka skupiny IETF používateľského rozhrania balíka Office

- **officeUserID** – náhodne vytvorený identifikátor GUID pre túto inštaláciu balíka Office

- **osArchitecture** – architektúra operačného systému

- **osEnvironment** – celé číslo označujúce operačný systém (Windows, Android, iOS, Mac atď.).

- **osVersionString** – verzia operačného systému

- **sessionID** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

- **UTCReplace_AppSessionGuid** – konštantná boolovská hodnota. Vždy hodnota True.

#### <a name="officeonenoteandroidapponenotelaunchednonactivated"></a>Office.OneNote.Android.App.OneNoteLaunchedNonActivated

*[Táto udalosť sa predtým nazývala OneNote.App.OneNoteLaunchedNonActivated.]*

Zaznamenávajú sa informácie o stave aktivácie aplikácie.  Údaje sa monitorujú s cieľom zabezpečiť, aby sme identifikovali výkyvy pri problémoch s aktiváciou. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie.

Zhromažďujú sa tieto polia: 

- **INSTALL_LOCATION** – označuje, či je aplikácia predinštalovaná alebo stiahnutá z obchodu

#### <a name="officeonenoteandroidresetstatus"></a>Office.OneNote.Android.ResetStatus

*[Táto udalosť sa predtým nazývala OneNote.ResetStatus.]*

Signál, ktorý sa používa na zaznamenanie všetkých problémov, ktoré sa vyskytli pri pokuse používateľa o resetovanie aplikácie.  Telemetria sa používa na sledovanie, zisťovanie a opravu všetkých problémov spôsobených počas resetovania. 

Zhromažďujú sa tieto polia: 

- **Kontá** – označuje typy kont používaných na prihlásenie do aplikácie

- **Typ generického reťazca** – vráti sa, ak ide úplné obnovenie v rámci obnovenia notes_light_data

- **LaunchPoint** – bod, v ktorom sa spúšťa resetovanie. Možné hodnoty: Tlačidlo Odhlásiť, Zlyhanie pri odhlásení, Spustené v službe Intune

- **Pass** – označuje, či bolo resetovanie úspešné

#### <a name="officeonenoteandroidsigninsignincompleted"></a>Office.OneNote.Android.SignIn.SignInCompleted

*[Táto udalosť sa predtým nazývala OneNote.SignIn.SignInCompleted.]*

Kritický signál, ktorý označuje, či ide o úspešné prihlásenie alebo nie. Telemetria sa zhromažďuje na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby.

Zhromažďujú sa tieto polia: 

- **CompletionState** – konečný stav prihlásenia – úspešný alebo neúspešný. A prípady zlyhania

- **EntryPoint** – označuje, kde sa prihlásenie začalo

- **Hresult** – kód chyby

- **ID balíka poskytovateľa** – v prípade automatického prihlásenia

- **Result** – Úspešné, Neúspešné, Neznáme, Zrušené

- **ServerType** – vráti typ servera, ktorý ponúka službu 

- **SignInMode** – prihlásenie alebo registrácia, alebo automatické prihlásenie alebo zrýchlená registrácia

#### <a name="officeonenoteandroidsigninsigninstarted"></a>Office.OneNote.Android.SignIn.SignInStarted

*[Táto udalosť sa predtým nazývala OneNote.SignIn.SignInStarted.]*

Signál, ktorý sa používa na označenie všetkých problémov, ktoré sa vyskytli počas používania panela hlásení.  Telemetria sa používa na sledovanie, zisťovanie a opravu všetkých problémov spôsobených počas používania panela hlásení.

Zhromažďujú sa tieto polia: 

- **EntryPoint** – označuje, kde sa prihlásenie začalo

- **Výsledok** – výsledok postupu prihlásenia

- **ServerType** – vráti typ servera, ktorý ponúka službu 

- **SignInMode** – prihlásenie alebo registrácia, alebo automatické prihlásenie alebo zrýchlená registrácia


#### <a name="officeonenotefirstrunfirstrun"></a>Office.OneNote.FirstRun.FirstRun

Kritický signál, ktorý sa používa na zaistenie, že noví používatelia môžu úspešne spustiť a používať OneNote po prvýkrát.  Telemetria sa zhromažďuje na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu spustiť aplikáciu po prvýkrát, môže to vyvolať incident s vysokou závažnosťou.

- **AfterOneDriveFrozenAccountError** – označuje chybu z OneDrivu, keď je konto zmrazené.

- **Attempt** – koľkokrát sa vyžaduje zopakovanie pokusu o prvé spustenie.

- **IsDefaultNotebookCreated** – označuje, či OneNote vytvoril predvolený poznámkový blok používateľa alebo nie.

- **IsDelayedSignIn** – označuje, či prvé spustenie je v režime odloženého prihlásenia, v ktorom sa nevyžaduje prihlásenie používateľa.

- **IsMSA** – označuje, či konto je kontom Microsoft alebo nie.

#### <a name="officeonenotefirstrunfirstrunformsa"></a>Office.OneNote.FirstRun.FirstRunForMSA

Kritický signál, ktorý sa používa na zaistenie, že noví individuálni používatelia (konto Microsoft) môžu úspešne spustiť a používať OneNote po prvýkrát.

Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu spustiť aplikáciu po prvýkrát, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **Attempt** – koľkokrát sa vyžaduje zopakovanie pokusu o prvé spustenie.

- **Error A** – objekt chyby OneNotu označuje chybu pri prvom spustení, ak sa vyskytla.

- **FAllowAddingGuide** – označuje, či OneNote umožní vytvoriť sprievodný poznámkový blok alebo nie.

- **FrozenOneDriveAccount** – označuje, či konto OneDrivu je zmrazené alebo nie.

- **IsDefaultNotebookCreated** – označuje, či OneNote vytvoril predvolený poznámkový blok používateľa alebo nie.

- **NoInternetConnection** – označuje, či zariadenie nemá internetové pripojenie.

- **ProvisioningFailure** – objekt chyby OneNotu označujúci chybu zriaďovania, ak sa vyskytla.

- **ProvisioningFinishedTime** – označuje čas ukončenia, kedy OneNote dokončí zriaďovanie poznámkového bloku pri prvom spustení.

- **ProvisioningStartedTime** – označuje čas začiatku, kedy OneNote začne zriaďovanie poznámkového bloku pri prvom spustení.

- **ShowSuggestedNotebooks** – označuje, či OneNote zobrazí funkciu navrhovaného poznámkového bloku alebo nie.

#### <a name="officeonenotefirstrunfirstrunfororgid"></a>Office.OneNote.FirstRun.FirstRunForOrgId

Kritický signál, ktorý sa používa na zaistenie, že noví podnikoví používatelia (AAD/ID organizácie) môžu úspešne spustiť a používať OneNote po prvýkrát.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu spustiť aplikáciu po prvýkrát, môže to vyvolať incident s vysokou závažnosťou.

- **Attempt** – koľkokrát sa vyžaduje zopakovanie pokusu o prvé spustenie.

- **Error** – objekt chyby OneNotu označuje chybu pri prvom spustení, ak sa vyskytla.

- **FAllowAddingGuide** – označuje, či OneNote umožní vytvoriť sprievodný poznámkový blok alebo nie.

- **IsDefaultNotebookCreated** – označuje, či OneNote vytvoril predvolený poznámkový blok používateľa alebo nie.

- **ProvisioningFailure** – objekt chyby OneNotu označuje chybu zriaďovania, ak sa vyskytla.

- **ProvisioningFinishedTime** – označuje čas ukončenia, kedy OneNote dokončí zriaďovanie poznámkového bloku pri prvom spustení.

- **ProvisioningStartedTime** – označuje čas začiatku, kedy OneNote začne zriaďovanie poznámkového bloku pri prvom spustení.

#### <a name="officeonenotefirstrunmrureadernotebookentries"></a>Office.OneNote.FirstRun.MruReaderNoteBookEntries 

Signál, ktorý sa používa na zaznamenanie všetkých problémov, ktoré sa vyskytli pri načítavaní poznámkových blokov počas prvého spustenia.  Telemetria sa používa na sledovanie, zisťovanie a opravu všetkých problémov pri prvom spustení.

Zhromažďujú sa tieto polia: 

- **OnPremNBCount** – počet poznámkových blokov na lokálnom serveri

- **TotalNBCount** – celkový počet poznámkových blokov priradených k používateľskému kontu

#### <a name="officetargetedmessagingensurecached"></a>Office.TargetedMessaging.EnsureCached 

Sleduje, či bol stiahnutý balík pre dynamické plátno. Berie do úvahy konfiguráciu softvéru, pretože balík musí byť úspešne stiahnutý, aby umožnil klientovi vykresliť správne prostredie. Veľmi dôležité najmä v rámci spotrebiteľských predplatných, kde pomocou plátna informujeme používateľa, že platnosť licencie uplynula. Slúži na sledovanie metaúdajov balíka dynamického obsahu, ktorý bol stiahnutý a uložený do vyrovnávacej pamäte produktom, a výsledkov operácií vykonaných s balíkom: zlyhania stiahnutia, zlyhania rozbalenia, zlyhania kontrol konzistentnosti, počet výskytov vo vyrovnávacej pamäti, využitia balíka, zdroje sťahovania.

Zhromažďujú sa tieto polia:

  - **Data\_CacheFolderNotCreated** – boolovský príznak, ktorý označuje, či bolo vytvorenie priečinka vyrovnávacej pamäte úspešné

  - **Data\_CdnPath – zdrojová adresa balíka**

  - **Data\_EnsureCached** – boolovský príznak, ktorý označuje, či bol balík obsahu uložený do vyrovnávacej pamäte

  - **Data\_ExistsAlready** boolovský príznak, ktorý označuje, že balík bol stiahnutý už predtým a bol vykonaný ďalší pokus

  - **Data\_GetFileStreamFailed** – zdrojový balík nie je k dispozícii v zdroji

  - **Data\_GetFileStreamFailedToCreateLocalFolder** – problémy s lokálnym diskom, ktoré spôsobujú zlyhanie vytvorenia adresára

  - **Data\_GetFileStreamFromPackageFailed** – príznak, ktorý označuje, ak bol balík stiahnutý, ale klient ho nedokáže prečítať

  - **Data\_GetFileStreamFromPackageSuccess** – úspešné pokusy čítania balíka

  - **Data\_GetFileStreamSuccess** – bez problémov s diskom či konfiguráciou, ktoré by nedovolili čítať prúd súborov

  - **Data\_GetRelativePathsFailed** – relatívna cesta nesmeruje na dostupné umiestnenie

  - **Data\_HashActualValue** – hodnota hash získaná z názvu súboru pri použití balíka

  - **Data\_HashCalculationFailed** – chyba výpočtu hodnoty hash

  - **Data\_HashMatchFailed** – nesúlad hodnoty hash medzi názvom balíka a hodnotami databázy Registry vo vyrovnávacej pamäti

  - **Data\_HashMatchSuccess** – úspešná kontrola konzistentnosti hodnoty hash

  - **Data\_PackageDownloadRequestFailed** – balík nie je možné stiahnuť

  - **Data\_PackageDownloadRequestNoData** – stiahnutý balík neobsahuje žiadne údaje

  - **Data\_PackageDownloadRequestSuccess** – úspešné stiahnutie balíka

  - **Data\_PackageExplodedSuccess** – stavy pokusov o rozbalenie

  - **Data\_PackageOpenFailed** – neúspešné pokusy otvorenia súboru balíka

  - **Data\_PackageOpenSuccess** – úspešné pokusy otvorenia súboru balíka

  - **Data\_SuccessHashValue** – hodnota hash získaná z názvu súboru pri stiahnutí balíka

  - **Data\_SuccessSource** – povrch, pre ktorý sa balík stiahol

#### <a name="officevisiovisiosku"></a>Office.Visio.VisioSKU

Zaznamenáva jednotky SKU Visia, či ide o Standard alebo Professional. Potrebné pri kategorizácii problémov podľa jednotiek SKU.

Zhromažďujú sa tieto polia:

  - **Data\_VisioSKU**:**integer** – 0 pre jednotky SKU Standard a 1 pre jednotky SKU Professional

### <a name="office-add-in-configuration-subtype"></a>*Podtyp Konfigurácia doplnkov balíka Office*

Softvérové doplnky a ich nastavenia

#### <a name="exceladdindefinedfunctioncustomfunctionsallinone"></a>Excel.AddinDefinedFunction.CustomFunctionsAllInOne

Zhromažďuje informácie o tom, ako sa v režime runtime správajú funkcie vlastných doplnkov. Udržiava počítadlá pokusov spustenia, úspešných dokončení, chýb infraštruktúry a chýb používateľských kódov. Táto možnosť sa používa na identifikovanie problémov so spoľahlivosťou v produkte a riešenie problémov, ktoré majú vplyv na používateľov.
 
Zhromažďujú sa tieto polia:

- **AsyncBegin** – počet asynchrónnych funkcií, ktoré začínajú

- **AsyncEndAddinError** – počet asynchrónnych funkcií, ktoré končia chybou

- **AsyncEndInfraFailure** – počet asynchrónnych funkcií, ktoré končia zlyhaním infraštruktúry

- **AsyncEndSuccess** – počet asynchrónnych funkcií, ktoré končia úspešne

- **AsyncRemoveCancel** – počet zrušených asynchrónnych funkcií 

- **AsyncRemoveRecycle** – počet asynchrónnych funkcií, ktoré boli odstránené z dôvodu recyklácie 

- **StreamingCycles1** – počítadlo streamovania cyklov

#### <a name="officeextensibilityappcommandsappcmdprojectionstatus"></a>Office.Extensibility.AppCommands.AppCmdProjectionStatus

Zhromažďuje informácie na sledovanie, ktoré inštalácie doplnku balíka Office aktualizovali pás s nástrojmi úspešne a neúspešne.

Slúži na riešenie bežných problémov registrácie, keď doplnky nie sú nainštalované správne a z toho dôvodu sú nepoužiteľné.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityappcommandsaddsolution"></a>Office.Extensibility.AppCommands.AddSolution

Zhromažďuje informácie o inštalácii pre doplnky balíka Office, ktorými sa prispôsobuje pás s nástrojmi.  Používa sa na zisťovanie problémov s tým, ako vlastné doplnky upravujú pás s nástrojmi balíka Office.
 
Zhromažďujú sa tieto polia:

- **AppVersion** – verzia aplikácie

- **SolutionId** – ID riešenia

- **StoreType** – označuje pôvod aplikácie


#### <a name="officeextensibilitycatalogexchangegetentitlements"></a>Office.Extensibility.Catalog.ExchangeGetEntitlements

Údaje o úspešnom a neúspešnom načítaní údajov nároku na doplnok pre doplnky priradené správcom nájomníka služieb Office 365. Slúžia na metriku stavu, grafy a analýzu problémov zákazníkov.

Zhromažďujú sa tieto polia:

  - **CachingResult** – výsledok pokusu o uloženie vrátenej hodnoty volania služby

  - **ClientParameter** – identifikátor klienta odoslaný počas volania služby

  - **EntitlementsCount** – počet nárokov očakávaných v odpovedi na volanie

  - **EntitlementsParsed** – počet nárokov analyzovaných z odpovede

  - **IsAllEntitlementsParsed** – označuje, či sa počet očakávaných nárokov zhoduje s analyzovaným počtom nárokov

  - **ServiceCallHResult** – výsledok vrátený rozhraním API volania služby

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa

  - **UsedCache** – označuje, či bol použitá odpoveď z vyrovnávacej pamäte namiesto volania služby

  - **VersionParameter** – číslo verzie balíka Office odoslané v rámci volania služby

#### <a name="officeextensibilitycatalogexchangegetlastupdate"></a>Office.Extensibility.Catalog.ExchangeGetLastUpdate

Údaje o úspešnom a neúspešnom načítaní potrebných aktualizovaných údajov o doplnkoch priradených správcom nájomníka služieb Office 365. Slúžia na metriku stavu, grafy a analýzu problémov zákazníkov. ExchangeGetLastUpdate sa spustí vždy pri štarte v rámci kódu hostiteľa a určí, či sa zmenili priradenia doplnku pre používateľa.   Ak áno, potom sa načíta osf.DLL, aby sme mohli volať ExchangeGetEntitlements a získať konkrétne priradenia (a ExchangeGetManifests sa zavolá, aby sa načítal každý nový manifest, ktorý bude potrebný).   ExchangeGetEntitlements (a ExchangeGetManifests) je možné tiež volať na požiadanie po spustení hostiteľskej aplikácie.   Cieľom je nenačítať veľkú knižnicu DLL, ak to nie je potrebné.   Bez toho, aby táto udalosť bola medzi povinnými údajmi, by nebolo možné zistiť, či sa používateľom nedarí získať im priradené doplnky, ak prvé volanie služby nie je úspešné.   Ide tiež o hlavný signál pre všetky problémy s overovaním, s ktorými sa stretávame, keď hovoríme so službou.

Zhromažďujú sa tieto polia:

  - **Abort** – označuje, či bol hostiteľ vypnutý počas volania služby

  - **AllowPrompt** – označuje, či bolo zapnuté zobrazovanie výziev na overenie

  - **AuthScheme** – schému overenia požadovaná serverom Exchange

  - **BackEndHttpStatus** – kód protokolu HTTP oznámený pri komunikácii so serverom Exchange

  - **BackupUrl** – sekundárna URL adresu servera Exchange na volanie

  - **BEServer** – názov servera Exchange

  - **CalculatedBETarget** – úplný názov počítača servera Exchange

  - **Call(n)\_TokenAuthError** – chyba overenia n-tého pokusu o volanie služby

  - **Call(n)\_TokenIsValid** – označuje, či bol overovací token platný pri n-tom pokuse o volanie služby

  - **CallMethod** – reťazec označujúci cestu, ktorou išiel kód

  - **ConfigSvcReady** – označuje, či služba konfigurácie už bola inicializovaná

  - **Date** – hodnota vrátená zo servera Exchange

  - **DiagInfo** – informácie vrátené zo servera Exchange

  - **End\_TicketAuthError** – každá chyba pri získavaní overovacieho lístka po volaní služby

  - **End\_TokenIsValid** – označuje, či je overovací lístok platný po volaní služby

  - **EndingIdentityState** – nahlásený stav objektov identity po uskutočnení volania služby

  - **EwsHandler** – hodnota vrátená zo servera Exchange

  - **FEServer** – klientske rozhranie servera Exchange, ktoré rieši žiadosť

  - **HResult** – kód výsledku

  - **HttpStatus** – kód stavu protokolu HTTP vrátený zo servera Exchange

  - **IsSupportedAuthResponse** – označuje, či typ overenia patrí medzi použiteľné

  - **LastUpdateValueRegistry** – hodnota hash načítaná z databázy Registry

  - **LastUpdateValueRetrieved** – hodnota hash vrátená z volania služby

  - **MSDiagnostics** – hodnota vrátená zo servera Exchange

  - **MsoHttpResult** – hodnota enumerátora vrátená z rozhrania API protokolu HTTP

  - **NeedRefresh** – pole s hodnotou true alebo false, ktoré označuje, či je údaj o doplnku zastaraný a je potrebné ho aktualizovať.

  - **PrimaryUrl** – hlavná URL adresa, na ktorú sa uskutočňuje volanie služby

  - **RequestId** – hodnota vrátená zo servera Exchange

  - **RequestTryCount** – počet našich pokusov o uskutočnenie volania služby

  - **RequestTryCount** – počet našich pokusov o komunikáciu so serverom Exchange

  - **ResultChain** – rad kódu výsledku z každého pokusu o volanie služby

  - **StartingIdentityState** – nahlásený stav objektov identity pred uskutočnením volania služby

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa, či je potrebné vykonať ďalšie volania služby

#### <a name="officeextensibilitycatalogexchangegetmanifests"></a>Office.Extensibility.Catalog.ExchangeGetManifests

Údaje o úspešnom a neúspešnom načítaní údajov manifestov doplnkov pre doplnky priradené správcom nájomníka služieb Office 365. Slúžia na metriku stavu, grafy a analýzu problémov zákazníkov.

Zhromažďujú sa tieto polia:

  - **CachedManifestsParsed** – počet manifestov nachádzajúcich sa vo vyrovnávacej pamäti

  - **IsAllReturnedManifestsParsed** – označuje, či bolo možné analyzovať všetky vrátené manifesty

  - **ManifestsRequested** – počet potrebných manifestov

  - **ManifestsReturned** – počet manifestov vrátených zo servera

  - **ManifestsToRetrieve** – počet manifestov, ktoré sa majú získať zo servera

  - **ReturnedManifestsParsed** – počet manifestov vrátených zo servera, ktoré boli úspešne analyzované

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa

#### <a name="officeextensibilityuxfensureloadosfdll"></a>Office.Extensibility.UX.FEnsureLoadOsfDLL 

Sleduje zlyhanie načítania Osf.DLL. Zisťuje neúspešne načítanú knižnicu DLL, ktorá bráni spusteniu funkcie.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityuxfensureloadosfuidll"></a>Office.Extensibility.UX.FEnsureLoadOsfUIDLL 

Sleduje zlyhanie načítania OsfUI.DLL. Zisťuje neúspešne načítanú knižnicu DLL, ktorá bráni spusteniu funkcie.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityuxfensureosfshareddllload"></a>Office.Extensibility.UX.FEnsureOsfSharedDLLLoad 

Sleduje zlyhanie načítania OsfShared.DLL. Zisťuje neúspešne načítanú knižnicu DLL, ktorá bráni spusteniu funkcie.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officeextensibilityvbatelemetrycomobjectinstantiated"></a>Office.Extensibility.VBATelemetryComObjectInstantiated

Zhromažďuje informácie o vyvolaní automatizačného servera alebo klienta v riešeniach VBA. Umožňuje pochopiť interakciu medzi VBA a objektami COM

Zhromažďujú sa tieto polia:

  - **ComObjectInstantiatedCount** – počet inštancií objektov COM

  - **HashComObjectInstantiatedClsid** – hodnota hash identifikátora triedy objektu COM

  - **HashProjectName** – hodnota hash názvu projektu VBA

  - **TagId** – jedinečná značka

#### <a name="officeextensibilityvbatelemetrydeclare"></a>Office.Extensibility.VBATelemetryDeclare 

Zhromažďuje informácie o vyvolaní rozhraní API Win32 v riešeniach VBA. Umožňuje pochopiť interakciu medzi VBA a používaním a doplniť vyšetrovania zabezpečenia.

Zhromažďujú sa tieto polia:

  - **DeclareCount** – počet deklarácií

  - **HashDeclare** – hodnota hash názvu knižnice DLL

  - **HashEntryPoint** – hodnota hash názvu rozhrania API

  - **HashProjectName** – hodnota hash názvu projektu VBA

  - **IsPtrSafe** – označuje, či je vyhlásenie deklarácie kompatibilné s inou architektúrou

  - **TagId** – jedinečná značka

#### <a name="officeoutlookdesktopadd-insadd-inloaded"></a>Office.Outlook.Desktop.Add-ins.Add-inLoaded

Zhromažďuje informácie o úspešnom a neúspešnom načítaní doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook správne fungoval s doplnkami zákazníkov. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

  - **Štandardná aktivita HVA** bez vlastnej údajovej časti

#### <a name="officeoutlookmacaddinapiusage"></a>Office.Outlook.Mac.AddinAPIUsage

Zhromažďuje informácie o úspešných a neúspešných spusteniach doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook fungoval s doplnkami správne. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

- **AccountType** – typ konta priradeného k doplnku 

- **Cookie** – súbor cookie, ktorý je používaný doplnkom

- **DispId** – identifikátor odoslania 

- **EndTime** – čas skončenia doplnku 

- **ExecutionTime** – čas uplynutý počas spustenia doplnku 

- **Výsledok** – výsledok použitia doplnku v Outlooku 

- **StartTime** – čas spustenia doplnku


#### <a name="officeoutlookmacaddineventapisusage"></a>Office.Outlook.Mac.AddinEventAPIsUsage

Zhromažďuje informácie o úspešných alebo neúspešných spusteniach doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook fungoval s doplnkami správne. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

- **AddinType** – typ doplnku 

- **EventAction** – akcia vykonaná doplnkom 

- **EventDispid** – identifikátor odoslania

- **EventResult** – výsledok akcie vykonanej doplnkom 

#### <a name="officeoutlookmacaddininstallationfrominclientstore"></a>Office.Outlook.Mac.AddInInstallationFromInClientStore

Zhromažďuje informácie o úspešných alebo neúspešných inštaláciách doplnku v Outlooku. Tieto údaje sú aktívne monitorované, aby Outlook fungoval s doplnkami správne. Tieto údaje sa používajú na zistenie a vyšetrovanie problémov.

Zhromažďujú sa tieto polia:

- **AccountType** – typ konta priradeného k doplnku 

- **FailureReason** – dôvod zlyhania inštalácie doplnku 

- **MarketplaceAssetId** – identifikátor obchodu s doplnkami 

- **Status** – stav inštalácie doplnku


#### <a name="officeprogrammabilityaddinsinternalsetconnectenterprise"></a>Office.Programmability.Addins.InternalSetConnectEnterprise

Udalosť vygenerovaná pri načítaní doplnku COM v podnikovom zariadení. Používa sa na určenie problémov s prijatím, výkonom a spoľahlivosťou doplnkov balíka Office. 

Zhromažďujú sa tieto polia:

  - **Activity Result** – stav úspechu pripojenia *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

  - **AddinConnectFlag** – predstavuje správanie pri načítaní 

  - **AddinDescriptionV2** – popis doplnku

  - **AddinFileNameV2** – názov súboru doplnku bez cesty k súboru

  - **AddinFriendlyNameV2** – popisný názov doplnku

  - **Add-inId** – ID triedy doplnku *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

  - **AddinIdV2** – identifikátor triedy doplnku

  - **AddinProgIdV2** – identifikátor programu doplnku

 - **AddinProviderV2** – poskytovateľ doplnku

  - **Add-inTimeDateStamp** – časová pečiatka doplnku z metaädajov súboru DLL *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

  - **AddinTimeDateStampV2** – časová pečiatka doplnku z metaúdajov knižnice DLL

  - **AddinVersionV2** – verzia doplnku

  - **IsBootInProgress** – či sa aplikácia balíka Office spúšťa
 
  - **LoadDuration** – trvanie načítania doplnku
  
  - **LoadResult** – stav úspechu načítania


#### <a name="officevisiovisioaddonload"></a>Office.Visio.Visio.AddonLoad

Zaznamenáva chyby, keď riešenie zlyhá pri načítavaní. Potrebné pri ladení chýb načítania doplnku vo Visiu.

Zhromažďujú sa tieto polia:

  - **Data\_Load1Error:integer** – hodnotu chyby počas načítania doplnku Visia

#### <a name="officevisiovisioaddonusage"></a>Office.Visio.Visio.AddonUsage

Zaznamenáva chyby v prípade chyby vo funkčnosti riešenia. Potrebné pri ladení chýb načítania doplnku v doplnkoch.

Zhromažďujú sa tieto polia:

  - **Data\_DocumentSessionLogID:string** – identifikátor relácie dokumentu

  - **Data\_IsEnabled**:**bool** – hodnota true, ak je riešenie povolené

  - **Data\_TemplateID:string** – identifikátor GUID šablóny, v ktorej sa načítalo riešenie. Záznam 0 pre vlastné riešenie

  - **Data\_AddOnID**:**string** – identifikátor GUID na identifikáciu načítaného doplnku

  - **Data\_Error**:**integer** – ID chyby

### <a name="security-subtype"></a>*Podtyp zabezpečenia*

Chybové stavy dokumentu, funkcie a doplnku, ktoré môže ohroziť zabezpečenie, vrátane pripravenosti na aktualizáciu produktu.

#### <a name="officeappguardcreatecontainer"></a>Office.AppGuard.CreateContainer

Zhromažďujeme kódy chýb a informácie o tom, či kontajner už existoval alebo nie. Tiež zhromažďujeme kódy chýb pre udalosť resetovania pre prípad, že sa nám nepodarí vytvoriť kontajner na prvý pokus. Údaje sa použijú na určenie percentuálneho podielu relácií, v ktorých úspešne vytvoríme kontajner na spustenie aplikácií Office Application Guard. Údaje tiež umožnia spoločnosti Microsoft identifikovať a riešiť kódy chýb z vytvorenia kontajnera.

Zhromažďujú sa tieto polia:

- **ErrorCode1** – typ kódu chyby nastavenia kontajnera.  

- **ErrorCode2** – kód chyby z vykonania vytvorenia. 

- **ErrorCode3** – dodatočný kód chyby. 

- **Id** – jedinečný identifikátor (GUID) pre vytvorenie kontajnera.

- **ResetError** – kód chyby z pokusu o resetovanie kontajnera po neúspešnom pokuse.

- **ResetErrorCode1** – typ kódu chyby nastavenia kontajnera po príkaze resetovania. 

- **ResetErrorCode2** – kód chyby z vykonania vytvorenia po príkaze resetovania.

- **ResetErrorCode3** – dodatočný kód chyby po príkaze resetovania.

- **ResetErrorType** – typ chyby počas resetovania: vytvorenie, príprava súboru alebo spustenie.

- **WarmBoot** – určuje, či kontajner už bol vytvorený alebo nie.

#### <a name="officeappguardlaunchfile"></a>Office.AppGuard.LaunchFile

Táto udalosť označuje výsledok spustenia súboru spustenia služby Application Guard. Budeme môcť určiť percentuálny podiel relácií, v ktorých sme úspešne spustili wordový, excelový alebo powerpointový súbor a kódy chýb pre neúspešné pokusy.

Zhromažďujú sa tieto polia:

- **AppId** – určuje, ktorá aplikácia sa spúšťa.

- **DetachedDuration** – určuje celkový čas trvania zlúčenej aktivity. 

- **ErrorCode1** – typ kódu chyby nastavenia kontajnera.  

- **ErrorCode2** – kód chyby z vykonania vytvorenia. 

- **ErrorCode3** – dodatočný kód chyby. 

- **FileId** – jedinečný identifikátor (GUID) vrátený z rozhrania API Windowsu po spustení súboru.

- **Id** – jedinečný identifikátor (GUID) pre spustenie a vytvorenie súboru. Tento identifikátor sa používa na vytváranie súvislostí medzi udalosťami z Office a Windows.

- **ResetError** – kód chyby z pokusu o resetovanie kontajnera po neúspešnom pokuse.

- **ResetErrorCode1** – typ kódu chyby nastavenia kontajnera po príkaze resetovania. 

- **ResetErrorCode2** – kód chyby z vykonania vytvorenia po príkaze resetovania.

- **ResetErrorCode3** – dodatočný kód chyby po príkaze resetovania.  

- **ResetErrorType** – typ chyby: vytvorenie, príprava súboru alebo spustenie.



#### <a name="officesecurityactivationfilterclsidactivated"></a>Office.Security.ActivationFilter.CLSIDActivated

Sleduje, kedy sa konkrétny identifikátor triedy (Flash, Silverlight atď.) aktivuje v Office. Umožňuje sledovať vplyv blokovania ovládacích prvkov Flash, Silverlight a Shockwave na koncových používateľov.

Zhromažďujú sa tieto polia:

  - **ActivationType** – typ aktivácie ovládacieho prvku

  - **Blocked** – označuje, či bol ovládací prvok zablokovaný balíkom Office

  - **CLSID** – identifikátor triedy ovládacieho prvku

  - **Count** – označuje, koľkokrát bol ovládací prvok aktivovaný

#### <a name="officesecurityactivationfilterfailedtoregister"></a>Office.Security.ActivationFilter.FailedToRegister

Sleduje chyby v obmedzení rizík zabezpečenia, ktoré blokuje aktiváciu nebezpečných ovládacích prvkov v Office.

Umožňuje diagnostiku chýb v obmedzení rizík zabezpečenia, ktoré môžu mať vplyv na zabezpečenie koncových používateľov.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officesecuritycomsecurityfileextensionlistfromservice"></a>Office.Security.ComSecurity.FileExtensionListFromService

Sleduje, či boli prečítané prípony blokovania balíčkovača v službe konfigurácie alebo bol použitý predvolený zoznam klienta. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **RetrievedFromServiceStatus** – označuje, či sa načítal zoznam prípon súborov, ktoré sa majú blokovať, a ak nie, čo bolo dôvodom chyby

#### <a name="officesecuritycomsecurityload"></a>Office.Security.ComSecurity.Load

Sleduje, keď sa načíta objekt OLE v dokumente. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Clsid** – identifikátor triedy ovládacieho prvku OLE

  - **Count** – označuje, koľkokrát bol načítaný ovládací prvok OLE

  - **DocUrlHash** – hodnota hash predstavujúca dokument jednoznačne. (Poznámka: Skutočné podrobnosti o dokumente sa z tohto nedajú zistiť žiadnym spôsobom. Ide len o jedinečné označenie dokumentu.)

  - **IsCategorized** – označuje, či bol ovládací prvok OLE kategorizovaný na načítanie v Office

  - **IsInsertable** – označuje, či je ovládací prvok OLE vložiteľný alebo nie

#### <a name="officesecuritycomsecurityobjdetected"></a>Office.Security.ComSecurity.ObjDetected

Sleduje, keď sa zistí objekt OLE v dokumente. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Clsid** – identifikátor triedy ovládacieho prvku OLE

  - **Count** – koľkokrát bol tento objekt OLE zistený

  - **DocUrlHash** – hodnota hash predstavujúca dokument jednoznačne. (Poznámka: Skutočné podrobnosti o dokumente sa z tohto nedajú zistiť žiadnym spôsobom. Ide len o jedinečné označenie dokumentu.)

  - **IsCategorized** – označuje, či je ovládací prvok OLE kategorizovaný na načítanie v Office

  - **IsInsertable** – označuje, či je ovládací prvok OLE vložiteľný alebo nie

#### <a name="officesecuritycomsecuritypackageractivation"></a>Office.Security.ComSecurity.PackagerActivation

Sleduje výsledok obmedzenia rizík zabezpečenia, ktoré blokuje nebezpečné prípony vložené v dokumentoch balíka Office. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **FromInternet** – označuje, či bol dokument z internetu

  - **PackagerSetting** – označuje, aké bolo aktuálne nastavenie balíčkovača

  - **TrustedDocument** – označuje, či bol dokument dôveryhodným dokumentom

#### <a name="officesecuritycomsecuritypackageractivationerrors"></a>Office.Security.ComSecurity.PackagerActivationErrors

Sleduje chyby v obmedzení rizík zabezpečenia, ktoré blokuje nebezpečné prípony vložené v dokumentoch balíka Office. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Error** – kód chyby

  - **Extension** – označuje, aká bola prípona súboru

  - **FromInternet** – označuje, či bol dokument z internetu

  - **LinkedDocument** – označuje, či to bol alebo nebol prepojený dokument

  - **PackagerSetting** – označuje, aké bolo aktuálne nastavenie balíčkovača

  - **TrustedDocument** – označuje, či bol dokument dôveryhodný


#### <a name="officesecuritymacrointernetvbablockenabled"></a>Office.Security.Macro.InternetVBABlockEnabled

Sleduje, či je v klientovi zapnuté nastavenia blokovania makra z internetu. Slúži na vyhodnotenie použitia obmedzenia rizík zabezpečenia na ochranu pred škodlivými makrami.

Zhromažďujú sa tieto polia:

  - Žiadne

#### <a name="officesecuritymacropolicydigsigtrustedpublishers"></a>Office.Security.Macro.PolicyDigSigTrustedPublishers

Sleduje, či bolo makro overené a pochádza od dôveryhodného vydavateľa. Umožňuje zabezpečiť efektivitu obmedzenia rizík zabezpečenia, ktoré chráni koncových používateľov balíka Office.

Zhromažďujú sa tieto polia:

  - **Policy** – označuje, či politika je alebo nie je nastavená, alebo nie je k dispozícii

#### <a name="officesecuritymacroprompted"></a>Office.Security.Macro.Prompted

Sleduje, keď sa používateľovi zobrazí výzva na povolenie makier VBA. Umožňuje vyhodnotiť výskyt makier VBA a zavádzať budúce obmedzenia rizík zabezpečenia, ktoré obmedzia spustenia makier v rámci odozvy na incidenty zabezpečenia.

Zhromažďujú sa tieto polia:

  - **PromptType** – označuje, aký typ výzvy sa zobrazil

  - **VBAMacroAntiVirusHash** – antivírusová hodnota hash makra

  - **VBAMacroAntiVirusHRESULT** – výsledok antivírusového hodnotenia

#### <a name="officesecuritymacrovbasecureruntimesessionenablestate"></a>Office.Security.Macro.VBASecureRuntimeSessionEnableState

Sleduje každé overenie režimu Runtime AMSI, ktoré sa uskutoční pri spustení makra. Sleduje efektivitu overenia režimu Runtime AMSI pri spustení makra a identifikuje chyby, ktoré môžu mať vplyv na zabezpečenie koncových používateľov.

Zhromažďujú sa tieto polia:

  - **IsRegistry** – označuje, či správca nastavil nejaké prepisovanie v databáze Registry

  - **State** – označuje, aký je stav zabezpečenia režimu Runtime

#### <a name="officesecuritymacroxl4prompted"></a>Office.Security.Macro.XL4Prompted

Sleduje, keď sa používateľovi zobrazí výzva na povolenie makier XL4. Umožňuje vyhodnotiť výskyt makier XL4 v Exceli a zavádzať budúce obmedzenia rizík zabezpečenia, ktoré predvolene blokujú XL4 v rámci odozvy na incidenty zabezpečenia, ktoré sa týkajú zneužitia makier XL4.

Zhromažďujú sa tieto polia:

  - **PromptType** – označuje, aký typ výzvy sa zobrazil


#### <a name="officesecurityocxufiprompt"></a>Office.Security.OCX.UFIPrompt

Sleduje, keď sa používateľovi zobrazí upozornenie zabezpečenia pri načítaní ovládacieho prvku ActiveX, ktorý je označený ako nebezpečný na inicializáciu. Umožňuje sledovať výskyt ovládacích prvkov UFI ActiveX v dokumentoch balíka Office a zavádzať obmedzenia rizík (napr. ovládacie prvky Killbitting) v rámci odozvy na incidenty zabezpečenia.

Zhromažďujú sa tieto polia:

  - **IsFromInternet** – označuje, či je dokument otvorený z internetu

  - **IsSecureReaderMode** – označuje, či je dokument otvorený v zabezpečenej čítačke

  - **OcxTrustCenterSettings** – označuje, aké je aktuálne nastavenie technológie ActiveX


#### <a name="officesecuritysecurereaderhostopeninosr"></a>Office.Security.SecureReaderHost.OpenInOSR

Sleduje dokončenie otvorenia súboru v chránenom zobrazení. Umožňuje diagnostiku podmienok, ktoré vedú k zlyhaniu pri otváraní súborov v chránenom zobrazení, čo má vplyv na zabezpečenie a produktivitu zákazníkov.

Zhromažďujú sa tieto polia:

  - Žiadne

## <a name="product-and-service-usage-data-events"></a>Udalosti v kategórii Údaje o používaní produktov a služieb

Toto sú podtypy údajov v tejto kategórii:

- [Úspešnosť funkcie aplikácie](#application-feature-success-subtype)
- [Stav a spustenie aplikácie](#application-status-and-boot-subtype)
- [Konfigurácia zjednodušenia ovládania balíka Office](#office-accessibility-configuration-subtype)
- [Ochrana osobných údajov](#privacy-subtype)


### <a name="application-feature-success-subtype"></a>*Podtyp Úspešnosť funkcie aplikácie*

Úspešnosť fungovania aplikácie. Obmedzené na otvorenie a zatvorenie aplikácie a dokumentov, úpravu súborov a zdieľanie súborov (spoluprácu).

#### <a name="accountaction"></a>account.action

Potrebné na zabezpečenie správneho fungovania konfigurácie konta a používa sa na monitorovanie stavu vytvárania konta, možnosti pridávania nových e-mailových kont a monitorovania mäkkých resetov kont 

Zhromažďujú sa tieto polia: 

- **account_calendar_count** – koľko kalendárov má konto
 
- **action** – typ vykonanej akcie, napr. create_account alebo delete_account.
 
- **duration_seconds** – trvanie akcie
 
- **entry_point** – vstupný bod akcie, spôsob spustenia akcie používateľom
 
- **has_hx** – označuje, či má zariadenie konto, ktoré používa našu novú službu synchronizácie pošty, nejedná sa nevyhnutne o konto, v ktorom bola akcia vykonaná
 
- **is_hx** – ide o konto používajúce našu novú službu synchronizácie pošty
 
- **is_shared_mailbox** – označuje, či sa akcia vzťahuje na zdieľanú poštovú schránku
 
- **number_of_accounts** – celkový počet kont, v ktorých bola akcia vykonaná
 
- **result** – výsledok akcie, napr. úspech alebo neúspech.
   
- **server_type** – typ servera pre konto, podobný ako pre account_type
 
- **shared_type** – typ zdieľaného konta (ak je konto zdieľané)
 
- **scope** – rozsah akcie, pre akciu delete je to this_device alebo all_devices
 
- **total_calendar_accounts** – počet kont kalendárov v aplikácii v čase akcie
 
- **total_email_accounts** – počet e-mailových kont v aplikácii v čase akcie
 
- **total_file_accounts** – počet kont súborov v aplikácii v čase akcie

#### <a name="accountlifecycle"></a>account.lifecycle

Táto udalosť sa zhromažďuje na zabezpečenie správneho fungovania konfigurácie konta a používa sa na monitorovanie stavu vytvárania konta, možnosti pridávania nových e-mailových kont a monitorovania mäkkých resetov kont.

Zhromažďujú sa tieto polia: 

- **account_creation_source** – voliteľná vlastnosť, ktorá sa používa na nájdenie a diagnostiku akýchkoľvek problémov, ktoré sa vyskytnú pri vytváraní konta pri pridávaní typu akcie.  Môže mať hodnoty, ako sú single sign-on (SSO), create_new_account, manual, atď.

- **action** – typ akcie vykonanej na konte, napríklad pridanie, odstránenie alebo resetovanie

#### <a name="addnewaccountstep"></a>add.new.account.step

Táto udalosť nám umožňuje zistiť, ako ďaleko sa používateľ dostal vo formulári vytvorenia nového konta.  Označuje, keď používateľ prešiel do ďalšieho kroku, alebo či zrušil.  Tieto informácie potrebujeme na určenie, či niektoré kroky zlyhávajú, a na zaručenie, že vytvorenie používateľského konta bolo úspešné. 

Zhromažďuje sa toto pole: 

- **OTAddAccountCurrentStep** – môže mať tieto hodnoty: profile_form, redirect_mobile_check, mobile_check_success

#### <a name="apperror"></a>app.error

Sleduje použité kritické chyby aplikácie, aby sme mohli zabrániť problémom, ktoré by mohli spôsobiť zlyhanie aplikácie alebo zabránenie čítaniu e-mailov.

Zhromažďujú sa tieto polia: 

- **clientName** – názov klienta pre cloudový súbor, kde sa vyskytla chyba (ak je k dispozícii).

- **cloudfile_error_type** – typ chyby, ktorá sa vyskytla pre cloudový súbor (ak je k dispozícii).

- **cloudfile_response_name** – názov odozvy pre chybu, ktorá sa vyskytla pre cloudový súbor (ak je k dispozícii).

- **component_name** – názov súčasti aplikácie, v ktorej sa vyskytla chyba, napríklad pošta alebo kalendár.

- **debug_info** – informácie o chybe, ktorá sa vyskytla pre cloudový súbor, slúžiace na určenie príčiny chyby.

- **error_origin_identifier** – pôvod chyby, ktorá sa vyskytla pri koncepte, v ktorom sa vyskytla chyba (ak je k dispozícii).

- **error_type** – typ chyby, ktorá sa vyskytla. Medzi príklady patrí ukladanie konceptu, odoslanie konceptu a chyba cloudového súboru.

- **exdate** – dátum rozšíreného pravidla (vzťahuje sa iba na chyby opakovania plánovanej činnosti) *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **exrule** – hodnota rozšíreného pravidla (vzťahuje sa iba na chyby opakovania plánovanej činnosti) *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **has_attachments** – znázorňuje, či má koncept, v ktorom sa vyskytla chyba, prílohy (ak je k dispozícii).

- **is_IRM_protected** – znázorňuje, či je koncept, v ktorom sa vyskytla chyba, chránený Správou prístupových práv k informáciám (ak je k dispozícii).

- **is_legitimate** – znázorňuje, či chyba pochádza z programovacej chyby alebo nie. Chyby programovania sa považujú za neoprávnené.

- **is_local** – znázorňuje, či je koncept, v ktorom sa vyskytla chyba, synchronizovaný so serverom (ak je k dispozícii).

- **is_recoverable** – znázorňuje, či je možné obnovenie po chybe alebo či ide o závažnú chybu.

- **rdate** – dátum pravidla opakovania (vzťahuje sa iba na chyby opakovania plánovanej činnosti) *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **rrule** – samotné pravidlo opakovania (vzťahuje sa iba na chyby opakovania plánovanej činnosti) *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **rrule_error_message** – chybové hlásenie o analýze pravidla opakovania (vzťahuje sa iba na chyby opakovania plánovanej činnosti) *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **rrule_error_type** – typ chyby analýzy pravidla opakovania (vzťahuje sa iba na chyby opakovania plánovanej činnosti) *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **status_code** –kód stavu chyby, ktorá sa vyskytla. Pomáha pochopiť príčinu chyby.

Možné vlastnosti sú aj všetky znaky. Pomáha pochopiť znaky v texte hlásenia konceptu, keď sa vyskytla chyba. Možné vlastnosti sú napríklad „a“, „b“ alebo „c“.

#### <a name="applaunchreport"></a>app.launch.report

Táto udalosť nám umožňuje zistiť a vyriešiť problémy spôsobujúce pomalé alebo neúplné spúšťanie Outlooku, čo používateľom sťažuje používanie aplikácie. Patria sem informácie o konkrétnych povolených funkciách a o dĺžke trvania spustenia konkrétnych častí.

Zhromažďujú sa tieto polia: 

- **is_agenda_widget_active** – uvádza, či je miniaplikácia agendy aktívna.

- **is_alert_available** – hovorí nám, či má aplikácia nakonfigurované povolenie upozornení v oznámeniach.

- **is_background_refresh_available** – hovorí, či je aplikácia nakonfigurovaná tak, aby sa mohla aktualizovať na pozadí.

- **is_badge_available** – hovorí nám, či má aplikácia nakonfigurované povolenie štítkov v oznámeniach.

- **is_intune_managed** – hovorí nám, či je aplikácia spravovaná službou Intune.

- **is_registered_for_remote_notifications** – hovorí nám, či má aplikácia zaregistrované vzdialené oznámenia.

- **is_sound_available** – hovorí nám, či má aplikácia nakonfigurované povolenie zvukov v oznámeniach.

- **is_watch_app_installed** – uvádza, či bola nainštalovaná hodinková aplikácia Outlook.

- **is_watch_paired** – hovorí nám, či je hodinková aplikácia Outlook spárovaná s hlavnou aplikáciou Outlook.

- **launch_to_db_ready_ms** – hovorí nám množstvo času od spustenia aplikácie Outlook po moment, kedy bola databáza pripravená.

- **num_calendar_accounts** – uvádza počet kont kalendára v aplikácii.

- **num_cloud_file_accounts** – uvádza počet kont ukladacieho priestoru v aplikácii.

- **num_hx_calendar_accounts** – uvádza počet kont kalendára v aplikácii, ktoré sú pripojené k našej novej službe synchronizácie pošty.

- **num_hx_mail_accounts** – uvádza počet poštových kont v aplikácii, ktoré sú pripojené k našej novej službe synchronizácie pošty.

- **num_calendar_accounts** – uvádza počet poštových kont v aplikácii.

#### <a name="calendaraction"></a>calendar.action

Používa sa na sledovanie akéhokoľvek možného nepriaznivého vplyvu na schopnosť vykonávať základné akcie kalendára, ako je vytváranie alebo úprava udalostí.  Udalosť tiež môže obsahovať rad názvov vlastností a to, či sa zmenili, alebo nie. Napríklad „title_changed“, „online_meeting_changed“ a „description_changed“ sú názvy zahrnutých vlastností, vďaka ktorým dokážeme zistiť, či sa vyskytli nejaké problémy s úpravou určitých vlastností.

Zhromažďujú sa tieto polia: 

- **account_sfb_enabled** – pomáha správne nakonfigurovať Skype for Business. 

- **action** – typ akcie, ktorá bola vykonaná v kalendári. Patria sem akcie ako otvorenie, úpravy, pridanie skratky, odloženie atď. Pomáha zabezpečiť, aby kalendár fungoval podľa očakávania a nič sa nepokazilo. 

- **action_result** – výsledok akcie vykonanej na súčastiach kalendára. Môžu sem patriť hodnoty ako úspech, neúspech, neznáme a časový limit. Slúži na sledovanie úspešnosti akcií a na zistenie, či neexistuje rozsiahly problém s akciami v kalendári. 

- **attendee_busy_status** – voľný/zaneprázdnený stav účastníka, ktorého sa akcia týka. Táto hodnota môže byť voľný, zaneprázdnený alebo nezáväzne. Pomáha pochopiť, či sa vyskytol problém s akciami týkajúcimi sa určitého zaneprázdneného stavu. 

- **availability** – hodnota dostupnosti, ak sa hodnota voľný/zaneprázdnený na schôdzi zmenila. Pomáha pochopiť, či sa vyskytli problémy s nastavením určitej hodnoty dostupnosti. 

- **calendar_onlinemeeting_default_provider** – obsahuje predvoleného poskytovateľa online schôdzí, ktorý sa používa pri vytváraní online schôdzí podporovaných serverom. Patrí sem napríklad Skype, Skype for Business, Hangouts a Teams for Business. Pomáha diagnostikovať možné problémy pri vytváraní online schôdzí niektorých poskytovateľov. 

- **calendar_onlinemeeting_enabled** – má hodnotu true, ak kalendár podporuje tvorbu online schôdzí podporovaných serverom na základe predvoleného poskytovateľa online schôdzí. Pomáha pochopiť, či sa vyskytli nejaké problémy s kalendármi s povolenými online schôdzami. 

- **calendar_type** – typ kalendára, v ktorom sa udalosť bude nachádzať po úprave schôdze používateľom. Možné hodnoty sú primárny, sekundárny, zdieľaný a skupinový. Pomáha pochopiť, či sa vyskytli problémy s niektorým typom kalendára. 

- **delete_action_origin** – pôvod vykonanej akcie odstránenia. Patria sem hodny ako navigačný panel, panel s nástrojmi a tabletkový panel s nástrojmi.  Pomáha pochopiť, či sa vyskytli nejaké problémy pri odstraňovaní schôdze z určitého umiestnenia. 

- **distribution_list_count** – počet účastníkov v distribučných zoznamoch. Pomáha sledovať, či sa nevyskytli problémy s účastníkmi v distribučných zoznamoch. 

- **guest_count** – počet hostí na schôdzi.  Pomáha so správnym pridávaním hostí. 

- **is_all_day** – spolu s „meeting_duration“ slúži na určenie toho, či ide o celodennú schôdzu. Pomáha pochopiť, či sa vyskytli nejaké problémy s akciami vykonanými počas celodenných schôdzí. 

- **is_location_permission_granted** – či používateľ aplikácii udelil povolenie na systémové umiestnenie. Ak je povolenie na umiestnenie udelené, aplikácia môže v používateľskom rozhraní zobraziť ďalšie informácie o pomôckach. Keď vieme, či bolo povolenie na umiestnenie udelené, umožňuje nám to zistiť, ako často sa používateľom zobrazujú ďalšie informácie o pomôckach.

- **is_organizer** – pomáha pochopiť, či organizátor dokáže správne upravovať a vytvárať schôdze. 

- **is_recurring** – pomáha pochopiť, či sa vyskytol problém, ktorý ovplyvňuje konkrétne opakované schôdze. 

- **launch_point** – spúšťací bod akcie. Môže ísť o hodnoty ako napríklad hlavička miniaplikácie, päta miniaplikácie, celodenná miniaplikácia a klávesová skratka kalendára. Pomáha pochopiť kontext, v ktorom sa akcia spustila. 

- **location_count** – počet umiestnení, ktoré sú nastavené pri vytvorení a upravení udalosti. Pomáha pochopiť, či sa vyskytli nejaké problémy s vytvorením alebo úpravou udalostí s určitým počtom umiestnení. 

- **location_selection_source_type** – typ zdroja výberu umiestnenia. Môže ísť o hodnoty ako napríklad návrh na umiestnenie, vlastné a existujúce. Pomáha diagnostikovať všetky problémy s výberom umiestnenia z určitého zdroja. 

- **location_session_id** – ID relácie výberu umiestnenia schôdze. Pomáha diagnostikovať všetky problémy s výberom umiestnenia na pridanie do schôdze. 

- **location_type** – typ vybraného umiestnenia.  Obsahuje typy ako napríklad vlastné umiestnenie, konferenčná miestnosť a Bing. Pomáha pochopiť problémy s pridaním určitých typov umiestnení do schôdze. 

- **meeting_duration** – dĺžka schôdze.  Pomáha zabezpečiť, aby mali schôdze nakonfigurované správne časy. 

- **meeting_insights_type** – typ prehľadov schôdze v podrobnostiach o udalosti.  Patria sem súbor a správa. Pomáha pochopiť počet zobrazovaných prehľadov schôdze. 

- **meeting_type** – typ online schôdze priradenej k akcii.  Patrí sem napríklad Skype, Skype for Business, Hangouts a Teams for Business. Pomáha zistiť, či sú online schôdze správne nakonfigurované. 

- **origin** – pôvod akcie kalendára. Patria sem typy ako agenda, kalendár, miniaplikácia agendy atď. Pomáha lepšie zabezpečiť správne interakcie v rámci súčastí kalendára. 

- **recurrence_scope** – typ opakovania schôdze, buď výskyt alebo rad.  Pomáha pochopiť, či sa vyskytli nejaké problémy s upravovaním rôznych typov opakovaní schôdze. 

- **reminder_time** – čas pripomenutia schôdze, ak sa zmenila.  Používa sa na uistenie, že čas pripomenutia schôdze bol uložený správne. 

- **reminders_count** – počet pripomenutí schôdze v prípade, že sa zmenili. Pomáha diagnostikovať všetky problémy s viacerými pripomenutiami udalosti. 

- **sensitivity** – citlivosť schôdze. Patria sem typy ako normálna, osobná, súkromná a dôverná. Pomáha pochopiť, či bola správne nastavená citlivosť schôdze. 

- **session_duration** – dĺžka trvania relácie v milisekundách. Pomáha pochopiť, či sa vyskytli problémy, ktoré zvyšujú čas potrebný na vykonanie akcie v kalendári. 

- **shared_calendar_result** – výsledok akcie vykonanej v zdieľanom kalendári. Možné hodnoty sú ok, žiadne povolenie, neznáme, lokálny vlastník a vlastník je skupina. Nám pochopiť spoľahlivosť akcií vykonaných v zdieľaných kalendároch. 

- **time_picker_origin** – pôvod nástroja na výber času pri akcii uloženia. Obsahuje hodnoty ako ďalšie možnosti a menej možností. Pomáha pochopiť, ako postupoval používateľ pri ukladaní schôdze a zabezpečiť správne fungovanie. 

- **title** – automaticky navrhnutý názov z hodnôt definovaných aplikáciou. Zahŕňa hodnoty ako Hovor, Obed a Skype. Pomáha pochopiť, či je automatické navrhovanie názvu správne nakonfigurované. 

- **txp** – typ objednania alebo rezervácie v udalosti (ak existuje). Patria sem typy ako rezervácia udalosti, rezervácia letu, rezervácia prenájmu auta atď. Pomáha pochopiť, či boli správne vykonané objednávacie/rezervačné karty. 

- **upcoming_event_count** – počet nadchádzajúcich udalostí zobrazených v zobrazení nadchádzajúcich udalostí. Pomáha pochopiť, či sa vyskytli problémy so zobrazením nadchádzajúcich udalostí. 

- **upcoming_event_seconds_until_event** – počet sekúnd do spustenia ďalšej naplánovanej udalosti. Pomáha pochopiť typické udalosti, ktoré sa zobrazujú v zobrazení nadchádzajúcich udalostí. 

- **value** – podrobnosti špecifické pre konkrétnu akciu ako napríklad dĺžka oneskorenia upozornenia alebo kategória opakovať do. Pomáha pochopiť kontext, v ktorom bola akcia vykonaná. 

#### <a name="combinedsearchuse"></a>combined.search.use

Používa sa na sledovanie možného nepriaznivého vplyvu na schopnosť vykonávať kľúčové funkcie vyhľadávania ako napríklad vyhľadávanie pošty, kontaktov alebo udalostí.

Zhromažďujú sa tieto polia v systémoch iOS a Android: 

- **account_switcher_action_type** – tento typ akcia zaznamená, či používateľ použije prepínač kont v jednoduchom zisťovaní alebo či sa rozhodne prepnúť konto.

- **action_type** – typ akcie, ktorá bola vykonaná na vyhľadávanie. Identifikuje, či sa vyhľadávanie začalo, prebieha alebo skončilo a aké akcie sa počas neho uskutočnili, napr. či bol použitý mikrofón. Pomáha s poskytovaním správnych a užitočných vyhľadávaní. 

- **conversation_id** – Jedinečný identifikátor pre každú reláciu vyhľadávania (t. j. vždy, keď používateľ prejde do vyhľadávacieho poľa)

- **entrance_type** – určuje, ako používateľ spustil vyhľadávací dotaz – na karte Hľadať, v dotazoch s nulovými výsledkami, v nadpise vyhľadávania alebo vo výsledkoch vyhľadávania. 

- **has_contact_results** – jednoducho označuje, či sa výsledky kontaktov zobrazujú vo vyhľadávacom dotaze, alebo nie.

- **include_deleted** – označuje, či sa vo výsledkoch vyhľadávania zobrazujú odstránené možnosti 

- **is_ics_external_data** – zachytáva, či je pridaná udalosť interná (t. j. pridaná v Outlooku do Outlook Kalendára), alebo externá (t. j. pridaná z inej e-mailovej aplikácie, ako je napríklad Gmail, do Outlook Kalendára).

- **is_network_fully_connected** – slúži na získanie indikátora dôvodu vyhľadávania v režime offline. Ak je sieť pripojená a vyhľadávanie je v režime offline, dôvodom pravdepodobne bude časový limit servera.

- **is_offline_search** – či je relácia vyhľadávania v režime offline vyhľadávania na základe výsledkov vyhľadávania, ktoré vráti hx.

- **re_enter_search_tab** – Boolovská hodnota na určenie, či používateľ pred výberom výsledku vyhľadávania prepol karty

- **result_selected_type** – s akým typom zobrazených údajov komunikuje používateľ, t. j. zobrazuje všetky kontakty, konverzácie, udalosti atď. 

- **search_conversation_result_data** – obsahuje údaje o konverzácii vybratej z výsledku vyhľadávania vrátane typu konta (hx, ac atď.), či správu uchováva cloudová služba a to, či je zobrazené odsadenie strany rovnaká strana ako prvá správa. 

- **search_origin** – odkiaľ pochádza vyhľadávanie, t. j. hlasový asistent, Cortana, napísané na klávesnici atď. 

- **search_scope** – reťazec, ktorý označuje, aký typ konta hľadal používateľ v službe (napr. Exchange, Gmail atď.) alebo či vyhľadával vo všetkých kontách. 

- **search_suggestion_type** – označuje dôvod návrhu vyhľadávania, napr. či ide o opravu pravopisu. Zakladá sa na histórii? Automatické dokončovanie?

- **search_request_reason** – označuje dôvod odoslania žiadosti o vyhľadávanie v aplikácii; v skutočnosti označí súčasť alebo akciu používateľa, ktorá vyvolala vyhľadávanie.

- **search_result_filter_type** – označuje typ filtra použitého na vyhľadávanie, zobrazí všetko alebo iba prílohy

Zhromažďujú sa tieto polia v aplikáciách systému iOS Outlooku Mobile: 

- **action** – typ akcie, ktorá bola vykonaná na vyhľadávanie. Identifikuje, či sa vyhľadávanie začalo, prebieha alebo skončilo a aké akcie sa počas neho uskutočnili, napr. či bol použitý mikrofón. Pomáha s poskytovaním správnych a užitočných vyhľadávaní.

- **answer_result_selected_count** – sleduje, koľkokrát bolo vyhľadávanie „úspešné“, napr. či používateľ našiel osobu, ktorú hľadal. Napísal e-mail? Založil si správu do záložiek? 

- **contact_result_in_full_list_selected_count** – sleduje počet prípadov, kedy používateľ odoslal žiadosť „Zobraziť všetky kontakty“, keď bol počas kombinovanej relácie vyhľadávania vybratý úplný zoznam

- **contact_result_selected_count** – sleduje, koľko bolo vybraných výsledkov kontaktov počas kombinovanej relácie vyhľadávania

- **conversation_result_selected_count** – sleduje, koľko bolo vybraných konverzácií počas kombinovanej relácie vyhľadávania

- **mail_paging_gesture_count** – sleduje počet gest stránovania vyhľadávania v pošte sa vykonalo v rámci kombinovanej relácie vyhľadávania

- **mail_requests_count** – sleduje počet žiadostí o vyhľadávanie v pošte odoslaných v rámci kombinovanej relácie vyhľadávania

- **people_filter_selected_contacts_count** – sleduje počet vybratých kontaktov vo filtri ľudí

- **search_session_ended_type** – označuje umiestnenie, kde bolo vyhľadávanie ukončené z dôvodu zrušenia alebo aktualizácie dotazu

- **search_suggestion_type** – označuje dôvod návrhu vyhľadávania, napr. či ide o opravu pravopisu. Zakladá sa na histórii? Automatické dokončovanie?

- **see_all_contacts_selected_count** – sleduje, koľkokrát bola počas kombinovanej relácie vyhľadávania vybraná možnosť „Zobraziť všetky kontakty“

- **subtab_type** – sleduje, kde používateľ vybral výsledok z ktorej karty výsledku

- **top_mail_result_selected_count** – sleduje, koľkokrát si používateľ vybral poskytnuté prvé výsledky.

- **ui_reload_result_count** – zaznamenáva časy opätovného načítania používateľského rozhrania z dôvodu aktualizácie množiny výsledkov (počas príslušného dotazu)

- **ui_reload_result_time** – zaznamenáva celkový čas strávený opätovným načítaním používateľského rozhrania z dôvodu aktualizácie množiny výsledkov (počas príslušného dotazu)

- **ui_reload_status_count** – zaznamenáva časy opätovného načítania používateľského rozhrania z dôvodu aktualizácie stavu (počas príslušného dotazu)

- **ui_reload_status_time** – zaznamenáva celkový čas strávený opätovným načítaním používateľského rozhrania z dôvodu aktualizácie stavu (počas príslušného dotazu)

#### <a name="composemailaccessory"></a>compose.mail.accessory

Táto akcia umožňuje zistiť a vyriešiť problémy s kľúčovými akciami písania pošty, aby sa nevyskytol problém s priložením súboru, odfotením fotografie ako prílohy alebo odoslaním vašej dostupnosti.

Zhromažďujú sa tieto polia: 

- **action** – uvádza akciu, ktorej pokus o vykonanie prebehol pri zaznamenaní akcie. Medzi príklady patrí priloženie súboru a zobrazenie ďalších možností.

- **icon_name** – uvádza názov ikony zobrazenej pri zaznamenaní akcie.
 
- **origin** – pôvod akcie. Možné hodnoty sú quick_reply a full_screen.

- **toolbar_type** – označuje typ panela s nástrojmi, ktorý sa nachádza na stránke písania. Možné hodnoty sú compose_actions a formatting.


#### <a name="conversationviewaction"></a>conversation.view.action

Slúži na sledovanie možného nepriaznivého vplyvu na schopnosť zobraziť e-mailové správy a odpovedať na ne

Zhromažďujú sa tieto polia:

- **contains_mention** – uvádza, či bola v konverzácii použitá zmienka @, aby sme mohli zistiť problémy s e-mailovými zmienkami

- **conversation_type** – uvádza, aký typ zobrazenia e-mailovej správy bol vykreslený, napríklad zobrazenie jednej správy alebo zobrazenie viacerých správ. Pomáha zistiť problémy súvisiace s konkrétnym typom správy v zobrazení e-mailovej konverzácie.

- **hx_error_type** – uvádza, aká chyba sa vyskytla, ktorá zabránila službe dokončiť odstránenie, aktualizovať alebo pridať reakciu v správe.

- **hx_string_tag** – uvádza značku chyby v databáze kódov služby

- **reaction_origin** – oznámi nám pôvodné miesto, odkiaľ používateľ reagoval 

- **reaction_type** – oznámi nám typ reakcie používateľa

- **suggested_reply_char_count** – uvádza, koľko znakov mali ponúkané navrhované odpovede (ak sú k dispozícii), aby sme mohli zistiť anomálie a problémy súvisiace s našimi návrhmi

- **suggested_reply_click_pos** – uvádza, kde bola vykreslená navrhovaná odpoveď (ak je k dispozícii), aby sme mohli zistiť problémy s konkrétnym návrhom

- **suggested_reply_type** – označuje typ navrhovanej odpovede pre túto akciu. Možné hodnoty sú text, send_avail a create_meeting.

- **use_default_quick_reply_mode** – uvádza, či bol použitý predvolený režim rýchlej odpovede, aby sme mohli zistiť problémy s rýchlou odpoveďou na e-mail

#### <a name="draftaction"></a>draft.action

Slúži na sledovanie možného nepriaznivého vplyvu na schopnosť vytvárať a ukladať e-mailové koncepty.

Zhromažďujú sa tieto polia: 

- **action** – typ akcie (napríklad uložiť alebo zahodiť).
 
- **draft_message_id** – ID správy konceptu

- **is_groups** – označuje, či sa koncept odosiela do alebo z priečinka skupiny
 
- **origin** – kde bol koncept spustený, napr. detail správy, písanie.

- **smart_compose_model_version** – sleduje, aká verzia modelu inteligentného písania sa používa

- **suggestions_requested** – udáva počet požadovaných návrhov inteligentného písania

- **suggestions_results** – výsledok návrhov inteligentného písania, t. j. prijaté, odmietnuté

- **suggestions_returned** – udáva počet návrhov inteligentného písania vrátených zo servera

- **suggestions_shown** – udáva počet návrhov inteligentného písania zobrazených používateľovi
 
- **thread_id** – ID vlákna konverzácie, ku ktorému je koncept priradený

#### <a name="draganddrop"></a>drag.and.drop

Táto udalosť nám umožňuje zistiť, či akcia presunutia myšou bola úspešná alebo nie.  Používa sa na zabezpečenie správneho fungovania presúvania myšou medzi aplikáciami, a to ako pri pustení myši v Outlooku, ako aj pri ťahaní z Outlooku.  Vďaka týmto údajom dokážeme zabezpečiť, že komplexná spolupráca s inými aplikáciami funguje podľa očakávaní.

Zhromažďujú sa tieto polia: 

- **action** – akcia bude buď ťahanie, alebo pustenie.

- **location**– v prípade akcie ťahania budeme vedieť, odkiaľ používateľ začal presúvať.  V prípade akcie pustenia budeme vedieť, kde používateľ pustil presúvaný súbor. 

- **source** – v prípade akcie presunutia myšou budeme vedieť, odkiaľ používateľ začal presúvať. Pomôže nám to zistiť problémy s presunom z konkrétneho zdroja, ako je napríklad OneDrive alebo súbory, do určitého umiestnenia, napríklad do nového e-mailu.

#### <a name="drawerevent"></a>drawer.event

Slúži na sledovanie možného nepriaznivého vplyvu na možnosť prístupu do priečinkov v doručenej pošte

Zhromažďujú sa tieto polia:

- **add_calendar_option** – označuje typ kalendára, ktorý sa pridá zo zásuvky (t. j. zaujímavý kalendár, kalendár pošty, zdieľaný kalendár), aby sme mohli zistiť problémy s konkrétnymi typmi kalendárov

- **calendar_accounts_count** – označuje počet kont kalendárov, aby sme mohli zistiť problémy s počtom kont, ktoré máte

- **calendar_apps_count** – označuje počet aplikácií kalendára nachádzajúcich sa v zariadení používateľa, aby sme mohli zistiť problémy s aplikáciami kalendára

- **drawer_type** – označuje typ zásuvky (kalendár, e-mailový dotaz alebo dotaz s nulovými výsledkami), aby sme mohli zistiť problémy s typom zásuvky

- **from_favorites** – označuje, či bola akcia prevzatá z obľúbených položiek, aby sme mohli zistiť problémy s obľúbenými položkami

- **group_calendar_count** – označuje počet kalendárov pre konto, aby sme mohli zistiť problémy s kalendármi skupiny

- **inbox_unread_count** – označuje počet neprečítaných správ v priečinku doručenej pošty, aby sme mohli zistiť problémy so zobrazením počtu neprečítaných správ.

- **interesting_calendar_accounts_count** – označuje počet kont, ktoré majú nárok na zaujímavé kalendáre v zariadení, aby sme mohli zistiť problémy so zaujímavými kalendármi

- **is_group_calendar** – označuje, či je kalendár kalendárom skupiny, aby sme mohli zistiť problémy s kalendármi skupiny

- **mail_folder_type** – označuje typ poštového priečinka (t. j. doručená pošta, koncepty atď.), aby sme mohli zistiť problémy s typmi priečinkov.

- **mail_accounts_count** – označuje počet poštových kont, aby sme mohli zistiť problémy s poštovými kontami.

- **selected_group_calendar_count** – označuje počet kalendárov skupín vybratých a aktívnych v používateľskom rozhraní

- **visibility_toggle** – označuje, či používateľ zapol alebo vypol daný kalendár, aby sme mohli zistiť problémy so zobrazením alebo skrytím kalendárov

#### <a name="ipccreaterepublishinglicense"></a>IpcCreateRepublishingLicense

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcCreateRepublishingLicense.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

#### <a name="ipcgetlicenseproperty"></a>IpcGetLicenseProperty

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcGetLicenseProperty.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicensePropertyType** – typ vlastnosti licencie.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

#### <a name="ipcgetserializedlicenseproperty"></a>IpcGetSerializedLicenseProperty

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcGetSerializedLicenseProperty.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicensePropertyType** – typ vlastnosti licencie.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

#### <a name="ipcgettemplateissuerlist"></a>IpcGetTemplateIssuerList

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcGetTemplateIssuerList.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.AuthCallbackProvided** – označuje, či poskytuje spätné volanie overovania ako vstup volania rozhrania API alebo nie.

- **RMS.ConnectionInfo.ExtranetUrl** – extranetová URL adresa informácií o pripojení.

- **RMS.ConnectionInfo.ExtranetUrl** – intranetová URL adresa informácií o pripojení.

- **RMS.ConnectionMode** – režim pripojenia medzi klientom a serverom služby správy prístupových práv: online alebo offline.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.GuestTenant** – ID hosťovského nájomníka pre používateľa.

- **RMS.HomeTenant** – ID domáceho nájomníka pre používateľa.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Identity.ExtranetUrl** – extranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.
 
- **RMS.Identity.IntranetUrl** – intranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.Status** – prvé získanie certifikátu Rights Account Certificate zo servera alebo predĺženie certifikátu Rights Account Certificate. 

- **RMS.Identity.Type** – typ používateľského konta, napríklad konto Windows alebo konto Live.

- **RMS.Identity.UserProvided** – označuje, či e-mailová adresa používateľa bola alebo nebola zadaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.IssuerId** – ID servera služby správy prístupových práv, ktorý vydáva certifikát Rights Account Certificate. 

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.RACType** – typ certifikátu Rights Accounts Certificate.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **UserInfo.UserObjectId** – ID objektu používateľa.

#### <a name="ipcgettemplatelist"></a>IpcGetTemplateList

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcGetTemplateList.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.AuthCallbackProvided** – označuje, či poskytuje spätné volanie overovania ako vstup volania rozhrania API alebo nie.

- **RMS.ConnectionInfo.ExtranetUrl** – extranetová URL adresa informácií o pripojení.

- **RMS.ConnectionInfo.ExtranetUrl** – intranetová URL adresa informácií o pripojení.

- **RMS.ConnectionMode** – režim pripojenia medzi klientom a serverom služby správy prístupových práv: online alebo offline.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.GuestTenant** – ID hosťovského nájomníka pre používateľa.

- **RMS.HomeTenant** – ID domáceho nájomníka pre používateľa.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Identity.ExtranetUrl** – extranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.
 
- **RMS.Identity.IntranetUrl** – intranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.Status** – prvé získanie certifikátu Rights Account Certificate zo servera alebo predĺženie certifikátu Rights Account Certificate. 

- **RMS.Identity.Type** – typ používateľského konta, napríklad konto Windows alebo konto Live.

- **RMS.Identity.UserProvided** – označuje, či e-mailová adresa používateľa bola alebo nebola zadaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.IssuerId** – ID servera služby správy prístupových práv, ktorý vydáva certifikát Rights Account Certificate. 

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.RACType** – typ certifikátu Rights Accounts Certificate.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **RMS.TemplatesCount** – počet šablón.

- **UserInfo.UserObjectId** – ID objektu používateľa.

#### <a name="ipcpcreatelicensefromscratch"></a>IpcpCreateLicenseFromScratch

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcpCreateLicenseFromScratch.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.GuestTenant** – ID hosťovského nájomníka pre používateľa.

- **RMS.HomeTenant** – ID domáceho nájomníka pre používateľa.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Identity.ExtranetUrl** – extranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.IntranetUrl** – intranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.UserProvided** – označuje, či e-mailová adresa používateľa bola alebo nebola zadaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.IssuerId** – ID servera služby správy prístupových práv, ktorý vydáva certifikát Rights Account Certificate. 

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.RACType** – typ certifikátu Rights Accounts Certificate.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **RMS.TokenProvided** – označuje, či poskytuje token ako vstup volania API alebo nie. 

- **RMS.UserProvided** – označuje, či poskytuje používateľa ako vstup volania API alebo nie. 

- **UserInfo.UserObjectId** – ID objektu používateľa. 

#### <a name="ipcpcreatelicensefromtemplate"></a>IpcpCreateLicenseFromTemplate

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcpCreateLicenseFromTemplate. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.AuthCallbackProvided** – označuje, či poskytuje spätné volanie overovania ako vstup volania rozhrania API alebo nie.

- **RMS.ConnectionMode** – režim pripojenia medzi klientom a serverom služby správy prístupových práv: online alebo offline.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **RMS.TokenProvided** – označuje, či poskytuje token ako vstup volania API alebo nie. 

- **RMS.UserProvided** – označuje, či poskytuje používateľa ako vstup volania API alebo nie. 

#### <a name="ipcpgettemplatelistforuser"></a>IpcpGetTemplateListForUser

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcpGetTemplateListForUser. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.AuthCallbackProvided** – označuje, či poskytuje spätné volanie overovania ako vstup volania rozhrania API alebo nie.

- **RMS.ConnectionInfo.ExtranetUrl** – extranetová URL adresa informácií o pripojení.

- **RMS.ConnectionInfo.ExtranetUrl** – intranetová URL adresa informácií o pripojení.

- **RMS.ConnectionMode** – režim pripojenia medzi klientom a serverom služby správy prístupových práv: online alebo offline.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.GuestTenant** – ID hosťovského nájomníka pre používateľa.

- **RMS.HomeTenant** – ID domáceho nájomníka pre používateľa.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Identity.ExtranetUrl** – extranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.IntranetUrl** – intranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.Status** – prvé získanie certifikátu Rights Account Certificate zo servera alebo predĺženie certifikátu Rights Account Certificate. 

- **RMS.Identity.Type** – typ používateľského konta, napríklad konto Windows alebo konto Live.

- **RMS.Identity.UserProvided** – označuje, či e-mailová adresa používateľa bola alebo nebola zadaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.IssuerId** – ID servera služby správy prístupových práv, ktorý vydáva certifikát Rights Account Certificate. 

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.RACType** – typ certifikátu Rights Accounts Certificate.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **RMS.TemplatesCount** – počet šablón.

- **RMS.TokenProvided** – označuje, či poskytuje token ako vstup volania API alebo nie. 
    
- **RMS.UserProvided** – označuje, či poskytuje používateľa ako vstup volania API alebo nie. 

- **UserInfo.UserObjectId** – ID objektu používateľa. 

#### <a name="ipcpserializelicense"></a>IpcpSerializeLicense

Zhromažďuje sa, keď sa používateľ pokúsi použiť ochrany IRM na dokument. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcpSerializeLicense.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.AuthCallbackProvided** – označuje, či poskytuje spätné volanie overovania ako vstup volania rozhrania API alebo nie.

- **RMS.ConnectionMode** – režim pripojenia medzi klientom a serverom služby správy prístupových práv: online alebo offline.

- **RMS.ContentId** – ID obsahu dokumentu.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.GuestTenant** – ID hosťovského nájomníka pre používateľa.

- **RMS.HomeTenant** – ID domáceho nájomníka pre používateľa.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Identity.ExtranetUrl** – extranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.IntranetUrl** – intranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.Status** – prvé získanie certifikátu Rights Account Certificate zo servera alebo predĺženie certifikátu Rights Account Certificate. 

- **RMS.Identity.Type** – typ používateľského konta, napríklad konto Windows alebo konto Live.

- **RMS.Identity.UserProvided** – označuje, či e-mailová adresa používateľa bola alebo nebola zadaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.IssuerId** – ID servera služby správy prístupových práv, ktorý vydáva certifikát Rights Account Certificate. 

- **RMS.KeyHandle** – pamäťová adresa popisovača kľúča.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.PL.KeyType** – hodnoty „Single“ alebo „Double“. Označuje, či PL bolo chránené s ochranou jednoduchým kľúčom alebo ochranou dvojitým kľúčom.

- **RMS.RACType** – typ certifikátu Rights Accounts Certificate.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **RMS.TokenProvided** – označuje, či poskytuje token ako vstup volania API alebo nie. 

- **RMS.UserProvided** – označuje, či poskytuje používateľa ako vstup volania API alebo nie. 

- **UserInfo.UserObjectId** – ID objektu používateľa. 

#### <a name="ipcsetlicenseproperty"></a>IpcSetLicenseProperty

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcSetLicenseProperty. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla. 

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicensePropertyType** – typ vlastnosti licencie.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.StatusCode** – ID scenára definované rozhraním API


#### <a name="linkclickedaction"></a>link.clicked.action

Udalosť sa používa na sledovanie úspešnosti používateľov pri zobrazovaní URL adresy vo webovom zobrazení Edge a dokončovaní štandardných webových scenárov v tomto webovom zobrazení bez chýb

Zhromažďujú sa tieto polia:

- **account_type** – ak bolo webové zobrazenie Edge spustené z e-mailu alebo udalosti v Outlooku, typ konta, z ktorého pochádza URL adresa

- **action** – akcia vykonaná používateľom v Outlooku od chvíle, keď ťukne na URL adresu po opustenie daného toku (otvorí prepojenie vo webovom zobrazení Edge, stránka sa nenačítala vo webovom zobrazení, vykoná vyhľadávanie vo webovom zobrazení, opustí webové zobrazenie Edge s cieľom otvoriť prepojenie v aplikácii webového prehliadača atď.)

- **duration** – trvanie relácie používateľa

- **launch_type** – ak sa spustilo webové zobrazenie Edge, bolo spustené z Outlooku, z miniaplikácie alebo z komponentu operačného systému

- **origin** – ak používateľ vykonal akciu vo webovom zobrazení Edge, uvádza pôvod tejto akcie

- **referrer** – umiestnenie URL adresy, na ktorú používateľ ťukol (e-maily, udalosti v kalendári, karta TXP atď.)

- **search_scope** – ak používateľ vykonal vyhľadávanie vo webovom zobrazení Edge, uvádza rozsah tohto vyhľadávania (všetko, obrázky, videá atď.)

- **search_subtype** – ak používateľ vykonal vyhľadávanie vo webovom zobrazení Edge, uvádza, či šlo o pôvodné alebo presnejšie vyhľadávanie

- **session_summary_page_loaded_count** – počet strán načítaných používateľom počas relácie vo webovom zobrazení Edge

- **session_summary_search_count** – počet vyhľadávaní v Bingu vykonaných používateľom počas relácie vo webovom zobrazení Edge

- **session_summary_session_id** – identifikátor súčasnej relácie používateľa vo webovom zobrazení Edge

- **txp** – ak bolo webové zobrazenie Edge spustené z karty TXP, uvádza typ udalosti pre túto kartu (stolovanie, let atď.)

- **txp_component** – ak bolo webové zobrazenie Edge spustené z karty TXP, uvádza typ komponentu používateľského rozhrania pre túto kartu


#### <a name="mailaction"></a>mail.action

Slúži na sledovanie možného nepriaznivého vplyvu na schopnosť vykonávať dôležité akcie pošty (napríklad spustenie režimu rozdelenia pošty do vlákien) na zaistenie správneho fungovania aplikácie pre poštu.

Zhromažďujú sa tieto polia:

- **account** – konto, v ktorom sa akcia vykonala *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **action** – sleduje vykonaný spôsob akcie, t. j. archivovať, odstrániť, označiť ako prečítané atď. 

- **attachment_content_type** – typ obsahu stiahnutej prílohy 

- **attachment_content_type_with_count** – sledovanie počtu príloh v e-maile

- **attachment_download_result** – výsledok (t. j. úspech/neúspech) pre akciu stiahnutia prílohy

- **attachment_download_time** – čas na akciu stiahnutia prílohy

- **attachment_extn** – prípona súboru stiahnutej prílohy *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **attachment_id** – identifikátor systému pre stiahnutú prílohu 

- **attachment_size** – veľkosť prevzatej prílohy

- **domain** – doména otvoreného dokumentu

- **duration** – sleduje, koľko trvalo zobrazenie akcie ako čitateľného anglického reťazca (napr. 1 s, 4 h)

- **error** – chybové hlásenie priradené k akcii 

- **event_mode** – v akom type režimu udalosti to bolo (skupiny alebo iné). 

- **Extension** – štyri znaky prípony súboru prepojenia alebo prílohy priradenej k tejto akcii *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **internet_message_id** – ID správy sledovania

- **is_group_escalation** – označuje, či sa správa o tom, že sa vykonala akcia, odoslala do poštovej schránky používateľa z dôvodu eskalácie (odber skupiny)

- **is_rule** – označuje, či vykonaná akcia pošty resetuje prioritnú/inú klasifikáciu

- **is_threaded_mode** – označuje, či bola správa v režime rozdelenia do vlákien alebo nie, t. j. ako sa správy zoskupujú

- **is_unread** – označuje, či je správa, pre ktorú sa vykonala akcia, neprečítaná

- **left_swipe_setting** – označuje, ktorá akcia bola nastavená na potiahnutie vľavo

- **message_id** – ID serverovej správy zamerané na akciu alebo zoznam položiek oddelených čiarkami v prípade, že bola v akcii viac ako jedna položka.

- **message_type** – označuje, pre aký typ správy sa vykonala akcia (skupina alebo iný)

- **number_selected** – počet položiek, ktoré používateľ vybral zo zoznamu správ a vykonal v režime viacnásobného výberu.

- **origin** – zdroj akcie, t. j. potiahnutie bunky, dotaz s nulovými výsledkami, priame prepojenie, zobrazenie e-mailu, zoznam e-mailov atď.

- **origin_view** – zdrojové zobrazenie akcie, napríklad konverzácia, správa atď.

- **reported_to_msft** – po odoslaní e-mailu do priečinka nevyžiadanej pošty (nevyžiadaná pošta) alebo do koša (neoprávnené získavanie údajov) možno zvoliť nahlásenie akcie spoločnosti Microsoft.

- **retry** – označuje, či bol zopakovaný pokus o vykonanie akcie

- **right_swipe_setting** – označuje, ktorá akcia bola nastavená na potiahnutie vpravo 

- **Klávesová skratka** – označuje, či sa použila klávesová skratka a aká klávesová skratka sa použila na naplánovanie správy, t. j. neskôr, zajtra, vybrať čas atď.

- **size** – veľkosť prepojenia alebo prílohy priradenej k tejto akcii

- **source_folder** – sleduje typ zdrojového priečinka, keď akcia označuje presun z jedného priečinka do druhého, t. j. do doručenej pošty, koša atď. 

- **source_inbox** – označuje, v ktorom priečinku doručenej pošty prebieha akcia pošty (napríklad prioritné, iné atď.), stav – stav akcie, t. j. úspech alebo bod zlyhania

- **state** – stav akcie, t. j. úspech alebo bod zlyhania

- **target_folder** – označuje typ cieľového priečinka pri presune e-mailov z jedného priečinka do druhého

- **thread_id** – ID vlákna konverzácie zameranej na akciu alebo zoznam položiek oddelených čiarkami v prípade, že bola vybraná viac ako jedna položka

- **time_taken_to_fetch_access_token** – trvanie načítania tokenu prístupu do systému, ktorý sa používa na otvorenie prepojenia

- **time_taken_to_fetch_drive_item** – trvanie načítania prostriedku OneDrivu po kliknutí

- **time_taken_to_fetch_embed_viewer_resource** – trvanie inicializácie vloženého zobrazovača pri otváraní prepojení

- **time_taken_to_load_embed_viewer** – trvanie inicializácie vloženého zobrazovača pri otváraní prepojení

- **time_taken_to_load_link** trvanie dokončenia akcie načítania prepojenia

- **time_taken_to_tap_attachment** – čas medzi otvorením správy a kliknutím na prílohu

- **time_taken_to_tap_link** – trvanie od zobrazenia správy používateľom po kliknutie na prepojenie

- **txp** – označuje, či existuje položka typu txp priradená k pošte, pre ktorú bola vykonaná akcia, t. j. rezervácia udalosti, rezervácia letu atď. 

- **type** – typ dokumentu, ktorý sa otvára cez prepojenie

#### <a name="mailcompose"></a>mail.compose

Slúži na sledovanie možného nepriaznivého vplyvu na schopnosť vytvárať e-maily a odpovedať na ne, ako je napríklad problém s odpovedaním všetkým, formátovaním e-mailov alebo odosielaním e-mailov.

Zhromažďujú sa tieto polia: 

- **draft_message_id** – označuje ID konceptu konverzácie, ktorá sa vytvára ako koncept, aby sme mohli zistiť problémy s konceptami e-mailov

- **message_id** – ID správy konverzácie, na ktorú sa vytvára odpoveď alebo ktorá sa preposiela, aby sme mohli zistiť problémy s konkrétnou správou

- **origin** – uvádza, odkiaľ pochádza vytvorený obsah, napríklad odpovedať všetkým, nová správa alebo rýchla odpoveď. Pomáha zistiť problémy súvisiace s konkrétnym typom pôvodu odpovede.

- **is_group_escalation** – označuje, či je správa eskalovaná skupinová správa, aby sme mohli zistiť problémy s vytváraním týkajúce sa skupín.

- **is_link** – uvádza, či bol nový koncept vytvorený cez prepojenie. Pomáha zistiť problémy súvisiace s konceptmi vytvorenými z prepojení.

- **is_force_touch** – uvádza, či bol nový koncept vytvorený pomocou akcie vynútenia. Pomáha zistiť problémy súvisiace s konceptmi vytvorenými z tejto konkrétnej akcie.

- **is_groups** – označuje, či bola udalosť spustená v priestore skupiny, aby sme mohli zistiť problémy s vytváraním týkajúce sa skupín.

- **source_inbox** – uvádza zdrojovú doručenú poštu, napríklad či ide o prioritnú alebo inú doručenú poštu

- **thread_id** – ID vlákna konverzácie, na ktorú sa vytvára odpoveď alebo ktorá sa preposiela, aby sme mohli zistiť problémy s konkrétnym vláknom

#### <a name="meetingcalltoaction"></a>meeting.call.to.action

Používa sa na sledovanie možného nepriaznivého vplyvu na schopnosť vykonávať dôležité akcie schôdze, ako je vytváranie, úprava a odpovedanie na schôdze.

Zhromažďujú sa tieto polia:

- **event_mode** – označuje, či táto udalosť pochádza zo skupiny alebo nie, aby sme mohli zistiť problémy s udalosťami skupiny

- **meeting_id** – ID schôdze, ktoré pomáha sledovať problémy počas celej životnosti schôdze, aby sme mohli zistiť problémy s konkrétnymi schôdzami

- **meeting_provider** – označuje poskytovateľa online schôdze (napr. Teams alebo Skype for Business), aby sme mohli zistiť problémy s konkrétnymi poskytovateľmi online schôdzí

- **notify_type** – označuje typ odpovede pre iné typy kont, aby sme mohli zistiť problémy s rôznymi typmi kont

- **recurrence** – označuje frekvenciu tejto schôdze, t. j. výskyt alebo rad, aby sme mohli zistiť problémy s opakujúcimi sa radmi schôdzí

- **response** – označuje typ odpovede v niektorých typoch kont, ako je napríklad prijatie alebo odmietnutie, aby sme mohli zistiť problémy s odpovedaním na udalosti

- **response_message_length** – označuje dĺžku správy, aby sme mohli zistiť problémy s odpovedaním na schôdze

- **review_time_proposal_action_type** – označuje odozvu používateľa v prípade návrhu nového termínu, aby sme mohli zistiť problémy s navrhovaním nového termínu

- **send_response** – označuje, či sa odoslala odpoveď, aby sme mohli zistiť problémy s odosielaním odpovedí na pozvánku na schôdzu

- **txp** – označuje, aký typ schôdze sa vygeneroval z rezervácií letov a doručení, aby sme mohli zistiť problémy s týmto typom schôdze

- **with_message_enabled** – označuje, či používateľ môže odpovedať na správu, aby sme mohli zistiť problémy s odpovedaním na pozvánky na schôdzu

#### <a name="officeandroiddocsuifileoperationsopendocumentmeasurements"></a>Office.Android.DocsUI.FileOperations.OpenDocumentMeasurements

Táto udalosť sa zhromažďuje pre aplikácie balíka Office, ktoré sú spustené na platforme Android, a zaznamená, keď sa vykoná operácia otvorenia súboru. Udalosť pomôže pri zachovaní bezpečnosti, aktuálnosti a správneho výkonu operácie otvorenia súboru. Účelom zhromažďovania týchto údajov je neustále zlepšovanie výkonu otvárania súboru. 

Zhromažďujú sa tieto polia:

- **Data_AppDocsOperationDuration** – čas strávený v podvrstve počas operácie otvorenia súboru.

- **Data_AppDuration** – trvanie spracovania aplikácie počas operácie otvorenia súboru. 

- **Data_AppWarmUpGain** – zisk trvania spúšťania aplikácie, ktorý sme dosiahli z dôvodu predbežného spustenia časti aplikácie vopred.

- **Data_BootDuration** – čas trvania spustenia aplikácie pri otváraní súboru.

- **Data_BootMarkers** – hodnota reťazca so zápisom trvania času medzi volaniami niektorých funkcií pri spúšťaní aplikácie vo formáte s ID funkcie a trvaním.

- **Data_ClosePreviouslyOpenedMarkers** – v niektorých scenároch otvárania súborov dôjde pred otvorením aktuálneho dokumentu k zatvoreniu predtým otvoreného dokumentu. Tento čas trvania medzi niektorými operáciami, ktoré prebiehajú v tomto prípade, sa zaznamenáva v reťazci, ktorý má formát \<functionId>\<functionValue>\<functionId>\<functionValue>...

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prípona súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – globálne jedinečný identifikátor (GUID), ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – identifikátor GUID, ktorý jednoznačne označuje identitu použitú na otvorenie súboru. 

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – či bol alebo nebol súbor prednačítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – označuje, či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor Web Application Open Platform Interface Protocol (WOPI) pochádza.

- **Data_ErrorId_Code** – kód chyby indikujúci neúspech operácie zhromažďovania údajov

- **Data_ErrorId_Tag** – značku v kóde, ktorá pomáha s nájdením bodu zlyhania

- **Data_FileOpenFlowMarkers** – pred začatím procesu otvorenia súboru sa vykonáva určité predbežné spracovanie. Tento čas trvania predbežného spracovania sa zaznamenáva v reťazci, ktorý má formát \<functionId>\<functionValue>\<functionId>\<functionValue>...

- **Data_FirstPartyProviderApp** – Ak sa súbor otvorený v aplikáciách Word, Excel, PowerPoint alebo Office použije v inej aplikácii od spoločnosti Microsoft, potom sa tu zaznamená názov tejto aplikácie poskytovateľa.

- **Data_InclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií. 

- **Data_InitializationReason** – enumerácia označujúca spôsob otvorenia súboru, napríklad prvok používateľského rozhrania, spustenie inou aplikáciou atď.

- **Data_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_OfficeMobileInitReason** – enumerácia označujúca vstupný bod otvorenia súboru. 

- **Data_RenderToInSpaceDuration** – Trvanie medzi ukončením vykresľovania a animáciou siluety/plátna.

- **Data_SilhouetteDuration** – trvanie vykresľovania otvorenia súboru.

- **Data_TimeSplitMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie, časovou pečiatkou a trvaním. 

#### <a name="officeandroiddocsuipaywallcontrolpresigninfre"></a>Office.Android.DocsUI.PaywallControl.PreSignInFRE

*[Táto udalosť sa predtým nazývala Office.DocsUI.PaywallControl.PreSignInFRE.]*
 
Toto je dôležitá telemetria používania pre následný predaj pri prvom spustení pre neprihlásených používateľov. Táto udalosť zachytáva metriku prihlásenia pri prvom spustení. Údaje sa použijú na odvodenie prehľadov pre predbežné prihlásenie a získanie informácií o tom, či používateľ pokračuje ďalším štádiom používateľského postupu.
 
Zhromažďujú sa tieto polia: 

- **EventDate** – časová pečiatka výskytu udalosti  

- **FunnelPoint** – enumerátor, ktorý označuje, kde sa používateľ nachádza v tomto kanáli experimentu. Enumerátor uvádza, či používateľ vidí spracovanie a či odíde alebo nie.

- **SessionID** – globálne jedinečný identifikátor na pripojenie udalostí podľa relácie


#### <a name="officeandroiddocsuipaywallcontrolskuchoosertoggled"></a>Office.Android.DocsUI.PaywallControl.SkuChooserToggled

Telemetria používania na zobrazenie, koľkokrát používateľ prepne medzi rôznymi jednotkami SKU ešte pred pokusom o uskutočnenie nákupu. Používa sa na porozumenie používaniu výberu SKU a optimalizáciu funkcie nakupovania v aplikácii v budúcich verziách.

Zhromažďujú sa tieto polia:

- **EventDate** – časová pečiatka výskytu udalosti 

- **SessionID** – identifikátor GUID na pripojenie udalostí podľa relácie


#### <a name="officeandroiddocsuipaywallcontroluserimageclicked"></a>Office.Android.DocsUI.PaywallControl.UserImageClicked 

*[Táto udalosť sa predtým nazývala Office.DocsUI.PaywallControl.UserImageClicked.]*
 
Táto udalosť meria telemetriu, aby sa zistilo, či sa používatelia pokúšajú dokončiť akciu kliknutím na avatar používateľa. Tieto údaje sa použijú na meranie počtu používateľov v interakcii s ikonou avatara na vyhodnotenie potreby prostredia sledovania po ťuknutí.
 
Zhromažďujú sa tieto polia: 

- **EventDate** – časová pečiatka výskytu udalosti  

- **SessionID** – globálne jedinečný identifikátor na pripojenie udalostí podľa relácie 


#### <a name="officeandroidearlytelemetryexpansionfilesavailability"></a>Office.Android.EarlyTelemetry.ExpansionFilesAvailability

Povoľujeme rozširujúce súbory súpravy Android Package Kit (APK) pre mobilnú aplikáciu Office. Rozširujúce súbory APK sú doplnkové zdrojové súbory, ktoré môžu vývojári aplikácií pre Android publikovať spolu so svojou aplikáciou. Na porozumenie spoľahlivosti rozširujúcich súborov zaznamenávame príznak označujúci, či sú rozširujúce súbory k dispozícii pri každom spustení alebo nie.

Zhromažďujú sa tieto polia:

- **Data_ExpansionFilesAvailable** – Boolovský príznak, ktorý označuje, či rozširujúce súbory APK sú k dispozícii v zariadení v čase spúšťania aplikácie.

#### <a name="officeandroidearlytelemetryexpansionfilesdownloader"></a>Office.Android.EarlyTelemetry.ExpansionFilesDownloader

Povoľujeme rozširujúce súbory súpravy Android Package Kit (APK) pre mobilnú aplikáciu Office. Rozširujúce súbory APK sú doplnkové zdrojové súbory, ktoré môžu vývojári aplikácií pre Android publikovať spolu so svojou aplikáciou.  Na porozumenie spoľahlivosti mechanizmu sťahovania rozširujúcich súborov zaznamenávame príznak označujúci, či rozširujúce súbory dokážeme úspešne stiahnuť.

Zhromažďujú sa tieto polia: 

- **Data_DownloadSuccess** – Boolovský príznak, ktorý označuje, či stiahnutie rozširujúcich súborov APK bolo úspešné, vždy, keď sa pokúsime o stiahnutie počas spúšťania aplikácie.

#### <a name="officeandroidearlytelemetrynotecreated"></a>Office.Android.EarlyTelemetry.NoteCreated

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov Rýchlych poznámok vytvárať poznámky v aplikácii. Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu vytvoriť poznámku, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **IsExportable** – príznak označujúci, či táto udalosť bola výsledkom akcie používateľa alebo nie. Mala by byť nastavená na hodnotu True, pretože NoteCreated je akcia spustená používateľom.

- **NoteLocalId** – rozlíšiteľný jedinečný identifikátor priradený poznámke, keď používateľ vytvorí poznámku v rámci aplikácii.

- **StickyNotes-SDKVersion** – číslo verzie označujúce verziu aplikácie Rýchle poznámky, ktorú používateľ používa. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby sa správne určila jeho priorita.


#### <a name="officeandroidearlytelemetrynoteviewed"></a>Office.Android.EarlyTelemetry.NoteViewed 

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov Rýchlych poznámok zobrazovať poznámky v aplikácii. Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu zobraziť svoje poznámky, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **HasImages** – príznak označujúci, či zobrazená poznámka obsahuje poznámku.

- **IsExportable** – príznak označujúci, či táto udalosť bola výsledkom akcie používateľa alebo nie. Mala by byť nastavená na hodnotu True, pretože NoteViewed je akcia spustená používateľom.

- **NoteLocalId** – rozlíšiteľný jedinečný identifikátor priradený poznámke, keď používateľ vytvorí poznámku v rámci aplikácii.

- **StickyNotes-SDKVersion** – číslo verzie označujúce verziu aplikácie Rýchle poznámky, ktorú používateľ používa. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby sa správne určila jeho priorita.


#### <a name="officeandroidintuneintunecompliancerequest"></a>Office.Android.Intune.IntuneComplianceRequest

Táto udalosť sa zhromažďuje pre aplikácie balíka Office, ktoré sú spustené na platforme Android vrátane mobilného balíka Office, Wordu, Excelu, PowerPointu a OneNotu. Udalosť označuje pokus o prihlásenie do konta organizácie s licenciou Intune, v ktorom správca organizácie nakonfiguroval politiku vynútenia podmieneného prístupu k aplikácii. Používa sa na zistenie počtu koncových používateľov, ktorí sa pokúšajú používať aplikácie s touto konfiguráciou politiky, a v kombinácii s inou udalosťou Office.Android.Intune.IntuneComplianceStatus na zaistenie vynútenia nakonfigurovanej politiky. 

Nezhromažďujú sa žiadne údajové polia.

#### <a name="officeandroidintuneintunecompliancestatus"></a>Office.Android.Intune.IntuneComplianceStatus

Táto udalosť sa zhromažďuje pre aplikácie balíka Office, ktoré sú spustené na platforme Android vrátane mobilného balíka Office, Wordu, Excelu, PowerPointu a OneNotu. Udalosť označuje pokus o prihlásenie do konta organizácie s licenciou Intune, v ktorom správca organizácie nakonfiguroval politiku vynútenia podmieneného prístupu k aplikácii. Táto udalosť označuje dodržiavanie súladu v aplikácii, v ktorej je používateľ prihlásený, a používa sa na skúmanie zlyhaní. Je skombinovaná s inou udalosťou Office.Android.Intune.IntuneComplianceRequest na zaistenie vynútenia nakonfigurovanej politiky.
  
Zhromažďujú sa tieto polia:

- **Data_ComplianceStatus** – označuje stav dodržiavania súladu aplikácie počas prihlásenia s kódom chyby úspechu alebo neúspechu.
  - -1 – Neznáma chyba
  -    0 – Aplikácia je v súlade s politikami organizácie
  - 1 – Aplikácia nie je v súlade s politikami organizácie
  - 2 – Zlyhania súvisiace so službou
  - 3 – Zlyhania súvisiace so sieťou
  - 4 – Aplikácii sa nepodarilo načítať overovací token 
  - 5 – Odpoveď ešte nebola prijatá zo služby
  - 6 – Aplikácia Company Portal musí byť nainštalovaná

#### <a name="officeandroidodwxpssotelemetry"></a>Office.Android.ODWXPSSO.Telemetry

Táto udalosť pomáha porozumieť, s akou inou aplikáciou Microsoft v zariadení naša aplikácia získala bezobslužné jediné prihlásenie, z ktorého vstupného bodu a tak ďalej. Pomáha tiež pochopiť príčinu zlyhania s nezískaním bezobslužného jediného prihlásenia.  Získame lepší prehľad napríklad o tom, s ktorou aplikáciou Microsoft v zariadení získavame jediné prihlásenie. Ide o neúspešné prípady, keď jednoduché prihlásenie nefunguje podľa očakávaní.

Zhromažďujú sa tieto polia:

- **AccountType** – označuje typ konta, s ktorým sa vyskytuje jediné prihlásenie, ako je napríklad osobné konto Microsoft alebo pracovné konto.

- **EntryPoint** – označuje vstupný bod v aplikácii, odkiaľ sa jediné prihlásenie spustilo.

- **ErrorCode** – označuje kód chyby pokusu o jediné prihlásenie.

- **ErrorDescription** – označuje chybové hlásenie pokusu o jediné prihlásenie.

- **HResult** – označuje kód stavu výsledku pokusu o jediné prihlásenie.

- **ProviderPackageId** – iná aplikácia Microsoft v zariadení, z ktorej dochádza k jedinému prihláseniu.

#### <a name="officeandroidphonenumbersignins"></a>Office.Android.PhoneNumberSignIns

Táto udalosť pomôže porozumieť, či sa používateľ prihlásil alebo zaregistroval s kontom založeným na telefónnom čísle alebo s e-mailovým osobným kontom Microsoft.  Táto udalosť pomáha zistiť počet používateľov, ktorí sa prihlasujú alebo registrujú s osobným kontom Microsoft založeným na telefónnom čísle.

Zhromažďujú sa tieto polia:

- **EntryPoint** – označuje vstupný bod v aplikácii, odkiaľ sa prihlásenie spustilo.

- **IsEmailMissing** – chýba e-mail v informáciách o profile konta?

- **IsPhoneNumberMissing** – chýba telefónne číslo v informáciách o profile konta?

- **UserDecision** – označuje používateľom vykonaný výber, ako je napríklad prihlásenie alebo registrácia, alebo prihlásenie neskôr.

#### <a name="officeandroidusersignindecision"></a>Office.Android.UserSignInDecision

Táto udalosť pomáha porozumieť, v ktorej fáze postupu používateľovi zlyháva prihlasovanie, prečo sa nedarí prihlásiť sa, koľko používateľov sa úspešne prihlásilo z ktorého vstupného bodu v aplikácii a podobne.  Táto udalosť pomôže s prihlasovacími liekovými údajmi, čo pomáha porozumieť, v ktorých fázach prihlásenie zlyháva u viacerých používateľov a podobne.

Zhromažďujú sa tieto polia:

- **AccountType** – označuje typ konta, s ktorým sa pokúšate prihlásiť, ako je napríklad osobné konto alebo pracovné konto.

- **AfterLicensingState** – označuje stav licencií aplikácií po dokončení prihlásenia.

- **AllowedEditsWithoutSignIn** – označuje, koľko voľných úprav uplynulo pred pokusom o prihlásenie.

- **BeforeLicensingState** – označuje stav licencií aplikácií pred pokusom o prihlásenie.

- **CompletionState** – označuje fázu dokončenia prihlásenia.

- **EntryPoint** – označuje vstupný bod v aplikácii, odkiaľ sa prihlásenie spustilo.

- **HRDAutoAcceleratedSignUpAttemptCount** – označuje počet pokusov o zrýchlenú registráciu.

- **HRDAutoAcceleratedSignUpQuitCount** – označuje počet zrušení zrýchlenej registrácie.

- **HResult** – označuje kód stavu výsledku operácie prihlásenia.

- **IsPhoneOnlyAuthFeatureEnabled** – je povolené prihlasovanie s telefónnym číslom alebo nie?

- **LicenseActivationHResult** – označuje kód stavu pokusu o aktiváciu licencie.

- **LicenseActivationMessageCode** – označuje kód správy z licenčnej služby.

- **NoFreeEditsTreatmentValue** – sú povolené voľné úpravy alebo nie?

- **SignUpAttemptCount** – označuje počet pokusov o registráciu.

- **StartMode** – označuje režim, v ktorom sa spustil pokus o prihlásenie.

- **UserDecision** – označuje používateľom vykonaný výber, ako je napríklad prihlásenie alebo registrácia, alebo prihlásenie neskôr.


#### <a name="officeappcompatappcompatagentscanandupload"></a>Office.AppCompat.AppCompat.AgentScanAndUpload

Zhromažďuje sa len vtedy, ak koncový používateľ povolil tabuľu telemetrie balíka Office. Zhromažďuje informácie o tom, kedy sa spustil agent telemetrie balíka Office.    Tieto údaje sa zhromažďujú len vtedy, ak je tabuľa telemetrie balíka Office povolená a používa sa na určenie stavu agenta telemetrie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data.AgentExit** – časová pečiatka toho, keď je agent telemetrie úspešne ukončený

  - **Data.AgentScan** – časová pečiatka toho, keď agent telemetrie úspešne dokončil sken

  - **Data.AgentUpload** – časová pečiatka toho, keď agent telemetrie úspešne dokončil nahratie

#### <a name="officeappcompatappcompatagentupload"></a>Office.AppCompat.AppCompat.AgentUpload

Generuje sa pri spustení klienta, ak koncový používateľ povolil tabuľu telemetrie balíka Office.  Zhromažďuje informácie o tom, kedy agent telemetrie balíka Office nahral údaje do priečinka na zdieľanie. Primárnym využítím tejto udalosti je monitorovanie stavu agenta telemetrie balíka Office a jej druhotným využitím je odhad používania tabule telemetrie balíka Office.

Zhromažďujú sa tieto polia:

- **UploadTime** – časová pečiatka posledného úspešného nahrávania vykonaného agentom telemetrie.


#### <a name="officeappcompatappcompattelemetrydashboardresiliencycrashlog"></a>Office.AppCompat.AppCompat.TelemetryDashboardResiliencyCrashLog

Zhromažďuje sa len vtedy, ak koncový používateľ (s najväčšou pravdepodobnosťou správca) povolil tabuľu telemetrie balíka Office. Zhromažďuje informácie o výskyte zlyhaní doplnkov a dokumentov balíka Office.  Tieto údaje sa zhromažďujú len vtedy, ak používateľ povolil tabuľu telemetrie balíka Office a používa sa na určenie toho, či dochádza k zvýšenému výskytu zlyhaní doplnkov alebo dokumentov.

Zhromažďujú sa tieto polia:

  - **Data.CollectionTime** – časová pečiatka toho, kedy sa zaznamenala udalosť zlyhania.

#### <a name="officeappdocsappdocsdocumentoperation"></a>Office.AppDocs.AppDocs.DocumentOperation

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v platformách Android, iOS, Universal alebo Windows. Udalosť zaznamená, keď sa vykoná operácia súboru z URL adresy (vytvorenie/otvorenie/uloženie/export/atď.), a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách súborov.

Zhromažďujú sa tieto polia:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikácie, ak nie je známa pred ukončením klásenia vyvolaného na operácii.

- **Data_CanContinueFromOnBeforeOperationBegins** – Stav CanContinue (môže pokračovať) pred vyvolaním popisovača začiatku.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prvé štyri znaky prípony súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – označuje, či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – označuje, či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – označuje, či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – označuje, či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – označuje, či súbor bol alebo nebol vopred načítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – označuje, či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_DocumentInputCurrency** – typ vstupu dokumentu, ktorý používa operácia.

- **Data_DocumentOperation_AppId** – hodnota enumerácie predstavujúca ID aplikácie.

- **Data_DocumentOperation_EndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_DocumentOperation_EndReason** – hodnota enumerácie predstavujúca dôvod ukončenia.

- **Data_DocumentOperation_IsReinitialized** – označuje, sa znova inicializuje dokument, ktorý je už otvorený.

- **Data_DocumentOperation_isTargetECBeginEC** – označuje, či je cieľový kontext spustenia rovnaký ako kontext, z ktorého sa dokument otvára.

- **Data_DocumentOperation_ParamsFlags** – príznaky enumerácie používané na spustenie operácie.

- **Data_DocumentOperation_TelemetryReason** – vyjadrenie enumerácie vstupného bodu pre udalosť otvorenia. Príklad: otvorenie zo zoznamu naposledy otváraných súborov alebo prehľadávania, aktivácia súborov atď.

- **Data_FileIOInclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_FileIO_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_InitializationReason** – vyjadrenie enumerácie konkrétneho dôvodu operácie. Napr. otvorenie z URL adresy alebo lokálnej cesty k súboru, vytvorenie pomocou výberu súboru, kopírovanie do cesty k súboru, exportovanie na URL adresu atď.

- **Data_IsDisambiguateCsiNetworkConnectivityErrorEnabled**.

- **Data_IsNameMissingInUrl** – označuje, či sa názov neanalyzoval z URL adresy.

- **Data_IsPathMissingForLocalFile** – označuje, či ide o lokálny súbor bez cesty.

- **Data_IsUnpackedLinkSupportedForOpen** – označuje, či je nezbalené prepojenie podporované pre otvorenie.

- **Data_LinksOpenRightScenario** – hodnota enumerácie pre scenár otvárania prepojení doprava.

- **Data_OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_OperationType** – vyjadrenie enumerácie generického typu operácie. Napr. vytvorenie, otvorenie, kopírovanie, uloženie atď.

- **Data_RelatedPrevOpTelemetryReason** – označuje, či sa operácia týka predchádzajúcej operácie.

- **Data_StopwatchDuration** – celkový čas aktivity.

- **Data_UnpackLinkHint** – enumerácia predstavujúca potenciálnu akciu používateľa na základe prepojenia rozbalenia.

- **Data_UnpackLinkPromptResult** – enumerácia predstavujúca odpoveď na výzvu na prepojenie rozbalenia.

#### <a name="officeappleactivateperpetual"></a>Office.Apple.ActivatePerpetual

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu aktivácie trvalej licencie a skúmanie príčin zlyhaní prostredníctvom revízie hodnôt FailedAt.

Zhromažďujú sa tieto polia:

- **Data_FailedAt** – zhromažďujeme reťazec označujúci, kde v postupe aktivovania trvalej licencie došlo k chybe.

#### <a name="officeappleactivatesubscription"></a>Office.Apple.ActivateSubscription

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Zhromažďujeme informácie súvisiace s migráciou zo zásobníka starších kódov licencií s kódmi licencií vNext. Táto funkcia sa používa na monitorovanie stavu postupu aktivácie predplatného, ako aj na sledovanie, ak ide o migráciu na licencie vNext a ak sa použila primárna identita.

Zhromažďujú sa tieto polia:

- **Data_ActivatingPrimaryIdentity** – Hodnota true alebo false, ktorá označuje, či bola použitá primárna identita. 

- **Data_NULSubscriptionLicensed** – Hodnota true alebo false, ktorá označuje stav predplatného.

#### <a name="officeapplecisauthticketwithidentity"></a>Office.Apple.CISAuthTicketWithIdentity

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zachytávanie zlyhaní generovania tokenov overovania počas nákupu v aplikácii v Macu (udalosť zaznamenáva prijatý kód chyby).  Táto udalosť sa používa na zisťovanie a pomoc pri riešení problémov so zlyhaniami generovania tokenov overovania

Zhromažďujú sa tieto polia:

- **Data_EmptyAuthToken** – zhromažďujeme reťazec označujúci, kde v postupe aktivovania trvalej licencie došlo k chybe.

- **Data_TicketAuthError** – kód chyby označujúci príčinu zlyhania

- **Data_ValidIdentity** – či má klient platnú identitu

#### <a name="officeappleinappassociationactivity"></a>Office.Apple.InAppAssociationActivity

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Zhromažďujeme informácie súvisiace s priradením produktu po zakúpení v rámci aplikácie. Zaznamenáme, ktorú jednotku SKU predplatného priraďujeme.  Používa sa to na monitorovanie stavu priradení produktov zakúpených v rámci aplikácie.

Zhromažďujú sa tieto polia:

- **Data_ProductID** – Jednotka SKU predplatného, ku ktorej sa snažíme priradiť produkt.

#### <a name="officeappleinapppurchaseactivity"></a>Office.Apple.InAppPurchaseActivity

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. 

Zhromažďujeme informácie súvisiace s nákupmi produktov v AppStore. Sledujeme výsledok nákupu (neúspešný, úspešný, problému s platbou atď.), typ žiadosti o nákup (obnovenie, nákup) a nakupovanú jednotku SKU/produkt (Microsoft 365 Family atď.).  Tieto údaje sa používajú na monitorovanie stavu postupov nákupu v rámci aplikácie.

Zhromažďujú sa tieto polia:

- **Data_ Data_PurchaseResult** – Výsledok operácie nákupu.

- **Data_ProductID** – Nakupovaný produkt.

- **Data_PurchaseRequestType** – Typ žiadosti o nákup.

#### <a name="officeappleintune"></a>Office.Apple.InTune

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Zhromažďujeme informácie o tom, či je aktuálna relácia spravovaná službou Intune. Táto možnosť sa používa na kontingenčné ovládanie/filtrovanie relácií spravovaných službou Intune a umožňuje nám skúmať potenciálne problémy súvisiace s balíkom Office pri spustení aplikácie spravovanej službou Intune.

Zhromažďujú sa tieto polia:

- **Data_EventID** – Zhromažďujeme reťazec predstavujúci kód, ktorý určuje, či je relácia spravovaná službou Intune.

#### <a name="officeapplelicensingmaclicensingstate"></a>Office.Apple.Licensing.Mac.LicensingState

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zachytáva aktuálny stav licencie na reláciu v zariadení (ID licencie OLS, použité jednotky SKU, s dobou odkladu alebo bez nej, RFM atď.). Zhromaždené údaje sa používajú na zisťovanie chýb a skúmanie príčin zlyhaní. 

Zhromažďujú sa tieto polia:

- **Data_DidRunPreview** – Reťazec, ktorý označuje, či sa táto relácia spustí v ukážke.

- **Data_LicensingACID** – Reťazec predstavujúci interný identifikátor systému licencií.

- **Data_LicensingType** – Reťazec, ktorý predstavuje typ licencie.

- **Data_OLSLicenseId** – Reťazec, ktorý predstavuje identifikátor licencie.

- **Data_State** – Reťazec, ktorý predstavuje aktuálny stav licencie.

#### <a name="officeconnectdeviceactivitystart"></a>Office.ConnectDevice.Activity.Start

Umožňuje zistiť, či pripojenie k zariadeniu alebo aplikácii bolo úspešné.  Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „ConnectDevice“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – spustenie

- **Activity_DateTimeTicks** – dátum a čas aktivity
 
#### <a name="officeconnectdeviceactivitystop"></a>Office.ConnectDevice.Activity.Stop

Umožňuje zistiť, či pripojenie k zariadeniu alebo aplikácii bolo úspešné. Umožňuje sledovanie stavu a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „ConnectDevice“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – zastavenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officedocsappdocsoperationopenfrommrubypath"></a>Office.Docs.AppDocs.OperationOpenFromMruByPath

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v platformách Android, iOS, Universal alebo Windows. Udalosť zaznamenáva, keď sa vykoná operácia otvorenia súboru z cesty v zozname naposledy použitých súborov a používa sa na pochopenie a stanovenie priorít chýb používateľských skúseností na základe informácií o operáciách otvorenia súborov.

Zhromažďujú sa tieto polia:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikácie, ak nie je známa pred ukončením klásenia vyvolaného na operácii.

- **Data_CanContinueFromOnBeforeOperationBegins** – Stav CanContinue (môže pokračovať) pred vyvolaním popisovača začiatku.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prvé štyri znaky prípony súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – označuje, či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – označuje, či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – označuje, či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – označuje, či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – označuje, či súbor bol alebo nebol vopred načítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – označuje, či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_DocumentInputCurrency** – typ vstupu dokumentu, ktorý používa operácia.

- **Data_DocumentOperation_AppId** – hodnota enumerácie predstavujúca ID aplikácie.

- **Data_DocumentOperation_EndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_DocumentOperation_EndReason** – hodnota enumerácie predstavujúca dôvod ukončenia.

- **Data_DocumentOperation_IsReinitialized** – označuje, sa znova inicializuje dokument, ktorý je už otvorený.

- **Data_DocumentOperation_ParamsFlags** – príznaky enumerácie používané na spustenie operácie.

- **Data_DocumentOperation_TelemetryReason** – vyjadrenie enumerácie vstupného bodu pre udalosť otvorenia. Príklad: otvorenie zo zoznamu naposledy otváraných súborov alebo prehľadávania, aktivácia súborov atď.

- **Data_DocumentOperation_isTargetECBeginEC** – označuje, či je cieľový kontext spustenia rovnaký ako kontext, z ktorého sa dokument otvára.

- **Data_FileIOInclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_FileIO_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_IsNameMissingInUrl** – označuje, či sa názov neanalyzoval z URL adresy.

- **Data_IsPathMissingForLocalFile** – označuje, či ide o lokálny súbor bez cesty.

- **Data_IsUnpackedLinkSupportedForOpen** – označuje, či je nezbalené prepojenie podporované pre otvorenie.

- **Data_LinksOpenRightScenario** – hodnota enumerácie pre scenár otvárania prepojení doprava.

- **Data_OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_RelatedPrevOpTelemetryReason** – označuje, či sa operácia týka predchádzajúcej operácie.

- **Data_StopwatchDuration** – celkový čas aktivity.

- **Data_UnpackLinkHint** – enumerácia predstavujúca potenciálnu akciu používateľa na základe prepojenia rozbalenia.

- **Data_UnpackLinkPromptResult** – enumerácia predstavujúca odpoveď na výzvu na prepojenie rozbalenia.

#### <a name="officedocsappdocsoperationopenfrommrubyurl"></a>Office.Docs.AppDocs.OperationOpenFromMruByUrl

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v platformách Android, iOS, Universal alebo Windows. Udalosť zaznamenáva, keď sa vykoná operácia otvorenia súboru z URL adresy v zozname naposledy použitých súborov a používa sa na pochopenie a stanovenie priorít používateľských skúseností na základe informácií o operáciách otvorenia súborov. 

Zhromažďujú sa tieto polia:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikácie, ak nie je známa pred ukončením klásenia vyvolaného na operácii.

- **Data_CanContinueFromOnBeforeOperationBegins** – Stav CanContinue (môže pokračovať) pred vyvolaním popisovača začiatku.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prvé štyri znaky prípony súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – označuje, či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – označuje, či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – označuje, či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – označuje, či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – označuje, či súbor bol alebo nebol vopred načítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – označuje, či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_DocumentInputCurrency** – typ vstupu dokumentu, ktorý používa operácia.

- **Data_DocumentOperation_AppId** – hodnota enumerácie predstavujúca ID aplikácie.

- **Data_DocumentOperation_EndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_DocumentOperation_EndReason** – hodnota enumerácie predstavujúca dôvod ukončenia.

- **Data_DocumentOperation_IsReinitialized** – označuje, sa znova inicializuje dokument, ktorý je už otvorený.

- **Data_DocumentOperation_ParamsFlags** – príznaky enumerácie používané na spustenie operácie.

- **Data_DocumentOperation_TelemetryReason** – vyjadrenie enumerácie vstupného bodu pre udalosť otvorenia. Príklad: otvorenie zo zoznamu naposledy otváraných súborov alebo prehľadávania, aktivácia súborov atď.

- **Data_DocumentOperation_isTargetECBeginEC** – označuje, či je cieľový kontext spustenia rovnaký ako kontext, z ktorého sa dokument otvára.

- **Data_FileIOInclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_FileIO_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_IsNameMissingInUrl** – označuje, či sa názov neanalyzoval z URL adresy.

- **Data_IsPathMissingForLocalFile** – označuje, či ide o lokálny súbor bez cesty.

- **Data_IsUnpackedLinkSupportedForOpen** – označuje, či je nezbalené prepojenie podporované pre otvorenie.

- **Data_LinksOpenRightScenario** – hodnota enumerácie pre scenár otvárania prepojení doprava.

- **Data_OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_RelatedPrevOpTelemetryReason** – označuje, či sa operácia týka predchádzajúcej operácie.

- **Data_StopwatchDuration** – celkový čas aktivity.

- **Data_UnpackLinkHint** – enumerácia predstavujúca potenciálnu akciu používateľa na základe prepojenia rozbalenia.

- **Data_UnpackLinkPromptResult** – enumerácia predstavujúca odpoveď na výzvu na prepojenie rozbalenia.


#### <a name="officedocsappdocsoperationopenfrompath"></a>Office.Docs.AppDocs.OperationOpenFromPath

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v platformách Android, iOS, Universal alebo Windows. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru z cesty a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov.

Zhromažďujú sa tieto polia:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikácie, ak nie je známa pred ukončením klásenia vyvolaného na operácii.

- **Data_CanContinueFromOnBeforeOperationBegins** – Stav CanContinue (môže pokračovať) pred vyvolaním popisovača začiatku.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prvé štyri znaky prípony súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – označuje, či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – označuje, či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – označuje, či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – označuje, či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – označuje, či súbor bol alebo nebol vopred načítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – označuje, či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_DocumentInputCurrency** – typ vstupu dokumentu, ktorý používa operácia.

- **Data_DocumentOperation_AppId** – hodnota enumerácie predstavujúca ID aplikácie.

- **Data_DocumentOperation_EndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_DocumentOperation_EndReason** – hodnota enumerácie predstavujúca dôvod ukončenia.

- **Data_DocumentOperation_IsReinitialized** – označuje, sa znova inicializuje dokument, ktorý je už otvorený.

- **Data_DocumentOperation_ParamsFlags** – príznaky enumerácie používané na spustenie operácie.

- **Data_DocumentOperation_TelemetryReason** – vyjadrenie enumerácie vstupného bodu pre udalosť otvorenia. Príklad: otvorenie zo zoznamu naposledy otváraných súborov alebo prehľadávania, aktivácia súborov atď.

- **Data_DocumentOperation_isTargetECBeginEC** – označuje, či je cieľový kontext spustenia rovnaký ako kontext, z ktorého sa dokument otvára.

- **Data_FileIOInclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_FileIO_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_IsNameMissingInUrl** – označuje, či sa názov neanalyzoval z URL adresy.

- **Data_IsPathMissingForLocalFile** – označuje, či ide o lokálny súbor bez cesty.

- **Data_IsUnpackedLinkSupportedForOpen** – označuje, či je nezbalené prepojenie podporované pre otvorenie.

- **Data_LinksOpenRightScenario** – hodnota enumerácie pre scenár otvárania prepojení doprava.

- **Data_OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_RelatedPrevOpTelemetryReason** – označuje, či sa operácia týka predchádzajúcej operácie.

- **Data_StopwatchDuration** – celkový čas aktivity.

- **Data_UnpackLinkHint** – enumerácia predstavujúca potenciálnu akciu používateľa na základe prepojenia rozbalenia.

- **Data_UnpackLinkPromptResult** – enumerácia predstavujúca odpoveď na výzvu na prepojenie rozbalenia.

#### <a name="officedocsappdocsoperationopenfromprotocolhandler"></a>Office.Docs.AppDocs.OperationOpenFromProtocolHandler

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v platformách Android, iOS, Universal alebo Windows. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru z inej aplikácie pomocou rozhrania popisovača protokolu a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov.

Zhromažďujú sa tieto polia:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikácie, ak nie je známa pred ukončením klásenia vyvolaného na operácii.

- **Data_CanContinueFromOnBeforeOperationBegins** – Stav CanContinue (môže pokračovať) pred vyvolaním popisovača začiatku.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prvé štyri znaky prípony súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – označuje, či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – označuje, či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – označuje, či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – označuje, či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – označuje, či súbor bol alebo nebol vopred načítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – označuje, či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_DocumentInputCurrency** – typ vstupu dokumentu, ktorý používa operácia.

- **Data_DocumentOperation_AppId** – hodnota enumerácie predstavujúca ID aplikácie.

- **Data_DocumentOperation_EndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_DocumentOperation_EndReason** – hodnota enumerácie predstavujúca dôvod ukončenia.

- **Data_DocumentOperation_IsReinitialized** – označuje, sa znova inicializuje dokument, ktorý je už otvorený.

- **Data_DocumentOperation_ParamsFlags** – príznaky enumerácie používané na spustenie operácie.

- **Data_DocumentOperation_TelemetryReason** – vyjadrenie enumerácie vstupného bodu pre udalosť otvorenia. Príklad: otvorenie zo zoznamu naposledy otváraných súborov alebo prehľadávania, aktivácia súborov atď.

- **Data_DocumentOperation_isTargetECBeginEC** – označuje, či je cieľový kontext spustenia rovnaký ako kontext, z ktorého sa dokument otvára.

- **Data_FileIOInclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_FileIO_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_IsNameMissingInUrl** – označuje, či sa názov neanalyzoval z URL adresy.

- **Data_IsPathMissingForLocalFile** – označuje, či ide o lokálny súbor bez cesty.

- **Data_IsUnpackedLinkSupportedForOpen** – označuje, či je nezbalené prepojenie podporované pre otvorenie.

- **Data_LinksOpenRightScenario** – hodnota enumerácie pre scenár otvárania prepojení doprava.

- **Data_OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_RelatedPrevOpTelemetryReason** – označuje, či sa operácia týka predchádzajúcej operácie.

- **Data_StopwatchDuration** – celkový čas aktivity.

- **Data_UnpackLinkHint** – enumerácia predstavujúca potenciálnu akciu používateľa na základe prepojenia rozbalenia.

- **Data_UnpackLinkPromptResult** – enumerácia predstavujúca odpoveď na výzvu na prepojenie rozbalenia.

#### <a name="officedocsappdocsoperationopenfromshell"></a>Office.Docs.AppDocs.OperationOpenFromShell

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v platformách Android, iOS, Universal alebo Windows. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru z prostredia (shell) a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov.

Zhromažďujú sa tieto polia:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikácie, ak nie je známa pred ukončením klásenia vyvolaného na operácii.

- **Data_CanContinueFromOnBeforeOperationBegins** – Stav CanContinue (môže pokračovať) pred vyvolaním popisovača začiatku.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prvé štyri znaky prípony súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – označuje, či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – označuje, či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – označuje, či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – označuje, či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – označuje, či súbor bol alebo nebol vopred načítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – označuje, či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_DocumentInputCurrency** – typ vstupu dokumentu, ktorý používa operácia.

- **Data_DocumentOperation_AppId** – hodnota enumerácie predstavujúca ID aplikácie.

- **Data_DocumentOperation_EndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_DocumentOperation_EndReason** – hodnota enumerácie predstavujúca dôvod ukončenia.

- **Data_DocumentOperation_IsReinitialized** – označuje, sa znova inicializuje dokument, ktorý je už otvorený.

- **Data_DocumentOperation_ParamsFlags** – príznaky enumerácie používané na spustenie operácie.

- **Data_DocumentOperation_TelemetryReason** – vyjadrenie enumerácie vstupného bodu pre udalosť otvorenia. Príklad: otvorenie zo zoznamu naposledy otváraných súborov alebo prehľadávania, aktivácia súborov atď.

- **Data_DocumentOperation_isTargetECBeginEC** – označuje, či je cieľový kontext spustenia rovnaký ako kontext, z ktorého sa dokument otvára.

- **Data_FileIOInclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_FileIO_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_IsNameMissingInUrl** – označuje, či sa názov neanalyzoval z URL adresy.

- **Data_IsPathMissingForLocalFile** – označuje, či ide o lokálny súbor bez cesty.

- **Data_IsUnpackedLinkSupportedForOpen** – označuje, či je nezbalené prepojenie podporované pre otvorenie.

- **Data_LinksOpenRightScenario** – hodnota enumerácie pre scenár otvárania prepojení doprava.

- **Data_OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_RelatedPrevOpTelemetryReason** – označuje, či sa operácia týka predchádzajúcej operácie.

- **Data_StopwatchDuration** – celkový čas aktivity.

- **Data_UnpackLinkHint** – enumerácia predstavujúca potenciálnu akciu používateľa na základe prepojenia rozbalenia.

- **Data_UnpackLinkPromptResult** – enumerácia predstavujúca odpoveď na výzvu na prepojenie rozbalenia.


#### <a name="officedocsappdocsoperationopenfromurl"></a>Office.Docs.AppDocs.OperationOpenFromUrl

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v platformách Android, iOS, Universal alebo Windows. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru z URL adresy a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov.

Zhromažďujú sa tieto polia:

- **Data_AppIdForReportEndBeforeAppKnown** – ID aplikácie, ak nie je známa pred ukončením klásenia vyvolaného na operácii.

- **Data_CanContinueFromOnBeforeOperationBegins** – Stav CanContinue (môže pokračovať) pred vyvolaním popisovača začiatku.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prvé štyri znaky prípony súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – označuje, či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – označuje, či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – označuje, či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – označuje, či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – označuje, či súbor bol alebo nebol vopred načítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – označuje, či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_DocumentInputCurrency** – typ vstupu dokumentu, ktorý používa operácia.

- **Data_DocumentOperation_AppId** – hodnota enumerácie predstavujúca ID aplikácie.

- **Data_DocumentOperation_EndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_DocumentOperation_EndReason** – hodnota enumerácie predstavujúca dôvod ukončenia.

- **Data_DocumentOperation_IsReinitialized** – označuje, sa znova inicializuje dokument, ktorý je už otvorený.

- **Data_DocumentOperation_ParamsFlags** – príznaky enumerácie používané na spustenie operácie.

- **Data_DocumentOperation_TelemetryReason** – vyjadrenie enumerácie vstupného bodu pre udalosť otvorenia. Príklad: otvorenie zo zoznamu naposledy otváraných súborov alebo prehľadávania, aktivácia súborov atď.

- **Data_DocumentOperation_isTargetECBeginEC** – označuje, či je cieľový kontext spustenia rovnaký ako kontext, z ktorého sa dokument otvára.

- **Data_FileIOInclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_FileIO_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_IsNameMissingInUrl** – označuje, či sa názov neanalyzoval z URL adresy.

- **Data_IsPathMissingForLocalFile** – označuje, či ide o lokálny súbor bez cesty.

- **Data_IsUnpackedLinkSupportedForOpen** – označuje, či je nezbalené prepojenie podporované pre otvorenie.

- **Data_LinksOpenRightScenario** – hodnota enumerácie pre scenár otvárania prepojení doprava.

- **Data_OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia ukončila.

- **Data_RelatedPrevOpTelemetryReason** – označuje, či sa operácia týka predchádzajúcej operácie.

- **Data_StopwatchDuration** – celkový čas aktivity.

- **Data_UnpackLinkHint** – enumerácia predstavujúca potenciálnu akciu používateľa na základe prepojenia rozbalenia.

- **Data_UnpackLinkPromptResult** – enumerácia predstavujúca odpoveď na výzvu na prepojenie rozbalenia.



#### <a name="officedocsappledocsuxiossaveasthroughfilemenu"></a>Office.Docs.Apple.DocsUXiOSSaveAsThroughFileMenu 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa vykoná operácia „Uložiť ako“, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách súborov, ako sú napríklad kategórie umiestnenia.  Operácia „Uložiť ako“ sa vyskytne vždy, keď používateľ vytvorí nový súbor a uloží ho prvýkrát alebo uloží kópiu existujúceho súboru do nového umiestnenia.

Zhromažďujú sa tieto polia:

- **Data_OriginServiceType** – Abstraktná kategorizácia pôvodného umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_ServiceType** – Abstraktná kategorizácia nového umiestnenia súboru po dokončení uloženia, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

#### <a name="officedocsappledocsuxmacatmentioninsertedatmention"></a>Office.Docs.Apple.DocsUXMacAtMentionInsertedAtMention 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď sa používateľ „@“zmieni o inom používateľovi, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe toho, ako používatelia spolupracujú s ostatnými používateľmi.

Zhromažďujú sa tieto polia:

- **Data_CharactersTyped** – Číselná hodnota, ktorá udáva celkový počet znakov zadaných v texte „@“zmienky.

#### <a name="officedocsappledocsuxmacodspsharingwebviewsharingcompleted"></a>Office.Docs.Apple.DocsUXMacODSPSharingWebViewSharingCompleted 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď sa používateľ rozhodne zdieľať dokument v cloude pomocou zdieľania vo OneDrive, a používa sa na lepšie pochopenie a uprednostňovanie používateľských skúseností na základe zdieľania dokumentov.

Zhromažďujú sa tieto polia:

- **Data_ShareType** – Naprogramovaný reťazec, ktorý označuje, aký druh operácie zdieľania bol dokončený, vrátane operácií „Kopírovať prepojenie“, „Ďalšie aplikácie“, „Teams“.

- **Data_ShareWebViewMode** – Naprogramovaný reťazec, ktorý označuje, aký druh režimu zdieľania bol aktívny v čase dokončenia zdieľania, vrátane režimov „ManageAccess“, „AtMentions“, „Share“.

#### <a name="officedocsuicollaborationcoauthorgalleryrowtapped"></a>Office.DocsUI.Collaboration.CoauthorGalleryRowTapped 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď používateľ vyberie možnosť pozrieť si zoznam aktuálnych spoluautorov.  Tieto údaje sa používajú na lepšie pochopenie a uprednostňovanie používateľských skúseností súvisiacich so spolutvorbou dokumentu v rovnakom čase.

Zhromažďujú sa tieto polia:

- **Data_CoauthorCount** – Číselná hodnota, ktorá predstavuje celkový počet ľudí, ktorí práve upravujú ten istý dokument ako používateľ.

#### <a name="officedocsuicollaborationcollabcornerpeoplegallerycoauthorsupdated"></a>Office.DocsUI.Collaboration.CollabCornerPeopleGalleryCoauthorsUpdated 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa zmení počet aktívnych spoluautorov v dokumente v cloude.  Tieto údaje sa používajú na lepšie pochopenie a uprednostňovanie používateľských skúseností súvisiacich so spolutvorbou dokumentu v rovnakom čase.

Zhromažďujú sa tieto polia:

- **Data_CoauthorsJoined** – Počet spoluautorov, ktorí sa pripojili k dokumentu.

- **Data_CoauthorsLeft** – Počet spoluautorov, ktorí opustili dokument.

- **Data_NewCoauthorCount** – Nový počet aktívnych spoluautorov v dokumente. 

- **Data_OldCoauthorCount** – Predchádzajúci počet aktívnych spoluautorov pred aktualizáciou.

- **Data_ServiceType** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

#### <a name="officedocsuidocstagedocstagecreatenewfromtemplate"></a>Office.DocsUI.DocStage.DocStageCreateNewFromTemplate 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa vytvorí nový súbor pomocou položky „Nové zo šablóny“, a používa sa na lepšie pochopenie a uprednostňovanie používateľských skúseností na základe informácií o vytváraní dokumentu.

Zhromažďujú sa tieto polia:

- **Data_InHomeTab** – Boolovská hodnota, ktorá označuje, či bol nový súbor zo šablóny vytvorený z karty Domov v novom prostredí súboru.

- **Data_InSearch** – Boolovská hodnota, ktorá označuje, či bol súbor vytvorený, keď používateľ hľadal šablónu.

- **Data_IsHomeTabEnabled** – Boolovská hodnota, ktorá označuje, či je karta Domov momentálne dostupná pre používateľa.

- **Data_IsRecommendedEnabled** – Boolovská hodnota, ktorá označuje, či je funkcia „Odporúčané“ momentálne dostupná pre používateľa.

- **Data_TemplateIndex** – Číselný index súboru šablóny, ako sa vizuálne zobrazuje používateľovi.

- **Data_TemplateType** – Klasifikácia na odlíšenie typu šablóny, ako sú, okrem iných, napríklad šablóny „Online“, „Online vyhľadávanie“, „Lokálne“.

#### <a name="officedocsuidocstagerecommendedopen"></a>Office.DocsUI.DocStage.RecommendedOpen

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru v časti odporúčaných súborov v galérii dokumentov, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov.

Zhromažďujú sa tieto polia:

- **Data_Success** – Boolovská hodnota, ktorá označuje, či sa operácia vykonala úspešne.

#### <a name="officedocsuifileoperationsdocsuifileopenmacrequired"></a>Office.DocsUI.FileOperations.DocsUIFileOpenMacRequired

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov, ako sú napríklad kategórie umiestnenia „ServiceType“ a prvé štyri znaky prípony.

Zhromažďujú sa tieto polia:

- **Data_Ext** – Prípona súboru obmedzená na prvé štyri znaky prípony alebo menej.

- **Data_ServiceType** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď.

#### <a name="officedocsuifileoperationsopendocumentmeasurements"></a>Office.DocsUI.FileOperations.OpenDocumentMeasurements

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platformy iOS. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov, najmä informácií o výkone.

Zhromažďujú sa tieto polia:

- **Data_AppDuration** – trvanie spracovania aplikácie počas operácie otvorenia súboru.

- **Data_BootDuration** – trvanie procesu spustenia otvorenia súboru.

- **Data_ClickOrigin** – reťazec označujúci, z ktorej časti bolo prepojenie, keď používateľ klikol na prepojenie v Outlooku pre iOS a otvoril súbor v aplikácii balíka Office.

- **Data_ClickTime** – čas Unix Epoch, keď používateľ klikol na prepojenie v Outlooku pre iOS a otvoril súbor v aplikácii balíka Office.

- **Data_ClosePreviouslyOpenedMarkers** – hodnota reťazca so zápisom trvania času medzi volaniami niektorých funkcií vo formáte s ID funkcie a trvaním.

- **Data_DetachedDuration** – trvanie procesu odpojenia udalosti. 

- **Data_Doc_AccessMode** – enumerácia označujúca režim prístupu k súboru, napríklad iba na čítanie, na čítanie a zapisovanie.

- **Data_Doc_AsyncOpenKind** – enumerácia označujúca typ asynchrónneho procesu použitého na otvorenie súboru.

- **Data_Doc_ChunkingType** – enumerácia označujúca typ algoritmu blokov údajov súboru.

- **Data_Doc_EdpState** – enumerácia označujúca stav ochrany podnikových údajov súboru.

- **Data_Doc_Ext** – prípona súboru.

- **Data_Doc_Fqdn** – názov hostiteľa servera súboru.

- **Data_Doc_FqdnHash** – identifikátor GUID, ktorý jednoznačne označuje názov hostiteľa servera.

- **Data_Doc_IdentityTelemetryId** – identifikátor GUID, ktorý jednoznačne označuje identitu použitú na otvorenie súboru.

- **Data_Doc_InitializationScenario** – enumerácia označujúca podrobný typ scenára otvorenia súboru.

- **Data_Doc_IOFlags** – enumerácia označujúca príznaky IO operácie otvorenia súboru, napríklad či je súbor uložený vo vyrovnávacej pamäti alebo nie.

- **Data_Doc_IsCloudCollabEnabled** – či je alebo nie je pre súbor zapnutá spolupráca v cloude.

- **Data_Doc_IsIncrementalOpen** – či sa súbor otvoril alebo neotvoril cez prírastkové otvorenie.

- **Data_Doc_IsOcsSupported** – či súbor podporuje alebo nepodporuje službu spolupráce v Office.

- **Data_Doc_IsOpeningOfflineCopy** – či sa súbor otvoril z offline kópie z vyrovnávacej pamäte.

- **Data_Doc_IsPrefetched** – či bol alebo nebol súbor prednačítaný pred výskytom operácie otvorenia.

- **Data_Doc_IsSyncBacked** – či sa cloudový súbor vyskytuje lokálne a synchronizuje so serverom alebo nie.

- **Data_Doc_Location** – enumerácia označujúca umiestnenie súboru, napríklad lokálne alebo v cloude.

- **Data_Doc_ReadOnlyReasons** – enumerácia označujúca dôvod, prečo je súbor iba na čítanie.

- **Data_Doc_ResourceIdHash** – identifikátor GUID, ktorý jednoznačne označuje ID zdroja servera súboru.

- **Data_Doc_RtcType** – enumerácia označujúca typ kanála v reálnom čase (RTC) použitého súborom.

- **Data_Doc_ServerDocId** – identifikátor GUID, ktorý jednoznačne označuje ID dokumentu na serveri.

- **Data_Doc_ServerProtocol** – enumerácia označujúca serverový protokol cloudového súboru.

- **Data_Doc_ServerType** – enumerácia označujúca serverový typ cloudového súboru.

- **Data_Doc_ServerVersion** – enumerácia označujúca serverovú verziu cloudového súboru.

- **Data_Doc_SessionId** – celé číslo, ktoré sa zvýši o 1 pri každej operácii otvorenia súboru v relácii.

- **Data_Doc_SharePointServiceContext** – reťazec, ktorý sa používa na koreláciu denníkov na strane klienta a na strane servera, zvyčajne ide o druh ID.

- **Data_Doc_SizeInBytes** – veľkosť súboru v bajtoch.

- **Data_Doc_SpecialChars** – enumerácia, ktorá označuje, aký typ špeciálneho znaku obsahuje URL adresa súboru.

- **Data_Doc_UrlHash** – identifikátor GUID, ktorý jednoznačne označuje URL adresu súboru.

- **Data_Doc_UsedWrsDataOnOpen** – či bol alebo nebol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti.

- **Data_Doc_WopiServiceId** – reťazec, ktorý označuje, z ktorej služby súbor WOPI (Web Application Open Platform Interface Protocol) pochádza.

- **Data_HWModel** – hodnota reťazca, ktorá do denníka zapisuje model zariadenia iPad alebo iPhone.

- **Data_InclusiveMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré zahŕňa trvanie volania podradených funkcií.

- **Data_InitializationReason** – enumerácia označujúca spôsob otvorenia súboru, napríklad z ktorého prvku používateľského rozhrania alebo spustenie inou aplikáciou.

- **Data_IsDocumentAlreadyOpen** – či už je súbor otvorený, aleb nie.

- **Data_IsInterrupted** – či bola operácia otvorenia súboru prerušená prechodom aplikácie na pozasie.

- **Data_Measurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie a trvaním, ktoré nezahŕňa trvanie volania podradených funkcií.

- **Data_OpenInPlace** – či sa súbor musí alebo nemusí kopírovať do izolovaného kontajnera balíka Office pred jeho otvorením používateľom.

- **Data_OpenStartTime** – čas Unix Epoch, keď sa spustilo otvorenie súboru.

- **Data_SilhouetteDuration** – trvanie vykresľovania otvorenia súboru.

- **Data_SourceApplication** – reťazec, ktorý označuje ID zväzku zdrojovej aplikácie, keď bolo otvorenie súboru spustené inou aplikáciou.

- **Data_StopwatchDuration** – trvanie od začiatku udalosti po koniec udalosti.

- **Data_TimeSplitMeasurements** – hodnota reťazca so zápisom trvania času potrebného na volanie niektorých funkcií vo formáte so značkou funkcie, časovou pečiatkou a trvaním.

#### <a name="officedocsuifileoperationsopenfilewithreason"></a>Office.DocsUI.FileOperations.OpenFileWithReason 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa vykoná operácia otvorenia súboru, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov, ako sú napríklad kategórie umiestnenia „ServiceType“ a z ktorého miesta v aplikácii používateľ žiadal o otvorenie súboru.

Zhromažďujú sa tieto polia:

- **Data_IsCandidateDropboxFile** – Boolovská hodnota, ktorá sa zapíše do denníka v prípade, že na základe kontroly cesty k súboru sa domnievame, že by mohol byť z priečinka, ktorý synchronizuje DropBox.

- **Data_IsSignedIn** – Či je používateľ prihlásený, keď sa súbor uloží.

- **Data_OpenReason** – Dôvod otvorenia je číselná hodnota, ktorá označuje, v ktorej časti aplikácie používateľ otvoril súbor.

- **Data_ServiceType** – Abstraktná číselná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

#### <a name="officedocsuifileoperationssavetourl"></a>Office.DocsUI.FileOperations.SaveToURL

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa vykoná operácia „Uložiť ako“ a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách otvorenia súborov, ako sú napríklad kategórie umiestnenia a prvé štyri znaky prípony.  Operácia „Uložiť ako“ sa vyskytne vždy, keď používateľ vytvorí nový súbor a uloží ho prvýkrát alebo uloží kópiu existujúceho súboru do nového umiestnenia.

Zhromažďujú sa tieto polia:

- **Data_FileExtension** – Prvé štyri znaky prípony nového súboru.

- **Data_IsNewFileCreation** – Označuje, či ide o operáciu uloženia nového súboru alebo kópie existujúceho súboru.

- **Data_IsSignedIn** – Či je používateľ prihlásený, keď sa súbor uloží.

- **Data_SaveErrorCode** – Číselná hodnota, ktorá sa nastaví, ak sa vyskytne chyba, a pomôže určiť druh chyby.

- **Data_SaveErrorDomain** – Určuje doménu SaveErrorCode, ako ju definuje Apple, SaveErrorDomains „sú ľubovoľné reťazce, ktoré sa používajú na odlíšenie skupín kódov“.

- **Data_SaveLocation** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_SaveOperationType** – Číselná hodnota definovaná skupinou hodnôt NSSaveOperationType spoločnosti Apple.


#### <a name="officedocsuisharinguicloudupsellshown"></a>Office.DocsUI.SharingUI.CloudUpsellShown 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď používateľ prejde prechodom dokumentu do postupu v cloude.  Tieto údaje sa používajú na lepšie pochopenie a uprednostňovanie používateľských skúseností súvisiacich s presúvaním dokumentov do cloudových umiestnení.

Zhromažďujú sa tieto polia:

- **Data_FileStyle** – Číselná hodnota, ktorá označuje, v akom scenári sa zobrazila možnosť prechodu, ako napríklad prepnutím na automatické ukladanie alebo tlačidlom na zdieľanie.

- **Data_FileType** – Prvé štyri znaky prípony aktuálneho súboru.

- **Data_InDocStage** – Boolovská hodnota, ktorá označuje, či sa možnosť prechodu zobrazuje v galérii dokumentov alebo v rámci okna dokumentu.

- **Data_IsDocumentOpened** – Boolovská hodnota, ktorá označuje, či je otvorený aj aktuálny dokument, pre ktorý sa zobrazuje možnosť prechodu.

- **Data_IsDraft** – Boolovská hodnota, ktorá označuje, či už bol aktuálny súbor niekedy uložený.

- **Data_IsSheetModal** – Boolovská hodnota, ktorá označuje, či bola možnosť prechodu uvedená modálne alebo nie.

#### <a name="officedocsuisharinguicloudupsellupload"></a>Office.DocsUI.SharingUI.CloudUpsellUpload 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď sa používateľ rozhodne nahrať nový alebo lokálny súbor do cloudu, a výsledok tejto operácie.  Tieto údaje sa používajú na lepšie pochopenie a uprednostňovanie používateľských skúseností súvisiacich s presúvaním dokumentov do cloudových umiestnení.

Zhromažďujú sa tieto polia:

- **Data_FileStyle** – Číselná hodnota, ktorá označuje, v akom scenári sa zobrazila možnosť prechodu, ako napríklad prepnutím na automatické ukladanie alebo tlačidlom na zdieľanie.

- **Data_FileType** – Prvé štyri znaky prípony aktuálneho súboru.

- **Data_InDocStage** – Boolovská hodnota, ktorá označuje, či sa možnosť prechodu zobrazuje v galérii dokumentov alebo v rámci okna dokumentu.

- **Data_IsDefaultServiceLocation** – Boolovská hodnota, ktorá označuje, či vybraté umiestnenie, do ktorého sa má dokument nahrať, je predvolené umiestnenie.

- **Data_IsDocumentOpened** – Boolovská hodnota, ktorá označuje, či je otvorený aj aktuálny dokument, pre ktorý sa zobrazuje možnosť prechodu.

- **Data_IsDraft** – Boolovská hodnota, ktorá označuje, či už bol aktuálny súbor niekedy uložený.

- **Data_IsSheetModal** – Boolovská hodnota, ktorá označuje, či bola možnosť prechodu uvedená modálne alebo nie.

- **Data_LocationServiceType** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_UploadAction** – Naprogramovaný reťazec, ktorý určuje, či išlo o operáciu nahrávania premiestnením alebo kopírovaním.

- **Data_UploadResult** – Naprogramovaný reťazec, ktorý označuje výsledok pokusu o nahratie vrátane hodnôt „Success“ „UserCancelledUpload“ a „PreAuthFailed“.

#### <a name="officedocsuisharinguicopylinkoperation"></a>Office.DocsUI.SharingUI.CopyLinkOperation

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď sa používateľ rozhodne zdieľať dokument generovaním prepojenia na dokument v cloude, a používa sa na lepšie pochopenie a uprednostňovanie používateľských skúseností na základe zdieľania dokumentov.

Zhromažďujú sa tieto polia:

- **Data_ServiceType** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_LinkType** – Naprogramovaný reťazec, ktorý popisuje druh vykonanej operácie pozvania, ako je „ViewOnly“ a „ViewAndEdit“.

- **Data_ShareScenario** – Naprogramovaný reťazec, ktorý popisuje, kde v rámci používateľského rozhrania aplikácie sa súbor zdieľa vrátane umiestnení „FileMenu“, „OpenTabShareActionMenu“, „RecentTabShareActionMenu“.

#### <a name="officedocsuisharinguidocsuionedriveshare"></a>Office.DocsUI.SharingUI.DocsUIOneDriveShare 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď sa používateľ rozhodne zdieľať dokument v cloude pomocou zdieľania vo OneDrive, a používa sa na lepšie pochopenie a uprednostňovanie používateľských skúseností na základe zdieľania dokumentov.

Zhromažďujú sa tieto polia:

- **Data_ODSPShareWebviewShareError** – Ak sa pri zdieľaní vyskytne chyba, toto je číselná hodnota, ktorá pomôže určiť dôvod zlyhania.

- **Data_ODSPShareWebviewShareGrantAccessResult** – Boolovská hodnota, ktorá ak je true, tak označuje, že sa úspešne dokončila jednoduchá operácia zdieľania.

- **Data_ODSPShareWebviewShareSuccessType** – Keď sa úspešne dokončí operácia zdieľania, toto je číselná hodnota, ktorá sa používa na určenie toho, aký druh operácie zdieľania sa dokončil.

- **Data_WebViewInfoResult** – Ak sa používateľské rozhranie nepodarí úspešne načítať, toto je číselná hodnota, ktorá pomôže určiť dôvod zlyhania. 

- **Data_WebViewLoadTimeInMs** – Číselná hodnota, ktorá zaznamenáva množstvo času potrebného na načítanie webového používateľského rozhrania.

#### <a name="officedocsuisharinguiinvitepeople"></a>Office.DocsUI.SharingUI.InvitePeople 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď sa používateľ rozhodne pozvať ľudí do dokumentu v cloude, a používa sa na lepšie pochopenie a uprednostňovanie používateľských skúseností na základe zdieľania dokumentov.

Zhromažďujú sa tieto polia:

- **Data_ServiceType** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_InviteeCount** – Celkový počet kontaktov pozvaných do dokumentu v rámci jednej akcie pozvania.

- **Data_LinkType** – Naprogramovaný reťazec, ktorý popisuje druh vykonanej operácie pozvania, ako je „ViewOnly“ a „ViewAndEdit“.

- **Data_MessageLength** – Číselná hodnota celkového počtu znakov odoslaných v správe pozvánky.

- **Data_ShareScenario** – Naprogramovaný reťazec, ktorý popisuje, kde v rámci používateľského rozhrania aplikácie sa súbor zdieľa vrátane umiestnení „FileMenu“, „OpenTabShareActionMenu“, „RecentTabShareActionMenu“.

#### <a name="officedocsuisharinguisendacopyoperation"></a>Office.DocsUI.SharingUI.SendACopyOperation

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zaznamená, keď sa používateľ rozhodne odoslať kópiu dokumentu, a používa sa na lepšie pochopenie a uprednostňovanie používateľských skúseností na základe zdieľania dokumentov.

Zhromažďujú sa tieto polia:

- **Data_IsHomeTabEnabled** – Boolovská hodnota, ktorá označuje, či je karta Domov momentálne dostupná pre používateľa.

- **Data_IsRecommendedEnabled** – Boolovská hodnota, ktorá označuje, či je funkcia „Odporúčané“ momentálne dostupná pre používateľa.

- **Data_OperationType** – Číselná hodnota, ktorá označuje, aký druh operácie odosielania kópie prebieha, ako je odoslanie kópie e-mailom alebo odoslanie kópie prostredníctvom ovládacieho prvku zdieľania od spoločnosti Apple.

- **Data_ServiceType** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_ShareFileType** – Naprogramovaný reťazec, ktorý popisuje, aký typ objektu sa zdieľa vrátane objektov „Document“, „PDF“, „Picture“.

- **Data_ShareScenario** – Naprogramovaný reťazec, ktorý popisuje, kde v rámci používateľského rozhrania aplikácie sa súbor zdieľa vrátane umiestnení „FileMenu“, „OpenTabShareActionMenu“, „RecentTabShareActionMenu“.

- **Data_SharingService** – Boolovská hodnota, ktorá označuje, či bol súbor vytvorený, keď používateľ hľadal šablónu.

#### <a name="officedocsuisharinguiupsellshare"></a>Office.DocsUI.SharingUI.UpsellShare 

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť zaznamená, keď používateľ prejde prechodom dokumentu do postupu v cloude pri pokuse o zdieľanie dokumentu.  Tieto údaje sa používajú na lepšie pochopenie a uprednostňovanie používateľských skúseností súvisiacich s presúvaním dokumentov do cloudových umiestnení.

Zhromažďujú sa tieto polia:

- **Data_FileOperationResult** – Číselná hodnota, ktorá označuje, či sa operácia vykonala úspešne.

- **Data_HostedFromDocStage** – Boolovská hodnota, ktorá označuje, či používateľ prechádza prechodom do postupu v cloude z prostredia DocStage alebo z otvoreného dokumentu.

- **Data_isLocalCopyOn** – Boolovská hodnota, ktorá označuje, či sa používateľ rozhodol ponechať lokálnu kópiu dokumentu, ktorý sa nahráva do umiestnenia v cloude, alebo premiestniť do cloudového umiestnenia existujúci dokument.

- **Data_NewFileType** – Abstraktná kategorizácia umiestnenia nového umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_OriginalFileType** – Abstraktná kategorizácia umiestnenia súboru, ako je napríklad „SharePoint“, „OneDrive“, „Lokálne“, „WOPI“ atď., a výslovne nie skutočného umiestnenia súboru.

- **Data_UploadButtonPressed** – Boolovská hodnota, ktorá označuje, či sa používateľ rozhodol nahrať aktuálny dokument do cloudového umiestnenia.

- **Data_UploadError** – Číselná hodnota, ktorá označuje druh chyby, ktorá sa vyskytla v prípade zlyhania operácie nahrávania.

- **Data_UpsellAppearsFromDelegate** – Boolovská hodnota, ktorá označuje, či sa zobrazenie zobrazilo z ponuky zdieľania.

#### <a name="officeextensibilitycatalogexchangeprocessentitlement"></a>Office.Extensibility.Catalog.ExchangeProcessEntitlement

Údaje o spracovaní individuálneho nároku na doplnok priradený správcom nájomníka služieb Office 365.

Používajú sa pri vytváraní grafov (požadovaných manažmentom tímu) úspešnosti zákazníkov a analýzy problémov zákazníkov.

Zhromažďujú sa tieto polia:

  - **AppVersion** – verzia hosťujúcej aplikácie doplnku.

  - **SolutionId** – identifikátor GUID predstavujúci jedinečný doplnok

  - **TelemetryId** – identifikátor GUID predstavujúci jedinečného používateľa

#### <a name="officeextensibilitycatalogexchangeprocessmanifest"></a>Office.Extensibility.Catalog.ExchangeProcessManifest

Údaje o spracovaní individuálneho manifestu doplnku priradeného správcom nájomníka služieb Office 365. Používa sa na analýzu problémov zákazníkov a vytváranie grafov úspešnosti zákazníka.
 
Zhromažďujú sa tieto polia:

- **AppVersion** – verzia aplikácie

- **IsAllReturnedManifestsParsed** – logická hodnota označujúca, že sme analyzovali všetky vrátené manifesty

- **IsAppCommand** – logická hodnota označujúca, či ide o príkaz aplikácie 

- **ReturnedManifestsParsed** – počet analyzovaných manifestov

- **SolutionId** – ID riešenia

- **TelemetryId** – ID telemetrie na základe prihlásenej identity

#### <a name="officeextensibilityodpappcommandsribbonclick"></a>Office.Extensibility.ODPAppCommandsRibbonClick

Zhromažďuje informácie o tom, či kliknutie na vlastný ovládacví prvok doplnku bolo úspešné alebo nie. Používa sa na zisťovanie problémov v interakcii používateľa s ovládacími prvkami doplnku.
 
Zhromažďujú sa tieto polia:

- **CommandActionType** – typ príkazu doplnku

- **CommandLabel** – označenie príkazu, na ktorý sa kliklo

- **SolutionId** – ID riešenia

#### <a name="officefeedeventsinitializing"></a>Office.Feed.Events.Initializing

Údaje o tejto udalosti sa zhromažďujú pri inicializácii informačného kanála. Táto udalosť sa používa na označenie toho, že informačný kanál sa spúšťa, a diagnostiku problémov so spoľahlivosťou pri spustení informačného kanála.

- **AppInfo.Language** – jazyk aplikácie vo formáte značiek jazyka skupiny IETF.

- **AppInfo.Name** – názov používanej súčasti (informačný kanál balíka Office).

- **AppInfo.Version** – verzia aplikácie.

- **clientCorrelationId** – globálne jedinečný identifikátor relácie aplikácie

- **clientType** – aplikácia, v ktorej súčasť spustená.

- **DeviceInfo.Make** – názov výrobcu zariadenia alebo výrobcu OEM zariadenia.

- **DeviceInfo.NetworkProvider** – sieť alebo mobilný operátor, ako je napríklad AT&T.

- **DeviceInfo.NetworkType** – typ sieťových pripojení zariadenia, ako je napríklad káblové, Wi-Fi alebo WWAN (dátové/mobilné).

- **DeviceInfo.OsName** – názov operačného systému zariadenia.

- **DeviceInfo_SDKUid** – jednoznačne identifikuje zariadenie z perspektívy SDK telemetrie.

- **eventId** –identifikátor názvu udalosti. 

- **EventInfo.SdkVersion** – verzia SDK telemetrie, ktorú klient použil na generovanie udalosti.

- **eventpriority** – hodnota enumerácie priority odoslania udalosti.

- **feature** – používa sa na zoskupovanie rôznych udalostí tej istej funkcie.

- **hostAppRing** – populácia používateľov, ktorým sa aplikácia distribuovala.

- **properties** – obsahuje dodatočné metaúdaje alebo vlastnosti zhromaždené pre každú udalosť.
        
    - **ClientTimeStamp** – časová pečiatka zaznamenania udalosti v klientovi.

- **publicEventName** – názov udalosti pre verejnosť.  

- **region** – geografická oblasť služby informačných kanálov, ku ktorej je používateľ pripojený. 

- **tenantAadObjectId** – globálne jedinečný identifikátor pre podnikového nájomníka používateľa.

- **type** – typ zaznamenanej udalosti, napr. sledovanie, chyba, udalosť, QoS.

- **userAadObjectId** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft.

- **UserInfo.Id** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft.

- **UserInfo.IdType** – určuje typ ID používateľa. 

- **UserInfo.Language** – jazyk používateľa vo formáte značiek jazyka skupiny IETF.

- **UserInfo.MsaId** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **UserInfo.TimeZone** – časové pásmo používateľa vzťahujúce sa na čas UTC.

- **userPuid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **version** – verzia klienta informačného kanála.

#### <a name="officefeedeventsofficefeeddidappear"></a>Office.Feed.Events.OfficeFeedDidAppear

Údaje o tejto udalosti sa zhromažďujú pri zobrazení informačného používateľovi. Táto udalosť sa používa na overenie toho, či informačný kanál dokončil krok spúšťania, a diagnostiku problémov so spoľahlivosťou pri spustení informačného kanála.

- **AppInfo.Language** – jazyk aplikácie vo formáte značiek jazyka skupiny IETF.

- **AppInfo.Name** – názov používanej súčasti (informačný kanál balíka Office).

- **AppInfo.Version** – verzia aplikácie.

- **bridgeWaitingTime** – metrika na diagnostiku výkonu pri vykresľovaní informačného kanála.

- **clientCorrelationId** – globálne jedinečný identifikátor relácie aplikácie

- **clientScenario** – diskriminátor scenárov pre rozličné varianty informačného kanála.

- **ClientTimeStamp** – časová pečiatka zaznamenania udalosti v klientovi.

- **clientType** – aplikácia, v ktorej súčasť spustená.

- **DeviceInfo.Make** – názov výrobcu zariadenia alebo výrobcu OEM zariadenia.

- **DeviceInfo.NetworkProvider** – sieť alebo mobilný operátor, ako je napríklad AT&T.

- **DeviceInfo.NetworkType** – typ sieťových pripojení zariadenia, ako je napríklad káblové, Wi-Fi alebo WWAN (dátové/mobilné).

- **DeviceInfo.OsName** – názov operačného systému zariadenia.

- **DeviceInfo_SDKUid** – jednoznačne identifikuje zariadenie z perspektívy SDK telemetrie.

- **eventId** –identifikátor názvu udalosti.

- **EventInfo.SdkVersion** – verzia SDK telemetrie, ktorú klient použil na generovanie udalosti.

- **eventpriority** – hodnota enumerácie priority odoslania udalosti.

- **feature** – používa sa na zoskupovanie rôznych udalostí tej istej funkcie.

- **hostAppRing** – populácia používateľov, ktorým sa aplikácia distribuovala.

- **properties** – obsahuje dodatočné metaúdaje alebo vlastnosti zhromaždené pre každú udalosť. *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **publicEventName** – názov udalosti pre verejnosť.  

- **region** – geografická oblasť služby informačných kanálov, ku ktorej je používateľ pripojený. 

- **renderTime** – metrika na diagnostiku výkonu pri vykresľovaní informačného kanála.

- **tenantAadObjectId** – globálne jedinečný identifikátor pre podnikového nájomníka používateľa.

- **type** – typ zaznamenanej udalosti, napr. sledovanie, chyba, udalosť, QoS.

- **userAadObjectId** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft.

- **UserInfo.Id** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft.

- **UserInfo.IdType** – určuje typ ID používateľa. 

- **UserInfo.Language** – jazyk používateľa vo formáte značiek jazyka skupiny IETF.

- **UserInfo.MsaId** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **UserInfo.TimeZone** – časové pásmo používateľa vzťahujúce sa na čas UTC.

- **userPuid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **version** – verzia klienta informačného kanála.


#### <a name="officefeedbacksurveyfloodgateclientsurveytracked"></a>Office.Feedback.Survey.FloodgateClient.SurveyTracked

Táto udalosť sleduje, keď zariadenie oprávnené na prieskum spustí aplikáciu. Používa sa na posúdenie stavu procesu výberu používateľov prieskumu a na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefeedbacksurveyfloodgateclienttriggermet"></a>Office.Feedback.Survey.FloodgateClient.TriggerMet

Táto udalosť sleduje, keď zariadenie splnilo kritériá na zobrazenie prieskumu. Používa sa na posúdenie stavu procesu spustenia prieskumu a na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefeedbacksurveyfloodgateclientuserselected"></a>Office.Feedback.Survey.FloodgateClient.UserSelected

Táto udalosť sleduje, keď zariadenie bolo vybraté na prieskum. Používa sa na posúdenie stavu procesu výberu používateľov prieskumu a na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefeedbacksurveyuiandroid"></a>Office.Feedback.Survey.UI.Android

Táto udalosť v zariadení s Androidom sleduje, keď používateľ v zariadení má zobrazenú výzvu na prieskum a používateľské rozhranie prieskumu. Používa sa na posúdenie stavu funkcie prieskumu a na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefeedbacksurveyuiios"></a>Office.Feedback.Survey.UI.IOS

Táto udalosť v zariadení s iOS sleduje, keď používateľ v zariadení má zobrazenú výzvu na prieskum a používateľské rozhranie prieskumu. Používa sa na posúdenie stavu funkcie prieskumu a na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefeedbacksurveyuimac"></a>Office.Feedback.Survey.UI.Mac

Táto udalosť v Macu sleduje, keď používateľ v zariadení má zobrazenú výzvu na prieskum a používateľské rozhranie prieskumu. Používa sa na posúdenie stavu funkcie prieskumu a na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefeedbacksurveyuiwin32"></a>Office.Feedback.Survey.UI.Win32

Táto udalosť v zariadení s Windowsom sleduje, keď používateľ v zariadení má zobrazenú výzvu na prieskum a používateľské rozhranie prieskumu. Používa sa na posúdenie stavu funkcie prieskumu a na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefeedbacksurveyuiwin32toast"></a>Office.Feedback.Survey.UI.Win32.Toast

Táto udalosť sleduje, keď je zobrazená výzva na prieskum. Používa sa na posúdenie stavu procesu výzvy na prieskum, ako aj na to, aby sa zaistilo, že signál použitý na analýzu problémov zákazníkov a stavu funguje správne.

Zhromažďujú sa tieto polia:

- **ExpirationTimeUTC** – dátum a čas uplynutia platnosti prieskumu

- **SurveyName** – zobrazený názov prieskumu

- **SurveyId** – jedinečná inštancia kampane

- **UniqueId** – ID na identifikovanie jednotlivých položiek telemetrie

#### <a name="officefileiocsiccachedfilecsiloadfilebasic"></a>Office.FileIO.CSI.CCachedFileCsiLoadFileBasic

Umožňuje zistiť, či sa súbor úspešne otvoril z vrstvy FIO. Umožňuje sledovanie stavu funkcie a monitorovanie.

Zhromažďujú sa tieto polia:

  - **Activity.Group** – značka, ktorá umožňuje zoskupiť množinu udalostí monitorovania a spravovať celkovú úspešnosť

  - **Activity.IsHVA** – príznak, ktorý označuje, že udalosť je kritická pre úspešnosť používateľa

  - **Data.AsyncOpen** – príznak, ktorý označuje otvorený obsah, ktorý prišiel po otvorení hlavnej časti

  - **Data.CacheFileId** – pripája sa k telemetrii vyrovnávacej pamäte dokumentov balíka Office a umožňuje analýzu vplyvu problémov s vyrovnávacou pamäťou na prostredie používateľa
 
  - **Data. CFREnabled** – Označuje, že operácia CacheFileRuntime je pre túto reláciu povolená

  - **Data. CFRFailure** – Označuje, že operácia CacheFileRuntime narazila na chybu.
  
  - **Data.CoauthStatus** – hlási stav spolupráce v rámci dokumentu pri otvorení

  - **Data.CountOfMultiRoundTripsDownload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou

  - **Data.CountOfMultiRoundTripsUpload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou

  - **Data.DialogId** – nastaví sa, ak sa zobrazí dialógové okno používateľského rozhrania počas otvorenia s informáciou, že používateľovi sa zobrazila správa s upozornením

  - **Data.DidFallbackToDAV** – nastaví sa, ak bol dokument otvorený pomocou staršieho protokolu prenosu súborov

  - **Data.Doc.AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť

  - **Data.Doc.AssistedReadingReasons** – nastaví sa, ak je v dokumente zavedená ochrana elektronických údajov

  - **Data.Doc.AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data.Doc.ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

  - **Data.Doc.EdpState** – nastavenie ochrany elektronických údajov dokumentu

  - **Data.Doc.Ext** prípona dokumentu (docx, xlsb, pptx atď.)

  - **Data.Doc.Extension** – zastarané

  - **Data.Doc.FileFormat** – verzia protokolu formátu súboru

  - **Data.Doc.Fqdn** – názov domény OneDrivu alebo SharePointu Online

  - **Data.Doc.FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény

  - **Data.Doc.IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia

  - **Data.Doc.IdentityUniqueId** – zastarané

  - **Data.Doc.InitializationScenario** – zaznamenáva, ako bol dokument otvorený

  - **Data.Doc.IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky

  - **Data.Doc.IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa

  - **Data.Doc.IsCloudCollabEnabled** – príznak, ktorý označuje, že služba podporuje spoluprácu v cloude

  - **Data.Doc.IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo

  - **Data.Doc.IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce

  - **Data.Doc.IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline

  - **Data.Doc.IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu

  - **Data.Doc.Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data.Doc.LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument

  - **Data.Doc.NumberCoAuthors** – počet používateľov v relácii spoločných úprav

  - **Data.Doc.PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie

  - **Data.Doc.ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie

  - **Data.Doc.ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerProtocol** – verzia protokolu použitá na komunikáciu so službou

  - **Data.Doc.ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.)

  - **Data.Doc.ServerVersion** – verzia servera, ktorý ponúka službu

  - **Data.Doc.SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie

  - **Data.Doc.SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online

  - **Data.Doc.SizeInBytes** – indikátor veľkosti dokumentu

  - **Data.Doc.SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu

  - **Data.Doc.StorageProviderId** – zastarané

  - **Data.Doc.StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý

  - **Data.Doc.SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby)

  - **Data.Doc.UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu

  - **Data.Doc.UsedWrsDataOnOpen** – diagnostický indikátor prírastkového otvorenia dokumentu

  - **Data.Doc.WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI

  - **Data.DocumentLoadEndpoint** – zastaraný/redundantný duplikát (Data.Doc.Location a Data.Doc.IsSyncbacked)

  - **Data.DocumentSizeInBytes** – zastarané/redundantné, náhrada je Data.Doc. SizeInBytes

  - **Data.DocumentSizeOnDisk** – zastarané

  - **Data.DoesBaseHaveContentOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DownloadFragmentSize** – veľkosť údajov odoslaných v podradenej požiadavke na diagnostiku problémov so sieťou

  - **Data.DsmcStartedTooEarly** – označuje chybu pri začatí relácie spoločných úprav

  - **Data.EditorsCount** – počet ostatných spolupracovníkov upravujúcich dokument

  - **Data.ExcludedDataThresholdInBytes** – veľkosť súboru potrebná na použitie asynchrónneho otvorenia

  - **Data.FileIOResult.Code** – vyrovnávacia pamäť vráteného kódu posledného otvorenia z vrstvy protokolu

  - **Data.FileIOResult.Success** – vyrovnávacia pamäť indikátora úspešnosti posledného otvorenia z vrstvy protokolu

  - **Data.FileIOResult.Tag** – vyrovnávacia pamäť značky chyby posledného otvorenia z vrstvy protokolu

  - **Data.FileIOResult.Type** – vyrovnávacia pamäť typu chyby posledného otvorenia z vrstvy protokolu

  - **Data.FqdnHash** – zastarané, náhrada je Data\_Doc\_FqdnHash

  - **Data.FullIError** – vyrovnávacia pamäť kódov všetkých chýb otvorení z vrstvy protokolu

  - **Data.FullyQualifiedDomainName** – zastarané, náhrada je Data\_Doc\_Fqdn

  - **Data.Input.FileOpenState** – stav vyžiadaný aplikáciou (čítanie, čítanie a zápis atď.)

  - **Data.Input.OpenAsync** – asynchrónne otvorenie požadované aplikáciou

  - **Data.Input.OpenOfflineCopy** – otvorenie z kópie v režime offline požadované doplnkom

  - **Data.IOFlags** – zastarané

  - **Data.IsBaseBranchEmptyOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.IsCachedHistoricalVersion** – vyrovnávacia pamäť obsahuje staršiu verziu dokumentu

  - **Data.IsDocEnterpriseProtected** – dokument je chránený pomocou šifrovania (ochrana elektronických dokumentov/EDP)

  - **Data.IsDocInODC** – dokument bol otvorený ešte predtým a už je vo vyrovnávacej pamäti

  - **Data.IsMapUnMapCase** – súčasť stavu súboru vo vyrovnávacej pamäti

  - **Data.IsMapUnMapCase.End** – súčasť stavu súboru vo vyrovnávacej pamäti

  - **Data.IsOfficeHydrationInProgress** – dokument je obnovený z offline ukladacieho priestoru v systéme Windows

  - **Data.isOfficeHydrationRequired** – dokument je momentálne v offline ukladacom priestore

  - **Data.isOpenFromCollab** – najnovšia kópia dokumentu sa načítala zo zdieľanej služby spolupráce

  - **Data.isPendingNameExist** – prebieha premenovanie dokumentu

  - **Data.IsStubFile** – dokument ešte nebol uložený v cloudovej službe

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen** – zmenil sa stav dokumentu a zmeny možno nastali, kým dokument nebol otvorený

  - **Data.isTaskCanceledAfterOpenComplete** – zastarané

  - **Data.IsWorkingBranchAvailableOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.LicenseStatus** – stav licencie na diagnostický produkt, používa sa na overenie, že príslušné funkcie produktu sú povolené pre typ licencie používateľa 

  - **Data.LicenseType** – označuje stav licencie (bezplatná, platená, skúšobná atď.)

  - **Data.Location** – označuje typ úložného média (USB, Cloud atď.)

  - **Data.LockRequestDocMode** – označuje, či je dokument k dispozícii ostatným používateľom

  - **Data.MyDeferredValue** – zastarané

  - **Data.Network.BytesReceived** – zastarané

  - **Data.Network.BytesSent** – zastarané

  - **Data.Network.ConnectionsCreated** – zastarané

  - **Data.Network.ConnectionsEnded** – zastarané

  - **Data.OcsDisableReasons** – dôvod, prečo nebola pre dokument k dispozícii zdieľaná služba spolupráce

  - **Data.OcsHostOnOpen** – príznak, ktorý označuje, že ovládací prvok sa prepne na zdieľanú službu spolupráce počas otvorenia

  - **Data.OpeningOfflineCopy** – príznak, ktorý označuje, že sa otvorí lokálna kópia dokumentu

  - **Data.Partition** – zastarané

  - **Data.RequestTime** – zastarané

  - **Data.ResourceIdHash** – zastarané

  - **Data.ResumedIncrementalOpen** – zastarané

  - **Data.RTCEnabled** – spustil sa protokol rýchlej distribúcie zmien

  - **Data.SaveOnOpen** – neuložené zmeny v lokálnom dokumente sa uložili v službe počas otvorenia

  - **Data.ServerProtocol** – zastarané, náhrada je Data\_Doc\_ServerProtocol

  - **Data.ServerType** – zastarané, náhrada je Data\_Doc\_ServerType

  - **Data.ServerVersion** – zastarané, náhrada je Data\_Doc\_ServerVersion

  - **Data.ServiceId** – zastarané, náhrada je Data\_Doc\_WopiServiceId

  - **Data.SessionId** – zastarané

  - **Data.ShouldSwitchToServerOnly** – lokálnu kópiu dokumentu nie je možné použiť, je nutné použiť serverovú verziu

  - **Data.SpecialChars** – zastarané

  - **Data.StopwatchDuration** – zastarané

  - **Data.SyncBackedFileTelemetrySessionId** – zastarané

  - **Data.SyncElapsedTime** – zastarané

  - **Data.SyncRequestId** – zastarané

  - **Data.TestProperty** – zastarané

  - **Data.TransitionToHostOnOpen** – príznak, ktorý označuje, že relácia sa pripojí k službe, ktorá je hostiteľom dokumentu

  - **Data.TransitionToHostOnOpenResult** – stav prechodu na hostiteľskú službu

  - **Data.UseCachedNetworkConnection** – príznak, ktorý označuje, či sa pripojenie použilo opakovane alebo sa vytvorilo nové pripojenie

  - **Data.UseClientIdAsSchemaLockId** – príznak na kontrolu, ako sú dokumenty v službe uzamknuté

  - **Data. VersionType** – Označuje, ktorý typ verzie je aktuálna operácia otvorenia.

  - **Data.WopiServiceId** – zastarané, náhrada je Data\_Doc\_WopiServiceId

#### <a name="officefileiocsiccachedfilecsisavefilebasic"></a>Office.FileIO.CSI.CCachedFileCsiSaveFileBasic

Umožňuje zistiť, či sa súbor úspešne uložil z vrstvy FIO. Umožňuje sledovanie stavu funkcie a monitorovanie.

Zhromažďujú sa tieto polia:

  - **Activity.Group** – značka, ktorá umožňuje zoskupiť množinu udalostí monitorovania a spravovať celkovú úspešnosť

  - **Activity.IsHVA** – príznak, ktorý označuje, že udalosť je kritická pre úspešnosť používateľa

  - **Data.AsyncOpen** – príznak, ktorý označuje, že dokument bol otvorený s obsahom, ktorý prišiel po otvorení hlavnej časti

  - **Data.BaseDownloadTriggered** – diagnostické sledovanie zmien, ktoré označuje, že bola požadovaná základná verzia dokumentu

  - **Data.BlockAutoUploadReasons** – kódy príčin stavu blokovania nahrávania (napr. je vypnuté automatické ukladanie, dokument je v prechode)

  - **Data.BlockUploadDueToFailedSaveAsOverExisting** – nahrávanie sa zablokuje, keď zlyhalo pri opakovanom pokuse

  - **Data.CacheFileId** – pripája sa k telemetrii vyrovnávacej pamäte dokumentov balíka Office a umožňuje analýzu vplyvu problémov s vyrovnávacou pamäťou na prostredie používateľa

  - **Data.ChartType** – zastarané

  - **Data.CoAuthStatus** – hlási stav spolupráce v rámci dokumentu pri uložení

  - **Data.CoauthUpdatesContext** – hlási kontext (zlúčenie/prírastkové otvorenie)

  - **Data.CountOfMultiRoundTripsDownload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou

  - **Data.CountOfMultiRoundTripsUpload** – počet výmen údajov na serveri, ktoré sa používajú na riešenie problémov s výkonom a sieťou
  
  - **Data. CFREnabled** – Označuje, že operácia CacheFileRuntime je pre túto reláciu povolená

  - **Data. CFRFailure** – Označuje, že operácia CacheFileRuntime narazila na chybu.

  - **Data.DialogChoice** – zaznamenáva výber v každom dialógovom okne chyby

  - **Data.DialogId** – zaznamenáva ID dialógového okna každého dialógového okna chyby, ktoré sa zobrazí počas ukladania

  - **Data.Dmc.IsOcsSupported** – zastarané

  - **Data.Doc.AccessMode** – dokument je iba na čítanie

  - **Data.Doc.AssistedReadingReasons** – nastaví sa, ak je v dokumente zavedená ochrana elektronických údajov

  - **Data.Doc.AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data.Doc.ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

  - **Data.Doc.EdpState** – nastavenie ochrany elektronických údajov dokumentu

  - **Data.Doc.Ext** – prípona dokumentu (docx, xlsm, pptx atď.)

  - **Data.Doc.Extension** – zastarané

  - **Data.Doc.FileFormat** – verzia protokolu formátu súboru

  - **Data.Doc.Fqdn** – názov domény OneDrivu alebo SharePointu Online

  - **Data.Doc.FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény

  - **Data.Doc.FqdnHasi** – zastarané

  - **Data.Doc.IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie uloženia

  - **Data.Doc.IdentityUniqueId** – zastarané

  - **Data.Doc.IKFlags** – zastarané

  - **Data.Doc.InitializationScenario** – zaznamenáva, ako bol dokument otvorený

  - **Data.Doc.IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky

  - **Data.Doc.IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa

  - **Data.Doc.IsCloudCollabEnabled** – príznak, ktorý označuje, že aplikácia podporuje spoluprácu v cloude

  - **Data.Doc.IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo

  - **Data.Doc.IsOcsSupported** – príznak, ktorý označuje, že dokument podporuje spoluprácu v cloude

  - **Data.Doc.IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline

  - **Data.Doc.IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu

  - **Data.Doc.Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data.Doc.LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument

  - **Data.Doc.NumberCoAuthors** – počet používateľov v relácii spoločných úprav

  - **Data.Doc.PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie

  - **Data.Doc.ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie

  - **Data.Doc.ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov

  - **Data.Doc.ServerProtocol** – verzia protokolu použitá na komunikáciu so službou

  - **Data.Doc.ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.)

  - **Data.Doc.ServerVersion** – verzia servera, ktorý ponúka službu

  - **Data.Doc.SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie

  - **Data.Doc.SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online

  - **Data.Doc.SizeInBytes** – indikátor veľkosti dokumentu

  - **Data.Doc.SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu

  - **Data.Doc.StorageProviderId** – zastarané

  - **Data.Doc.StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý

  - **Data.Doc.SussionId** – zastarané

  - **Data.Doc.SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby)

  - **Data.Doc.UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu

  - **Data.Doc.UsedWrsDataOnOpen** – diagnostický indikátor prírastkového otvorenia dokumentu

  - **Data.Doc.WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI

  - **Data.DocnReadOnlyReasons** – zastarané

  - **Data.DocumentSaveEndpoint** – zastaraný, náhrada je Data\_Doc\_Location

  - **Data.DocumentSaveType** – typ uloženia (Normálne, Vytvoriť, Uložiť ako)

  - **Data.DocumentSizeOnDisk** – zastarané, náhrada je Data\_Doc\_SizeInBytes

  - **Data.DoesBaseHaveContentOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DoesWorkingBranchHaveExcludedDataOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.DstDoc.AccessMode** – označuje, či je nový dokument iba na čítanie alebo sa dá upraviť

  - **Data.DstDoc.EdpState** – nastavenie ochrany elektronických údajov nového dokumentu

  - **Data.DstDoc.Extension** – prípona nového dokumentu (docx, xlsm, pptx atď.)

  - **Data.DstDoc.FileFormat** – protokol formátu súboru nového dokumentu

  - **Data.DstDoc.Fqdn** – názov domény nového dokumentu OneDrivu alebo SharePointu Online

  - **Data.DstDoc.FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény nového dokumentu

  - **Data.DstDoc.IdentityUniqueId** – zastarané

  - **Data.DstDoc.IOFlags** – príznaky možností vo vyrovnávacej pamäti nového dokumentu použité pri otvorení

  - **Data.DstDoc.IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia nového dokumentu v režime offline

  - **Data.DstDoc.IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu

  - **Data.DstDoc.Location** – označuje, ktorá služba poskytla nový dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data.DstDoc.NumberCoAuthors** – počet používateľov v relácii spoločných úprav v novom dokumente

  - **Data.DstDoc.ReadOnlyReasons** – dôvody, prečo bol nový dokument otvorený iba na čítanie

  - **Data.DstDoc.ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov s novým dokumentom

  - **Data.DstDoc.ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov s novým dokumentom

  - **Data.DstDoc.ServerProtocol** – verzia protokolu použitá na komunikáciu so službou pri tvorbe nového dokumentu

  - **Data.DstDoc.ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.) pre nový dokument

  - **Data.DstDoc.ServerVersion** – verzia servera, ktorý ponúka službu pre nový dokument

  - **Data.DstDoc.SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie pre nový dokument

  - **Data.DstDoc.SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online pre nový dokument

  - **Data.DstDoc.SizeInBytes** – indikátor veľkosti nového dokumentu

  - **Data.DstDoc.UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu pre nový dokument

  - **Data.EditorsCount** – počet ostatných spolupracovníkov upravujúcich dokument

  - **Data.FullIError** – vyrovnávacia pamäť kódov všetkých chýb z vrstvy protokolu

  - **Data.HasFilteredCategories** – zastarané

  - **Data.HasFilteredCategoryNames** – zastarané

  - **Data.HasFilteredSeries** – zastarané

  - **Data.HasFilteredSeriesNames** – zastarané

  - **Data.HasPendingSaveAs** – označuje, že prebieha požiadavka Uložiť ako/Uložiť kópiu

  - **Data.Input.FileOpenState** – stav požadovaný aplikáciou (Na čítanie alebo Na čítanie a zapisovanie atď.)

  - **Data.Input.FileSaveState** – stav požadovaný aplikáciou (uloženie pri otvorení, uloženie pod iným názvom atď.)

  - **Data.Input.NetworkCost** – označuje typ nákladov na sieť (účtované podľa objemu údajov, účtované podľa objemu údajov nad limit atď.)

  - **Data.Input.OpenAsync** – príznak, ktorý označuje, že aplikácia požadovala asynchrónne otvorenie

  - **Data.Input.OpenOfflineCopy** – príznak, ktorý označuje, že aplikácia požadovala otvorenie offline

  - **Data.IsCachedHistoricalVersion** – označuje, že tento súbor vo vyrovnávacej pamäti nie je najnovšia verzia

  - **Data.IsHtml** – označuje, že bol vložený text vo formáte HTML

  - **Data.IsLegacyCode** – označuje, že bol vložený text vo formáte so starším kódom

  - **Data.IsLocalOnlyFile** – označuje, že súbor bol otvorený iba z lokálneho ukladacieho priestoru

  - **Data.IsLocalOrSyncBackedFile** – označuje, že súbor bol otvorený lokálne a priradený k službe

  - **Data.IsMapUnMapCase** – súčasť stavu súboru vo vyrovnávacej pamäti

  - **Data.isOpenFromCollab** – označuje, že súbor bol otvorený zo zdieľanej služby spolupráce

  - **Data.IsStubFile** – dokument ešte nebol zdieľaný v cloudovej službe

  - **Data.IsSyncBackedFile** – dokument sa nachádza v priečinku, ktorý je automaticky synchronizovane aktualizovaný

  - **Data.IsSyncBackedStateDifferentThanOnLastOpen** – zmenil sa stav dokumentu a zmeny možno nastali, kým dokument nebol otvorený

  - **Data.IsWorkingBranchAvailableOnOpen** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.Location** – označuje typ úložného média (USB, Cloud atď.)

  - **Data.LockRequestDocMode** – označuje, či je dokument k dispozícii ostatným používateľom

  - **Data.MruRequestResult** – zastarané

  - **Data.NewDataNotAvailableReason** – zastarané

  - **Data.OcsDisableReasons** – nepoužíva sa uložením

  - **Data.OcsHostOnOpen** – nepoužíva sa uložením

  - **Data.Output.FileSaveState** – stav pri dokončení uloženia

  - **Data.PivotChart** – zastarané

  - **Data.resolveConflictState** – kódy príčin požiadavky na vyriešenie konfliktov zlúčenia

  - **Data.RTCEnabled** – spustil sa protokol rýchlej distribúcie zmien

  - **Data.SaveAsToCurrent** – označuje, že aktívny dokument prepíše uložený súbor

  - **Data.ServiceId** – zastarané, náhrada je Data\_Doc\_WopiServiceId

  - **Data.SessionId** – zastarané

  - **Data.SizeInBytes** – zastarané, náhrada je Data\_Doc\_SizeInBytes

  - **Data.StopwatchDuration** – zastarané

  - **Data.SyncBackedFileRequiresOnlineTransition** – príznak, ktorý označuje, že akcia uloženia je dočasne blokovaná online prechodom

  - **Data.SyncBackedFileSaveOnOpen** – príznak, ktorý označuje, že zmeny vykonané automatickou synchronizáciou vyžadujú uloženie pri otvorení

  - **Data.TelemetryId** – zastarané

  - **Data.TriggerSaveAfterBaseDownload** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.UploadBlockedDueToCoherencyFailure** – uloženie do služby blokované, čaká sa na vyriešenie konfliktných zmien používateľom

  - **Data.UploadBlockedDueToFailedSaveAsOverExisting** – uloženie do služby blokované v dôsledku neúspešného pokusu o prepísanie existujúceho súboru

  - **Data.UploadPreemptedForCoherency** – uloženie do služby bolo zrušené, pretože používateľ vykonáva ďalšie zmeny

  - **Data.UploadPreemptedForSaveAsOverExistingFailure** – uloženie do služby bolo zrušené v dôsledku skoršieho zlyhania SaveAsOverExisting

  - **Data.UploadScheduled** – súbor je pripravený na asynchrónne nahratie do služby

  - **Data.UseClientIdAsSchemaLockId** – príznak na kontrolu, ako sú dokumenty v službe uzamknuté

  - **Data.WorkingCopySaved** – diagnostické sledovanie zmien, ktoré zabezpečí najnovšiu verziu zdieľaného súboru

  - **Data.ZrtSaveAsforSyncBackedBusinessEnabled** – príznak, ktorý označuje rýchle ukladanie povolené pre SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedConsumerEnabled** – príznak, ktorý označuje rýchle ukladanie povolené pre OneDrive Consumer

  - **Data.ZrtSaveAsforSyncBackedCTBusinessEnabled** – príznak, ktorý označuje typy obsahu na rýchle ukladanie povolené pre SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedCTConsumerEnabled** – príznak, ktorý označuje typy obsahu na rýchle ukladanie povolené pre OneDrive Consumer

  - **Data.ZrtSaveAsforSyncBackedMetaDataBusinessEnabled** – príznak, ktorý označuje rýchle ukladanie metaúdajov súborov povolené pre SharePoint Online

  - **Data.ZrtSaveAsforSyncBackedMetaDataConsumerEnabled** – príznak, ktorý označuje rýchle ukladanie metaúdajov súborov povolené pre OneDrive Consumer

#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Zhromažďuje sa, ak spustenie aplikácie zlyhá z dôvodu výskytu neočakávanej chyby počas spúšťania. Používa na sledovanie výnimiek a zlyhaní. Pomáha monitorovať a ladiť stav aplikácie.

Zhromažďujú sa tieto polia:
- **DateTime** – časová pečiatka zaznamenania udalosti

- **EventName** – názov udalosti, ktorá sa práve zaznamenáva

#### <a name="officefirstrunappleactivationresult"></a>Office.FirstRun.Apple.ActivationResult

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu aktivácie aplikácie. Zhromažďujeme údaje na zistenie výsledku aktivácie predplatného služieb Office 365 spolu s postupom, ktorý sa používa na aktiváciu (prvé spustenie, postup v aplikácii, nákup atď.).

Zhromažďujú sa tieto polia:

- **Data_ActivationStatusCollectionTime** – Časová pečiatka.

- **Data_ActivationStatusError** – Kód chyby aktivácie.

- **Data_ActivationStatusFlowType** – Číselná hodnota označujúca typ postupu aktivácie.

#### <a name="officefirstrunappleactivationstatus"></a>Office.FirstRun.Apple.ActivationStatus

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zistenie výsledku aktivácie predplatného služieb Office 365 spolu s postupom, ktorý sa používa na aktiváciu (FRE, InApp, Purchase atď.). Zhromažďujeme údaje obsahujúce typ aktivácie, typ postupu (FRE/DocStage/Purchase) a ID licenčnej služby balíka Office.

Zhromažďujú sa tieto polia:

- **Data_ActivationTypeCollectionTime** – Časová pečiatka.

- **Data_ActivationTypeFlowType** – Číselná hodnota označujúca typ postupu aktivácie.

- **Data_ActivationTypeOLSLicense** – Identifikátor licencie.

- **Data_ActivationTypeStatus** – Kód stavu aktivácie.

#### <a name="officefirstrunapplefirstruncomplete"></a>Office.FirstRun.Apple.FirstRunComplete

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám umožňuje zistiť, ak je používateľ spustený v rámci modelu freemium, typ spusteného postupu (FRE/DocStage/Purchase) a typ identity (MSA/OrgID). Túto udalosť používame na to, aby sme zistili, či bolo dokončené prvé spustenie (FRE) a aký typ identity sa použil na prihlásenie (MSA/OrgID).

Zhromažďujú sa tieto polia:

- **Data_FirstRunCompletedCollectionTime** – Časová pečiatka registrujúca čas, v ktorom sa postup dokončil.

- **Data_FirstRunCompletedFlowType** – Kód označujúci typ dokončeného postupu používateľa. 

- **Data_FirstRunCompletedFreemiumStatus** – Kód predstavujúci stav dokončenia postupu používateľa v modeli freemium.

- **Data_FirstRunCompletedIdentityType** – Typ identity používateľa, ktorý postup dokončil.

#### <a name="officefirstrunapplefirstrunstart"></a>Office.FirstRun.Apple.FirstRunStart

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám umožňuje vedieť, že používateľ zadal prvé spustenie a typ spusteného postupu (FRE/DocStage/Purchase). Túto udalosť používame na to, aby sme zistili, či sa prvé spustenie (FRE) začalo úspešne.

Zhromažďujú sa tieto polia:

- **Data_FirstRunStartedCollectionTime** – Časová pečiatka registrujúca čas, v ktorom sa postup dokončil.

- **Data_FirstRunStartedFlowType** – Kód označujúci typ dokončeného postupu používateľa. 

#### <a name="officefirstrunapplefirstrunstartedandcompleted"></a>Office.FirstRun.Apple.FirstRunStartedAndCompleted

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám umožňuje zistiť, ak je používateľ spustený v rámci modelu freemium, typ spusteného postupu (FRE/DocStage/Purchase) a typ identity (MSA/OrgID). Túto udalosť používame na to, aby sme zistili stav a účinnosť postupu skúsenosti s prvým spustením (FRE).

Zhromažďujú sa tieto polia:

- **Data_FirstRunCompletedCollectionTime** – Časová pečiatka registrujúca čas, v ktorom sa postup dokončil.

- **Data_FirstRunCompletedFlowType** – Kód označujúci typ dokončeného postupu používateľa.  

- **Data_FirstRunCompletedFreemiumStatus** – Kód predstavujúci stav dokončenia postupu používateľa v modeli freemium.

- **Data_FirstRunCompletedIdentityType** – Typ identity používateľa, ktorý postup dokončil.

- **Data_FirstRunStartedCollectionTime** – Časová pečiatka registrujúca čas, v ktorom sa postup začal.

- **Data_FirstRunStartedFlowType** – Kód označujúci typ začatého postupu používateľa.

#### <a name="officefirstrunappleinapppurchaseactivationfail"></a>Office.FirstRun.Apple.InAppPurchaseActivationFail

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu aktivácie aplikácie. Zhromažďujeme údaje na zistenie výsledku aktivácie nákupu v aplikácii spolu s postupom, ktorý sa používa na aktiváciu (prvé spustenie, postup v aplikácii, nákup atď.). 

Zhromažďujú sa tieto polia:

- **Data_ActivationFailCollectionTime** – Časová pečiatka registrujúca čas, v ktorom sa vyskytla chyba aktivácie. 

- **Data_ActivationFailFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_AssoicatedSuccessfullyCollectionTime** – Časová pečiatka registrujúca čas, v ktorom nastalo priradenie. 

- **Data_AssoicatedSuccessfullyFlowType** – Kód označujúci typ uplatneného postupu používateľa.

#### <a name="officefirstrunappleinapppurchaseactivationsuccess"></a>Office.FirstRun.Apple.InAppPurchaseActivationSuccess

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu aktivácie aplikácie. Zhromažďujeme údaje na zistenie výsledku aktivácie nákupu v aplikácii spolu s postupom, ktorý sa používa na aktiváciu (prvé spustenie, postup v aplikácii, nákup atď.). 

Zhromažďujú sa tieto polia:

- **Data_ActivatedSuccessfullyCollectionTime** – Časová pečiatka registrujúca čas, v ktorom nastala aktivácia. 

- **Data_ActivatedSuccessfullyFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_AssoicatedSuccessfullyCollectionTime** – Časová pečiatka registrujúca čas, v ktorom nastalo priradenie. 

- **Data_AssoicatedSuccessfullyFlowType** – Kód označujúci typ uplatneného postupu používateľa.

#### <a name="officefirstrunappleinapppurchaseassociationfailed"></a>Office.FirstRun.Apple.InAppPurchaseAssociationFailed

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu aktivácie aplikácie. Zhromažďujeme údaje na zistenie výsledku aktivácie nákupu v aplikácii spolu s postupom, ktorý sa používa na aktiváciu (prvé spustenie, postup v aplikácii, nákup atď.). 

Zhromažďujú sa tieto polia:

- **Data_AppChargedSuccessfullyCollectionTime** – Časová pečiatka registrujúca čas, v ktorom bol nákup zaúčtovaný.

- **Data_AppChargedSuccessfullyFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_AssoicationFailedCollectionTime** – Časová pečiatka registrujúca čas, v ktorom zlyhalo priradenie aplikácie.

- **Data_AssoicationFailedFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_AssoicationFailedResult** – Kód označujúci typ zisteného zlyhania.

#### <a name="officefirstrunappleinapppurchaseassociationsuccess"></a>Office.FirstRun.Apple.InAppPurchaseAssociationSuccess

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu aktivácie aplikácie. Zhromažďujeme údaje na zistenie výsledku aktivácie nákupu v aplikácii spolu s postupom, ktorý sa používa na aktiváciu (prvé spustenie, postup v aplikácii, nákup atď.). 

Zhromažďujú sa tieto polia:

- **Data_AppChargedSuccessfullyCollectionTime** – Časová pečiatka registrujúca čas, v ktorom bol nákup zaúčtovaný.

- **Data_AppChargedSuccessfullyFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_AssoicatedSuccessfullyCollectionTime** – Časová pečiatka registrujúca čas, v ktorom zlyhalo priradenie aplikácie.

- **Data_AssoicatedSuccessfullyFlowType** – Kód označujúci typ uplatneného postupu používateľa.

#### <a name="officefirstrunappleinapppurchasefailures"></a>Office.FirstRun.Apple.InAppPurchaseFailures

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu aktivácie aplikácie. Zhromažďujeme údaje o výsledku postupu nákupu v rámci aplikácie.

Zhromažďujú sa tieto polia:

- **Data_AppStoreFailureFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_AppStoreFailureResult** – Zistený výsledok zlyhania.

- **Data_CancelRequestFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_EventId** – Kód označujúci typ zisteného zlyhania.

#### <a name="officefirstrunappleinapppurchasesattempted"></a>Office.FirstRun.Apple.InAppPurchasesAttempted

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu nákupu aplikácie v rámci aplikácie. Zhromažďujeme údaje na sledovanie pokusov o nákupy v aplikácii a typu jednotky SKU, ktorá sa zakupuje (mesačné/ročné/domáce/osobné).

Zhromažďujú sa tieto polia:

- **Data_EventId** – Kód označujúci typ zisteného výsledku.

- **Data_PurchasedClickedOfferType** – Typ jednotky SKU s pokusom o nákup.

- **Data_PurchaseSuccessfulFlowType** – Kód označujúci typ uplatneného postupu používateľa.

#### <a name="officefirstrunappleinapprestoreattempted"></a>Office.FirstRun.Apple.InAppRestoreAttempted

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu nákupu aplikácie v rámci aplikácie. Zhromažďujeme údaje na sledovanie pokusov o obnovenie v rámci aplikácie.

Zhromažďujú sa tieto polia:

- **Data_EventId** – Kód označujúci typ výsledku pokusu.

- **Data_RestoreAttemptFlowType** – Kód označujúci typ uplatneného postupu používateľa.

#### <a name="officefirstrunappleinapprestoreattemptfailed"></a>Office.FirstRun.Apple.InAppRestoreAttemptFailed

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu postupu nákupu aplikácie v rámci aplikácie. Zhromažďujeme údaje na sledovanie pokusov o obnovenie v rámci aplikácie a ich priradených postupov a chýb.

Zhromažďujú sa tieto polia:

- **Data_RestoreButtonFlowType** – Kód označujúci typ uplatneného postupu používateľa.

- **Data_RestoredFailedPaymentCancelledFlowType** – Kód označujúci typ uplatneného postupu zrušenia platby.

- **Data_RestoredFailedUnKnownFlowType** – Či pokus zlyhal z dôvodu uplatnenia neočakávaného postupu používateľa.

- **Data_RestoredFailedUnKnownResult** – Či pokus zlyhal z neznámych dôvodov.

#### <a name="officefirstrunapplemacfirstruncompleted"></a>Office.FirstRun.Apple.MacFirstRunCompleted

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám umožňuje vedieť, že používateľ prešiel prvým spustením. Túto udalosť používame na to, aby sme zistili, či sa prvé spustenie (FRE) dokončilo úspešne.

Zhromažďujú sa tieto polia:

- **Data_FirstRunCollectionTime** – Časová pečiatka registrujúca čas, v ktorom sa postup dokončil.

#### <a name="officefirstrunapplemacwxpfirstrunstarted"></a>Office.FirstRun.Apple.MacWXPFirstRunStarted

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám umožňuje vedieť, že používateľ zadal prvé spustenie. Túto udalosť používame na to, aby sme zistili, či sa prvé spustenie (FRE) začalo úspešne.

Zhromažďujú sa tieto polia:

- **Data_FirstRunPanelName** – Názov panela, z ktorého skäsenosť začala.

#### <a name="officelenslenssdkcloudconnectorlaunch"></a>Office.Lens.LensSdk.CloudConnectorLaunch

Keď používateľ oreže obrázok a ťukne na potvrdenie konečného výberu obrázka na použitie OCR, táto udalosť sa zhromaždí.     
Toto je záznam medzi používateľom a žiadosťou o službu, pretože v službe neexistuje priradenie medzi používateľom a úlohou služby. UserId sa vyžaduje na splnenie požiadaviek nariadenia o ochrane údajov (GDPR), pretože služba nie je vystavená používateľom priamo, ale prostredníctvom klientov, a na identifikáciu celkového počtu ľudí, ktorí túto službu používajú, čo pomáha službe sledovať objem používateľov, ktorí produkt používajú, ako aj identifikovať zmeny trendov a vyhľadávať a riešiť problémy v produkte.

Zhromažďujú sa tieto polia:

- **CallType** – reťazec na identifikáciu, či bolo volanie rozhrania API synchrónne alebo asynchrónne.

- **CloudConnectorRequestId** – reťazec, ktorý identifikuje žiadosť o službu, ktorá bola vykonaná na konverziu obrázkov prostredníctvom služby. 

- **CloudConnectorTarget** – reťazec, ktorý potvrdzuje, aký typ konverzie služba vykoná s obrázkami, ako je napríklad konvertovanie na PDF, Docx, text atď.

- **CustomerID** – reťazec, ktorý identifikuje používateľa, ktorý vlastní spracúvané obrázky.

- **CustomerType** – reťazec, ktorý identifikuje zákazníka ako podnikového alebo individuálneho používateľa. Toto rozlíšenie ovplyvňuje počet obrázkov (kvótu), ktoré môže klient naraz konvertovať. 

- **RelationId** – reťazec, ktorý identifikuje koreláciu medzi Lensom a službou, ktorá sa použila na spracovanie súborov.


#### <a name="officelenslenssdkcloudconnectoruploaderror"></a>Office.Lens.LensSdk.CloudConnectorUploadError

Pri konverzii obrázka na tabuľku keď používateľ ťukne na položku Zdieľať, Kopírovať alebo Otvoriť, opravy v tabuľke vykonané používateľom sa zdieľajú so službou na vylepšenie OCR. Táto udalosť sa zhromažďuje pri chybovej odpovedi tejto služby a obsahuje príslušné identifikátory na riešenie rôznych problémov v službe. 

Zhromažďujú sa tieto polia:

- **CloudConnectorRequestId** – identifikátor reťazca na prepojenie úlohy služby s aktuálnou žiadosťou o službu, pre ktorú sa zdieľali údaje o zlepšení.

- **CorrelationId** – reťazec, ktorý obsahuje identifikátor aktuálnej inštancie úlohy služby.

- **Reason** – reťazec, ktorý obsahuje kód chyby a popis chyby.

- **TargetType** – reťazec, ktorý identifikuje koncový bod služby.

- **TaskType** – reťazec, ktorý identifikuje zámer volania služby.


#### <a name="officelenslenssdkcloudconnectoruploadsuccess"></a>Office.Lens.LensSdk.CloudConnectorUploadSuccess

Pri konverzii obrázka na tabuľku keď používateľ ťukne na položku Zdieľať, Kopírovať alebo Otvoriť, opravy v tabuľke vykonané používateľom sa zdieľajú so službou na vylepšenie OCR. Táto udalosť sa zhromažďuje pri úspešnej odpovedi tejto služby a obsahuje príslušné identifikátory na riešenie problémov s procesom. Pomáha tiež analyzovať využívanie kanála vylepšovania služby.

Zhromažďujú sa tieto polia:

- **CloudConnectorRequestId** – identifikátor reťazca na prepojenie úlohy služby s aktuálnou žiadosťou o službu, pre ktorú sa zdieľali údaje o zlepšení.

- **CorrelationId** – reťazec, ktorý obsahuje identifikátor aktuálnej inštancie úlohy služby.

- **TargetType** – reťazec, ktorý identifikuje koncový bod služby.

- **TaskType** – reťazec, ktorý identifikuje zámer volania služby.


#### <a name="officelenslenssdkpermission"></a>Office.Lens.LensSdk.Permission

Povolenia sú citlivou funkciou, pretože bez nich používateľ nemôže používať žiadne funkcie Lensu. Povolenia sa sledujú na pochopenie používateľských zvykov na poskytovanie alebo zrušenie povolení. Keď používateľ pracuje s akýmkoľvek dialógovým oknom povolení v našej aplikácii, zhromažďujeme tieto udalosti. Na základe používateľských trendov na prijímanie a odmietanie povolení identifikujeme vylepšenia funkcií, ktoré používateľom pomáhajú porozumieť tomu, prečo sú povolenia dôležité.

Zhromažďujú sa tieto polia:

- **Data_action** – obsahuje hodnoty ako CameraPermissionAllowed (alebo Denied), StoragePermissionGranted (alebo Denied), ktoré nám pomáhajú pochopiť, či používateľ prijal alebo odmietol povolenia na úložisko a kameru.

- **Data_Action** – Toto pole nám pomáha pochopiť, aký typ povolenia sa žiadal od používateľa, napríklad Fotoaparát alebo Úložisko

- **Data_status** – obsahuje hodnoty ako Allowed, Denied a DeniedForever, ktoré nám pomáhajú pochopiť, či používateľ prijal alebo odmietol povolenia na úložisko a kameru.


#### <a name="officelenslenssdksavemedia"></a>Office.Lens.LensSdk.SaveMedia

Táto udalosť sa vyvolá, keď používateľ klikne na tlačidlo Hotovo a uloží obrázky v Androide a iOS. Pomáha merať úroveň interakcie používateľov kvantifikovaním používateľov, ktorí nakoniec uložia obrázky prostredníctvom našej aplikácie.

V Androide sa zhromažďujú tieto polia:

- **Data_FileSizeAfterCleanUp** – veľkosť súboru po vyčistení aplikáciou, aby sa pochopilo, koľko kompresie sa dosiahlo po vyčistení.

- **Data_FileSizeAfterSave** – veľkosť súboru po uložení používateľom, aby sa pochopilo, koľko kompresie sa dosiahlo po uložení.

- **Data_FileSizeBeforeCleanUp** – veľkosť súboru pred vyčistením aplikáciou, aby sa pochopilo, aká bola zachytená veľkosť

- **Data_Filter** – filter použitý na obrázok.

- **Data_ImageHeightAfterCleanUp** – výška obrázka po jeho vyčistení aplikáciou.

- **Data_ImageHeightBeforeCleanUp** – výška obrázka pred jeho vyčistením aplikáciou.

- **Data_ImageWidthAfterCleanUp** – šírka obrázka po jeho vyčistení aplikáciou.

- **Data_ImageWidthBeforeCleanUp** – šírka obrázka pred jeho vyčistením aplikáciou.

- **Data_MediaId** – identifikátor obrázkov, ktorý pomáha sledovať úspešnosť operácie.

- **Data_ProcessMode** – režim používateľa v čase uloženia obrázka používateľom.

- **Data_Source** – definuje, odkiaľ sa obrázok získal, napríklad zachytený fotoaparátom, importovaný z galérie atď. 

V iOS sa zhromažďujú tieto polia:

- **Data_filter** – filter použitý na obrázok. 

- **Data_imageDPI** – zmenšenie obrázka použité na uložený súbor obrázka

- **Data_imageSize** – veľkosť obrázka po uložení obrázka používateľom

- **Data_mediaId** – identifikátor obrázkov, ktorý pomáha sledovať úspešnosť operácie.

- **Data_mode** – režim používateľa v čase uloženia obrázka používateľom.

- **Data_sizeinPixel** – veľkosť obrázka vo forme pixelov

- **Data_source** – definuje, odkiaľ sa obrázok získal, napríklad zachytený fotoaparátom, importovaný z galérie atď. 


#### <a name="officelenslenssdkserviceidmapping"></a>Office.Lens.LensSdk.ServiceIDMapping

Keď sa obrázok úspešne nahrá do služby, táto udalosť sa zhromaždí. Znamená to, že služba teraz spustí jednu alebo viac úloh na spracovanie obrázka, a obsahuje príslušné identifikátory na pomoc pri riešení problémov s týmto procesom. Pomáha tiež analyzovať využívanie jednotlivých funkcií služby.

Zhromažďujú sa tieto polia:

- **CloudConnectorRequestId** – reťazec, ktorý identifikuje žiadosť o službu, ktorá bola vykonaná na konverziu obrázkov prostredníctvom služby.

- **I2DserviceProcessID** – reťazec, ktorý identifikuje úlohu služby, ktorá spúšťa konkrétnu podpožiadavku 


#### <a name="officeiospaywallpaywallpresented"></a>Office.iOS.Paywall.Paywall.Presented

Táto telemetria kritického používania sa zhromažďuje, keď sa používateľovi zobrazí ovládací prvok platobnej brány a používa sa na vysvetlenie skúsenosti používateľa pri nákupe v rámci aplikácie a optimalizovanie toho istého pre budúce verzie.

Zhromažďujú sa tieto polia:

- **entryPoint** – reťazec – tlačidlo/tok spracovania, ktorým sa zobrazuje platobná stena. Napríklad „Premium Upgrade Button” alebo „First Run Flow”.

- **isFRE** – boolovská hodnota – zobrazuje sa prostredie prvého spustenia alebo bežné používateľské rozhranie?

#### <a name="officeiospaywallpaywallstats"></a>Office.iOS.Paywall.Paywall.Stats

Tieto metaúdaje založené na relácii sa zhromažďujú pri zobrazovaní používateľského rozhrania platobnej steny, trvanie interakcie, či sa uskutočnil pokus o nákup a či a bol úspešný alebo zlyhal.  Tieto údaje sa používajú na porozumenie používaniu a stavu celej platobnej funkcie a na ladenie, optimalizáciu a riešenie problémov s funkciou nakupovania v aplikácii v budúcich verziách.

Zhromažďujú sa tieto polia:

- **entryPoint** – reťazec – tlačidlo/tok spracovania, ktorým sa zobrazuje platobná stena. Napríklad „Premium Upgrade Button” alebo „First Run Flow”.

- **isFRE** – boolovská hodnota – zobrazuje sa prostredie prvého spustenia alebo bežné používateľské rozhranie?

- **status** – reťazec – stav ukončenia platobnej steny. Napríklad „initiated“, „paymentDone“, „provisionFailed“

- **userDuration** – double – čas v milisekundách, ktorý používateľ strávil v platobnej stene

#### <a name="officeiospaywallskuchoosermorebenefitsstats"></a>Office.iOS.Paywall.SKUChooser.MoreBenefits.Stats

Táto udalosť zhromažďuje funkcie a aplikácie, ktoré používateľ rozbaľuje z ponuky Zobraziť ďalšie výhody a trvanie stráveného času.  Údaje sa používajú na vysvetlenie používania funkcie „Zobraziť všetky výhody“ a ďalšiu optimalizáciu skúseností v budúcich verziách.

Zhromažďujú sa tieto polia:

- **appsExpanded** – reťazec – zoznam služieb alebo aplikácií oddelených čiarkami, pre ktoré sa rozbalili výhody.

- **productId** – reťazec – AppStore ID produktu, pre ktorý si používateľ prezerá ďalšie ponúkané výhody

- **userDuration** – double – čas v milisekundách, ktorý používateľ strávil na obrazovke Výhody.

#### <a name="officeiospaywallskuchooserstats"></a>Office.iOS.Paywall.SKUChooser.Stats

Táto telemetria používania sa zhromažďuje, aby sa zistilo, ako používateľ prešiel na výber jednotiek SKU, koľko času používateľ strávil na obrazovke výberu jednotiek SKU a prečo ukončil výber jednotiek SKU.  Tieto údaje sa používajú na porozumenie používaniu výberu SKU a optimalizáciu funkcie nakupovania v aplikácii v budúcich verziách.

Zhromažďujú sa tieto polia:

- **entryPoint** – reťazec – tlačidlo/tok spracovania, ktorým sa zobrazuje platobná stena. Napríklad „Premium Upgrade Button” alebo „First Run Flow”.

- **exitReason** – reťazec – dôvod ukončenia výberu jednotky SKU. Napríklad „BuyButton“, „CloseButton“

- **isFRE** – boolovská hodnota – zobrazuje sa prostredie prvého spustenia alebo bežné používateľské rozhranie?

- **userDuration** – double – čas v milisekundách, ktorý používateľ strávil vo výbere SKU


#### <a name="officelivepersonacardconfigurationsetaction"></a>Office.LivePersonaCard.ConfigurationSetAction

Prihlásime sa, keď sa bude používateľ nachádzať v aplikácii, ktorá načíta kartu osoby pri očakávaní, že používateľ otvorí živú kartu osoby.  Údaje sa používajú na určenie toho, či sa karta načíta správne. 

Zhromažďujú sa tieto polia: 

- **Data.accountType** – označuje, či používateľ patrí k organizácii alebo spotrebiteľovi.

- **Data.appContextId** – náhodne vygenerovaný identifikátor používaný na identifikáciu rôznych kont v tej istej aplikácii.

- **Data.AppInfo.Name** – názov používanej služby (karta profilu)

- **Data.AppInfo_Id** – názov hostiteľskej aplikácie

- **Data.AppInfo_Version** – verzia hostiteľskej aplikácie

- **Data.cardCorrelationId** – globálne jedinečný identifikátor karty osoby

- **Data.cardPersonaCorrelationId** – globálne jedinečný identifikátor konkrétnej osoby zobrazenej na karte

- **Data.cardCorrelationId** – globálne jedinečný identifikátor relácie aplikácie

- **Data.clientType** – typ zariadenia, v ktorom je aplikácia spustená.

- **Data.contextType** – označuje, v akom kontexte (aplikácii) sa karta spustila

- **Data.ecsConfigIds** – identifikátory verzií pre funkcie povolené na karte

- **Data.ecsTagId** – ID značiek pre funkcie

- **Data.eventId** – identifikátor názvu udalosti, napr. „LivePersonaCardRenderedAction“

- **Data.eventpriority** – hodnota enumerácie priority odoslania udalosti.

- **Data.feature** – používa sa na zoskupovanie rôznych udalostí tej istej funkcie (karta profilu)

- **Data.flights** – funkcie povolené na karte

- **Data.fromCache** – označuje, či boli údaje načítané z pamäte

- **Data.hasFinePointer** – označuje, či je v zariadení funkcia ukazovateľa myši

- **Data.hasHoverEvents** – označuje, či je v zariadení funkcia ukázania myšou

- **Data.immersiveProfileCorrelationId** – globálne jedinečný identifikátor relácie zobrazenia rozbaleného profilu

- **Data.offlineResolved** – označuje, či sa údaje načítavali v režime offline

- **Data.OTelJS.Version** – verzia zapisovača OTel

- **Data.personaCorrelationId** – globálne jedinečný identifikátor jedinečných osôb v relácii

- **Data.properties** – dodatočné metaúdaje zhromaždené pre každú udalosť nasledovne: *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

  - **cardCorrelationId** – duplikát poľa Data.appContextId vyššie
  - **cardPersonaCorrelationId** – duplikát poľa Data.cardCorrelationId vyššie.
  - **ClientTimeStamp** – čas v aplikácii, keď sa udalosť zaznamenala.
  - **consumerCorrelationId** – duplikát poľa Data.clientCorrelationId vyššie.

  - **externalAppSessionCorrelationId** – globálne jedinečný identifikátor pre aplikáciu na identifikáciu všetkých kariet osôb otvorených v tej istej čiastkovej relácii.

- **Data.region** – geografická oblasť backendovej služby karty profilu, ku ktorej je používateľ pripojený

- **Data.tenantAadObjectId** – nájomník, ku ktorému je priradené predplatné používateľa. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.type** – typ zaznamenanej udalosti, napr. sledovanie, chyba, udalosť.

- **Data.userAadObjectId** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft (duplikát poľa Data.UserInfo.Id).

- **Data.UserInfo.Id** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft.

- **Data.UserInfo.MsaId** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **Data.UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.userPuid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft (duplikát poľa Data.UserInfo.MsaId).

- **Data.version** – verzia služby (karta profilu).

- **Data.workloadCulture** – kultúra nastavená v hostiteľskej aplikácii

- **DeviceInfo_Id** – globálne jedinečný identifikátor zariadenia pre zariadenie

- **DeviceInfo_Make** – značka operačného systému.

- **DeviceInfo_Model** – model zariadenia.

- **DeviceInfo_OsName** – názov operačného systému zariadenia.

- **DeviceInfo_OsVersion** – verzia operačného systému.

- **DeviceInfo_SDKUid** – jednoznačne identifikuje zariadenie z perspektívy SDK telemetrie

#### <a name="officelivepersonacarduseractionsclosedexpandedpersonacard"></a>Office.LivePersonaCard.UserActions.ClosedExpandedPersonaCard

Táto udalosť sa zaznamená, keď používateľ zatvorí rozbalenú kartu osoby. Používa sa na pozorovanie kritických anomálií v mierach zlyhania zavretia funkcie Live Persona Card.

Zhromažďujú sa tieto polia:

- **AppInfo_Id** – názov hostiteľskej aplikácie.

- **AppInfo_Version** – verzia hostiteľskej aplikácie.

- **Data.appContextId** – náhodne vygenerovaný identifikátor používaný na identifikáciu rôznych kont v tej istej aplikácii.

- **Data.AppInfo.Name** – názov používanej služby (karta profilu)

- **Data.cardCorrelationId** – globálne jedinečný identifikátor karty osoby

- **Data.cardPersonaCorrelationId** – globálne jedinečný identifikátor konkrétnej osoby zobrazenej na karte

- **Data.cardCorrelationId** – globálne jedinečný identifikátor relácie aplikácie

- **Data.clientType** – typ zariadenia, v ktorom je aplikácia spustená, napr. Outlook_Win32

- **Data.eventId** – identifikátor názvu udalosti, napr. „LivePersonaCardRenderedAction“

- **Data.exportName** – človekom čitateľný názov udalosti akcie používateľa, napr. „ClosedExpandedPersonaCard“

- **Data.exportType** – kategória udalosti pre požiadavku na export GDPR

- **Data.externalAppSessionCorrelationId** – globálne jedinečný identifikátor pre aplikáciu na identifikáciu všetkých kariet osôb otvorených v tej istej čiastkovej relácii

- **Data.feature** – používa sa na zoskupovanie rôznych udalostí tej istej funkcie (karta profilu)

- **Data.immersiveProfileCorrelationId** – globálne jedinečný identifikátor relácie zobrazenia rozbaleného profilu

- **Data.OTelJS.Version** – verzia zapisovača OTel

- **Data.personaCorrelationId** – globálne jedinečný identifikátor jedinečných osôb v relácii

- **Data.properties** – dodatočné metaúdaje zhromaždené pre každú udalosť nasledovne: *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

   - **cardCorrelationId** – duplikát poľa Data.appContextId vyššie 
   - **cardPersonaCorrelationId** – duplikát poľa Data.cardCorrelationId vyššie.
   - **ClientTimeStamp** – čas výskytu udalosti v čase Unix Epoch
   - **consumerCorrelationId** – duplikát poľa Data.clientCorrelationId vyššie. 

- **Data.region** – geografická oblasť backendovej služby karty profilu, ku ktorej je používateľ pripojený

- **Data.tenantAadObjectId** – nájomník, ku ktorému je priradené predplatné používateľa. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.type** – typ zaznamenanej udalosti, napr. sledovanie, chyba, udalosť.

- **Data.userAadObjectId** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft (duplikát poľa Data.UserInfo.Id).

- **Data.UserInfo.Id** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft. 

- **Data.UserInfo.MsaId** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **Data.UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.UserPuid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft (duplikát poľa Data.UserInfo.MsaId).

- **Data.version** – verzia služby (karta profilu).

- **DeviceInfo_Id** – globálne jedinečný identifikátor zariadenia pre zariadenie

- **DeviceInfo_Make** – značka operačného systému.

- **DeviceInfo_Model** – model zariadenia.

- **DeviceInfo.NetworkCost** – označuje typ nákladov na sieť (účtované podľa objemu údajov, účtované podľa objemu údajov nad limit atď.)

- **DeviceInfo_OsName** – názov operačného systému zariadenia.

- **DeviceInfo_OsVersion** – verzia operačného systému.

- **PipelineInfo.ClientCountry** – kód krajiny odosielateľa, na základe neočistenej IP adresy klienta


#### <a name="officelivepersonacarduseractionsclosedpersonacard"></a>Office.LivePersonaCard.UserActions.ClosedPersonaCard

Zaznamenávame, keď používateľ zatvorí kartu osoby.  Údaje sa používajú na určenie toho, či sa karta zatvorí správne. 

Zhromažďujú sa tieto polia: 

- **BatchId** – globálne jedinečný identifikátor v prípade, že bola vytvorená množina požiadaviek

- **Data.appContextId** – náhodne vygenerovaný identifikátor používaný na identifikáciu rôznych kont v tej istej aplikácii.

- **Data.AppInfo.Name** – názov používanej služby (karta profilu)

- **Data.AppInfo_Id** – názov hostiteľskej aplikácie

- **Data.AppInfo_Version** – verzia hostiteľskej aplikácie

- **Data.cardCorrelationId** – globálne jedinečný identifikátor karty osoby

- **Data.cardPersonaCorrelationId** – globálne jedinečný identifikátor konkrétnej osoby zobrazenej na karte

- **Data.cardCorrelationId** – globálne jedinečný identifikátor relácie aplikácie

- **Data.clientType** – typ zariadenia, v ktorom je aplikácia spustená.

- **Data.eventId** – identifikátor názvu udalosti, napr. „LivePersonaCardRenderedAction“

- **Data.externalAppSessionCorrelationId** – globálne jedinečný identifikátor pre aplikáciu na identifikáciu všetkých kariet osôb otvorených v tej istej čiastkovej relácii

- **Data.feature** – používa sa na zoskupovanie rôznych udalostí tej istej funkcie (karta profilu)

- **Data.immersiveProfileCorrelationId** – globálne jedinečný identifikátor relácie zobrazenia rozbaleného profilu

- **Data.OTelJS.Version** – verzia zapisovača OTel

- **Data.personaCorrelationId** – globálne jedinečný identifikátor jedinečných osôb v relácii

- **Data.properties** – dodatočné metaúdaje zhromaždené pre každú udalosť nasledovne: *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

  - **ClientTimeStamp** – čas v aplikácii, keď sa udalosť zaznamenala.
  - **cardCorrelationId** – duplikát poľa Data.appContextId vyššie
  - **cardPersonaCorrelationId** – duplikát poľa Data.cardCorrelationId vyššie.
  - **consumerCorrelationId** – duplikát poľa Data.clientCorrelationId vyššie.

- **Data.region** – geografická oblasť backendovej služby karty profilu, ku ktorej je používateľ pripojený

- **Data.tenantAadObjectId** – nájomník, ku ktorému je priradené predplatné používateľa. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.type** – typ zaznamenanej udalosti, napr. sledovanie, chyba, udalosť.

- **Data.userAadObjectId** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft (duplikát poľa Data.UserInfo.Id).

- **Data.UserInfo.Id** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft.

- **Data.UserInfo.MsaId** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **Data.UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.UserPuid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft (duplikát poľa Data.UserInfo.MsaId).

- **Data.version** – verzia služby (karta profilu).

- **Data_hostAppRing** – zavádzací okruh karty osoby

- **Event_ReceivedTime** – čas zaznamenania udalosti v službe

#### <a name="officelivepersonacarduseractionsopenedexpandedpersonacard"></a>Office.LivePersonaCard.UserActions.OpenedExpandedPersonaCard

Zaznamenáva sa, keď používateľ otvorí rozbalenú kartu osoby. Používa sa na pozorovanie kritických anomálií v mierach zlyhania spustenia funkcie Live Persona Card.

Zhromažďujú sa tieto polia:

- **AppInfo_Id** – názov hostiteľskej aplikácie.

- **AppInfo_Version** – verzia hostiteľskej aplikácie.

- **Data.appContextId** – náhodne vygenerovaný identifikátor používaný na identifikáciu rôznych kont v tej istej aplikácii.

- **Data.AppInfo.Name** – názov používanej služby (karta profilu)

- **Data.cardCorrelationId** – globálne jedinečný identifikátor karty osoby

- **Data.cardPersonaCorrelationId** – globálne jedinečný identifikátor konkrétnej osoby zobrazenej na karte

- **Data.cardCorrelationId** – globálne jedinečný identifikátor relácie aplikácie

- **Data.clientScenario** – na identifikovanie funkcie v aplikácii, v ktorej sa otvorila karta osoby.

- **Data.clientType** – typ zariadenia, v ktorom je aplikácia spustená.

- **Data.eventId** – identifikátor názvu udalosti, napr. „LivePersonaCardRenderedAction“

- **Data.externalAppSessionCorrelationId** – globálne jednoznačný identifikátor pre aplikáciu na identifikáciu všetkých kariet osôb otvorených v tej istej čiastkovej relácii

- **Data.exportName** – človekom čitateľný názov udalosti akcie používateľa, napr. „OpenedPersonaCard“

- **Data.exportType** – kategória udalosti pre požiadavku na export GDPR

- **Data.feature** – používa sa na zoskupovanie rôznych udalostí tej istej funkcie (karta profilu)

- **Data.hasPersonalInsightRing** – prehľady v Office alebo LinkedIne môžu byť pre používateľa k dispozícii

- **Data.hostAppRing** – okruh, v ktorom bola aplikácia distribuovaná

- **Data.immersiveProfileCorrelationId** – globálne jedinečný identifikátor relácie zobrazenia rozbaleného profilu

- **Data.OTelJS.Version** – verzia zapisovača OTel

- **Data.personaCorrelationId** – globálne jedinečný identifikátor jedinečných osôb v relácii

- **Data.properties** – dodatočné metaúdaje zhromaždené pre každú udalosť nasledovne: *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

  - **cardCorrelationId** – duplikát poľa Data.appContextId vyššie 
  - **cardPersonaCorrelationId** – duplikát poľa Data.cardCorrelationId vyššie.
  - **consumerCorrelationId** – duplikát poľa Data.clientCorrelationId vyššie. 

- **Data.region** – geografická oblasť backendovej služby karty profilu, ku ktorej je používateľ pripojený

- **Data.section** – aktívna časť rozbalenej karty.

- **Data.tenantAadObjectId** – nájomník, ku ktorému je priradené predplatné používateľa. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.type** – typ zaznamenanej udalosti, napr. sledovanie, chyba, udalosť.

- **Data.userAadObjectId** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft (duplikát poľa Data.UserInfo.Id).

- **Data.UserInfo.Id** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft. 

- **Data.UserInfo.MsaId** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **Data.UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.UserPuid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft (duplikát poľa Data.UserInfo.MsaId).

- **Data.version** – verzia služby (karta profilu).

- **DeviceInfo_Id** – globálne jedinečný identifikátor zariadenia pre zariadenie

- **DeviceInfo_Make** – značka operačného systému.

- **DeviceInfo_Model** – model zariadenia.

- **DeviceInfo_OsName** – názov operačného systému zariadenia.

- **DeviceInfo_OsVersion** – verzia operačného systému.

- **DeviceInfo_SDKUid** – jednoznačne identifikuje zariadenie z perspektívy SDK telemetrie

- **NetworkCost** – označuje typ nákladov na sieť (účtované podľa objemu údajov, účtované podľa objemu údajov nad limit atď.).

- **NetworkCountry** – kód krajiny odosielateľa, na základe neočistenej IP adresy klienta.


#### <a name="officelivepersonacarduseractionsopenedpersonacard"></a>Office.LivePersonaCard.UserActions.OpenedPersonaCard

Zaznamenáva sa, keď používateľ otvorí kartu osoby. Používa sa na pozorovanie kritických anomálií v mierach zlyhania spustenia funkcie Live Persona Card.

Zhromažďujú sa tieto polia:

- **Data.appContextId** – náhodne vygenerovaný identifikátor používaný na identifikáciu rôznych kont v tej istej aplikácii.

- **Data.AppInfo.Name** – názov používanej služby (karta profilu)

- **Data.bandwidthEstimateMbps** – odhad efektívnej šírky pásma v Mbit/s.

- **Data.cardCorrelationId** – globálne jedinečný identifikátor karty osoby

- **Data.cardPersonaCorrelationId** – globálne jedinečný identifikátor konkrétnej osoby zobrazenej na karte

- **Data.cardCorrelationId** – globálne jedinečný identifikátor relácie aplikácie

- **Data.clientType** – typ zariadenia, v ktorom je aplikácia spustená.

- **Data.eventId** – identifikátor názvu udalosti, napr. „LivePersonaCardRenderedAction“

- **Data.exportName** – človekom čitateľný názov udalosti akcie používateľa, napr. „OpenedPersonaCard“

- **Data.exportType** – kategória udalosti pre požiadavku na export GDPR

- **Data.externalAppSessionCorrelationId** – globálne jedinečný identifikátor pre aplikáciu na identifikáciu všetkých kariet osôb otvorených v tej istej čiastkovej relácii

- **Data.feature** – používa sa na zoskupovanie rôznych udalostí tej istej funkcie (karta profilu)

- **Data.hasPersonalInsightRing** – prehľady v Office alebo LinkedIne môžu byť pre používateľa k dispozícii

- **Data.hostAppRing** – okruh, v ktorom bola aplikácia distribuovaná

- **Data.immersiveProfileCorrelationId** – globálne jedinečný identifikátor relácie zobrazenia rozbaleného profilu

- **Data.OTelJS.Version** – verzia zapisovača OTel

- **Data.personaCorrelationId** – globálne jedinečný identifikátor jedinečných osôb v relácii

- **Data.properties** – dodatočné metaúdaje zhromaždené pre každú udalosť nasledovne. *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

    - **cardCorrelationId** – duplikát poľa Data.appContextId vyššie 
    - **cardPersonaCorrelationId** – duplikát poľa Data.cardCorrelationId vyššie.
    - **consumerCorrelationId** – duplikát poľa Data.clientCorrelationId vyššie. 
    - **networkEffectiveType** – efektívny typ sieťového pripojenia, napr. „slow-2g Online“ na identifikáciu, či je používateľ v čase zobrazenia karty osoby pripojený na internet.
    - **networkType** – typ sieťového pripojenia používaného zariadenia.
    - **roundTripEstimateMs** – odhadovaný efektívny čas výmeny údajov aktuálneho pripojenia v milisekundách.

- **Data.region** – geografická oblasť backendovej služby karty profilu, ku ktorej je používateľ pripojený

- **Data.tenantAadObjectId** – nájomník, ku ktorému je priradené predplatné používateľa. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.type** – typ zaznamenanej udalosti, napr. sledovanie, chyba, udalosť.

- **Data.userAadObjectId** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft (duplikát poľa Data.UserInfo.Id).

- **Data.UserInfo.Id** – globálne jedinečný identifikátor používateľa pre podnikové konto Microsoft. 

- **Data.UserInfo.MsaId** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft.

- **Data.UserInfo.OMSTenantId** – nájomník, s ktorým je predplatné používateľa spojené. Umožňuje klasifikovať problémy a identifikovať, či je problém rozšírený všeobecne alebo izolovaný v určitej množine používateľov alebo konkrétnom nájomníkovi.

- **Data.UserPuid** – globálne jedinečný identifikátor používateľa pre spotrebiteľské konto Microsoft (duplikát poľa Data.UserInfo.MsaId).

- **Data.version** – verzia služby (karta profilu).

- **Data.viewType** – definuje typ zobrazenej karty profilu.

- **Data.wasOpenedAsCompactCard** – používa sa na identifikáciu, či karta bola pôvodne otvorená v kompaktnom zobrazení.

- **NetworkCost** – označuje typ nákladov na sieť (účtované podľa objemu údajov, účtované podľa objemu údajov nad limit atď.).

- **NetworkCountry** – kód krajiny odosielateľa, na základe neočistenej IP adresy klienta.

#### <a name="officemanageabilityclient-fetchpolicyprechecks"></a>Office.Manageability.Client Fetch.PolicyPreChecks

Veľmi dôležitá telemetria na sledovanie zlyhania\\úspešnosti predbežného kontrolného overenia načítania politiky cloudu. ExitReason obsahuje mapu enumerátora k stavu predbežnej kontroly, kde došlo k zlyhaniu.

Zhromažďujú sa tieto polia:

  - **Data.ExitReason** – hodnota enumerátora s informáciou o dôvode ukončenia, ak predbežná kontrola zlyhala

  - **Data.Log** – hlásenie vlastného denníka s informáciou o úspešnosti alebo neúspešnosti predbežnej kontroly

#### <a name="officemanageabilityclientfetchandapplypolicy"></a>Office.Manageability.Client.Fetch.AndApplyPolicy

Veľmi dôležitá telemetria na sledovanie zlyhania\\úspešnosti spustenia načítania politiky cloudu z aplikácie. ExitReason obsahuje mapu enumerátora k dôvodu zlyhania.

Zhromažďujú sa tieto polia:

  - **Data.ExitReason** – hodnota enumerátora s informáciou o dôvode ukončenia, ak predbežná kontrola zlyhala

  - **Data.Log** – hlásenie vlastného denníka s informáciou o úspešnosti alebo neúspešnosti predbežnej kontroly

#### <a name="officeofficemobilepdfviewerpdffileopenmeasurements"></a>Office.OfficeMobile.PdfViewer.PdfFileOpenMeasurements

Táto udalosť sa zhromažďuje pre aplikáciu Office pre iOS a zaznamenáva, či prebieha operácia otvorenia súboru. Zhromažďujeme tieto údaje, aby ste zabezpečili spoľahlivé otváranie všetkých súborov v aplikácii. 

Zhromažďujú sa tieto polia:

- **Data_Doc_ActivationFQDN** – názov domény aplikácie poskytovateľa pre scenár aktivácie súboru (zaznamenávajú sa len informácie o aplikácii 1. strany).

- **Data_Doc_CreateTelemetryReason** – telemetrický dôvod vytvorenia PDF súboru (napr. vytvorenie zo skenu, pomocou akcie „obrázok do PDF“, pomocou akcie „dokument do PDF“ atď.)

- **Data_Doc_DownloadDurationms** – trvanie stiahnutia cloudového PDF súboru.

- **Data_Doc_DownloadEndTime** – časová pečiatka konca sťahovania cloudového súboru.

- **Data_Doc_DownloadStartTime** – časová pečiatka začiatku sťahovania cloudového súboru.

- **Data_Doc_FileOpSessionID** – jedinečný identifikátor pre reláciu dokumentu.

- **Data_Doc_Location** – miesto, kde sa nachádza súbor (lokálne, ODSP, iCloud, aplikácia pre súbory tretej strany, wopi).

- **Data_Doc_OpenCompletionTime** – časová pečiatka konca operácie otvorenia PDF súboru.

- **Data_Doc_OpenDurationms** – trvanie otvorenia PDF súboru v milisekundách.

- **Data_Doc_OpenStartTime** – časová pečiatka začiatku operácie otvorenia PDF súboru.

- **Data_Doc_TelemetryReason** – dôvod telemetrie otvorenej udalosti (napr. otvorenie zo služby MRU alebo prehľadávanie, aktivácia súborov, aktivácia protokolu atď.).

- **Doc_RenderDurationms** – trvanie vykreslenia PDF súboru


#### <a name="officeofficemobilepdfviewerpdffileoperations-on-android"></a>Office.OfficeMobile.PdfViewer.PdfFileOperations (v Androide)

Táto udalosť sa zhromažďuje pre aplikáciu balíka Office pre Android. Zaznamená, keď sa vykoná operácia otvorenia, zatvorenia alebo uloženia .pdf súboru, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách .pdf súborov. Táto akcia nám umožňuje zachovávať fungovanie operácií otvorenia, zatvorenia a uloženia .pdf súborov podľa očakávaní a zlepšiť výkon operácií s .pdf súbormi.

Zhromažďujú sa tieto polia:

- **Data_Doc_FileOpSessionID** – jedinečný identifikátor pre reláciu dokumentu

- **Data_ErrorCode** -- chyba v prípade zlyhania otvorenia súboru, zlyhania sťahovania alebo zrušenia sťahovania

- **Data_ErrorMessage** - príslušný kód hlásenia chyby

- **Data_FailureReason** -- v prípade zlyhania otvorenia tieto enumerátory definujú dôvod zlyhania.

- **Data_FileGUID** – globálny identifikátor súboru, ktorý je generovaný náhodne

- **Data_FileLocation** - druh umiestnenia súboru, napr. lokálne, ODSP, iCloud atď.

- **Data_FileOpenEntryPoint** - vstupný bod pre otvorenie súboru

- **Data_FileSize** – veľkosť súboru, na ktorom sa operácia vykonáva

- **Data_NetworkRequestErrorResponse** – odozva chyby siete, ktorá zodpovedá kódu chyby.

- **Data_NetworkRequestStage** – fáza chyby v prípade stiahnutia súboru PDF v cloude.

- **Data_OpenMode** – v ktorom režime bol PDF súbor otvorený, napr. 0: režim zobrazenia, 2: režim podpisu

- **Data_PageCount** – počet strán v PDF súbore.

- **Data_PasswordProtected** – značka, ktorá označuje, či súbor je chránený heslom alebo nie.

- **Data_ProviderApp** – aktuálna aplikácia poskytovateľa v prípade iba aktivácie súboru 

- **Data_ReadOnly** – značka, ktorá označuje, či súbor je len na čítanie alebo nie.

- **Data_Result** – stav vykonávanej operácie, napr. true:úspech, false:zlyhanie

- **Data_Type** – typ operácie súboru (otvorenie, zatvorenie alebo uloženie) 

#### <a name="officeofficemobilepdfviewerpdffileoperations-on-ios"></a>Office.OfficeMobile.PdfViewer.PdfFileOperations (on iOS)

Táto udalosť sa zhromažďuje pre aplikáciu Office pre iOS. Zaznamená, keď sa vykoná operácia otvorenia, zatvorenia alebo uloženia .pdf súboru, a používa sa na pochopenie a uprednostňovanie používateľských skúseností na základe informácií o operáciách .pdf súborov. Táto akcia nám umožňuje zachovávať fungovanie operácií otvorenia, zatvorenia a uloženia .pdf súborov podľa očakávaní a zlepšiť výkon operácií s .pdf súbormi. 

- **Data_Doc_FileOpSessionID** – jedinečný identifikátor pre reláciu dokumentu 

- **Data_ErrorCode** – chyba v prípade zlyhania otvorenia súboru, zlyhania sťahovania alebo zrušenia sťahovania 

- **Data_ErrorMessage** – príslušný kód hlásenia chyby 

- **Data_FailureReason** -- v prípade zlyhania otvorenia tieto enumerátory definujú dôvod zlyhania. 

- **Data_FileGUID** – globálny identifikátor súboru, ktorý je generovaný náhodne

- **Data_FileLocation** - druh umiestnenia súboru (lokálne, ODSP, iCloud atď.) 

- **Data_FileOpenEntryPoint** – vstupný bod pre otvorenie súboru 

- **Data_FileSize** – veľkosť súboru, na ktorom sa operácia vykonáva 

- **Data_OpenMode** – v ktorom režime bol PDF súbor otvorený (0: režim zobrazenia, 2: režim podpisu) 

- **Data_PageCount** – počet strán v PDF súbore.

- **Data_PasswordProtected** – značka, ktorá označuje, či súbor je chránený heslom alebo nie. 

- **Data_ProviderApp** – aktuálna aplikácia poskytovateľa v prípade iba aktivácie súboru 

- **Data_ReadOnly** – značka, ktorá označuje, či súbor je len na čítanie alebo nie.

- **Data_Result** – stav vykonávanej operácie (true:úspech, false:zlyhanie) 

- **Data_Type** – typ operácie súboru (otvorenie, zatvorenie alebo uloženie)


#### <a name="officeonenoteandroidappnavigationnavigationuistatechanged"></a>Office.OneNote.Android.App.Navigation.NavigationUIStateChanged

*[Táto udalosť sa predtým nazývala OneNote.App.Navigation.NavigationUIStateChanged.]*

Táto udalosť zhromažďuje kritický signál, ktorý sa používa na zaistenie, aby používatelia OneNotu mohli úspešne navigovať v aplikácii.  Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. 

Zhromažďujú sa tieto polia: 

- **IS_SPANNED** – označuje, či je aplikácia v rozloženom režime. Toto sa špeciálne zaznamenáva pre skladacie zariadenia.

- **NEW_STATE** – označuje stav aplikácií hneď po navigácii

- **OLD_STATE** – označuje stav aplikácií tesne pred navigáciou

#### <a name="officeonenoteandroidcanvaspageopened"></a>Office.OneNote.Android.Canvas.PageOpened

*[Táto udalosť sa predtým nazývala OneNote.Canvas.PageOpened.]*

Signál, ktorý sa používa na zaznamenanie, keď sa otvorí strana.  Telemetria sa používa na sledovanie, zisťovanie a opravu všetkých problémov spôsobených pri otvorení strany vo OneNote.

Zhromažďujú sa tieto polia: 

- **JOT_ID** – objekt otvorenej strany

- **TIME_TAKEN_IN_MS** – čas potrebný na otvorenie strany

#### <a name="officeonenoteandroidcapturenewnotenewnotetaken"></a>Office.OneNote.Android.Capture.NewNote.NewNoteTaken

*[Táto udalosť sa predtým nazývala OneNote.Capture.NewNote.NewNoteTaken.]*

Tento signál sa používa na zabezpečenie toho, aby sa po prihlásení používateľa do aplikácie OneNote pre Android správne zriadili poznámkové bloky a aby používateš úspešne vytvoril novú poznámku.  Používa sa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby.

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeonenoteandroidlenssdkofficelenslaunched"></a>Office.OneNote.Android.LensSDK.OfficeLensLaunched

*[Táto udalosť sa predtým nazývala OneNote.LensSDK.OfficeLensLaunched.]*

Táto udalosť zhromažďuje kritický signál, ktorý sa používa na zaistenie, že OfficeLens sa spustí správne.  Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. 

Zhromažďujú sa tieto polia: 

- **CAPTURE_MODE** – označuje, v ktorom režime bol OfficeLens spustený.  Môže to byť predvolený režim, úprava, rýchle vloženie alebo import videa.

- **ERROR_CODE** – označuje kód chyby spustenia v prípade, že pri spúšťaní došlo k chybe.

- **IMAGE_COUNT** – označuje počet zhotovených obrázkov

- **LAUNCH_REASON** – označuje tok, pod ktorým sa OfficeLens spustil. Môže to byť cez obrazovku uzamknutia alebo prostredníctvom možností fotoaparátu alebo galérie v StickyNotes alebo cez OneNote Canvas atď.

#### <a name="officeonenoteandroidmessagebarmessagebarclicked"></a>Office.OneNote.Android.MessageBar.MessageBarClicked

*[Táto udalosť sa predtým nazývala OneNote.MessageBar.MessageBarClicked.]*

Signál, ktorý sa používa na označenie všetkých problémov, ktoré sa vyskytli počas používania panela hlásení.  Telemetria sa používa na sledovanie, zisťovanie a opravu všetkých problémov spôsobených počas používania panela hlásení.

Zhromažďujú sa tieto polia: 

- **Message_Bar_Type** – vráti, či používateľ používa starý alebo nový panel hlásení

- **Message_Type** – vráti ID chybového hlásenia

#### <a name="officeonenoteandroidstickynotesnotecreated"></a>Office.OneNote.Android.StickyNotes.NoteCreated
 
Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov Rýchlych poznámok vytvárať poznámky v aplikácii.   Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu vytvoriť poznámku, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **IsExportable** – príznak označujúci, či táto udalosť bola výsledkom akcie používateľa alebo nie. Mala by byť nastavená na hodnotu True, pretože NoteCreated je akcia spustená používateľom.

- **NoteLocalId** – rozlíšiteľný jedinečný identifikátor priradený poznámke, keď používateľ vytvorí poznámku v rámci aplikácii.

- **StickyNotes-SDKVersion** – číslo verzie označujúce verziu aplikácie Rýchle poznámky, ktorú používateľ používa. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby sa správne určila jeho priorita.


#### <a name="officeonenoteandroidstickynotesnoteviewed"></a>Office.OneNote.Android.StickyNotes.NoteViewed

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov Rýchlych poznámok zobrazovať poznámky v aplikácii.  Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu zobraziť svoje poznámky, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **HasImages** – príznak označujúci, či zobrazená poznámka obsahuje poznámku.

- **IsExportable** – príznak označujúci, či táto udalosť bola výsledkom akcie používateľa alebo nie. Mala by byť nastavená na hodnotu True, pretože NoteViewed je akcia spustená používateľom.

- **NoteLocalId** – rozlíšiteľný jedinečný identifikátor priradený poznámke, keď používateľ vytvorí poznámku v rámci aplikácii.

- **StickyNotes-SDKVersion** – číslo verzie označujúce verziu aplikácie Rýchle poznámky, ktorú používateľ používa. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby sa správne určila jeho priorita.


#### <a name="officeonenotecanvasinkinkstrokelogger"></a>Office.OneNote.Canvas.Ink.InkStrokeLogger 

Táto udalosť sa používa na zisťovanie a diagnostiku chyby s vysokou frekvenciou, na ktorú používateľ narazí pri používaní funkcie písania rukou.  Táto možnosť sa použije na určenie najvhodnejšieho režimu opravy tohto problému. 

Zhromažďujú sa tieto polia:

- **CurrentCanvasZoomFactor** – aktuálny faktor priblíženia plátna.

- **CurrentNotebook** – identifikátor aktuálneho aktívneho poznámkového bloku.

- **CurrentPage** – identifikátor aktuálnej aktívnej strany.

- **CurrentSection** – identifikátor aktuálnej aktívnej sekcie.

- **DefaultCanvasZoomFactor** – predvolený faktor priblíženia plátna.

- **InkStrokeCount** – celkový počet ťahov perom od posledného záznamu denníka.

- **InkStrokeWithLayerInkEffect** – počet ťahov perom s efektom vrstveného písania rukou od posledného záznamu denníka.

- **InkStrokeWithoutPressureCount** – počet ťahov perom bez tlaku od posledného záznamu denníka.

- **InkStrokeWithPencilInkEffect** – počet ťahov perom s efektom písania ceruzkou od posledného záznamu denníka.

- **InkStrokeWithTilt** – počet ťahov perom s naklonením od posledného záznamu denníka.

#### <a name="officeonenotenavigationcreatepage"></a>Office.OneNote.Navigation.CreatePage

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu vytvárať strany vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia stranu nemôžu vytvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **IsAtSectionEnd** – označuje, či sa na konci sekcie vytvorí nová strana alebo nie.

- **IsBlank** – označuje, či je nová strana prázdna alebo vytvorená pomocou šablóny.

- **IsRecentsView** – označuje, či je strana vytvorená z posledných položiek alebo nie.

- **NavView** – označuje, či je strana vytvorená z navigačného zobrazenia alebo nie.

- **NoteType** – označuje typ strany (rýchla poznámka, zoznam alebo fotografia).

- **QuickNoteType** – označuje typ strany (rýchla poznámka, zoznam alebo fotografia).

- **RailState** – označuje stav navigačnej časti OneNotu pri vytváraní strany.

- **Trigger** – označuje vstupný bod, v ktorom sa spustí akcia vytvorenia strany.

- **TriggerInfo** – označuje ďalšie informácie týkajúce sa spúšťača.


#### <a name="officeonenotenavigationcreatesection"></a>Office.OneNote.Navigation.CreateSection

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu vytvárať sekcie vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia stranu nemôžu vytvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **NotebookID** – jedinečný identifikátor poznámkového bloku.

- **SectionID** – jedinečný identifikátor vytvorenej sekcie.

- **Trigger** – označuje vstupný bod, v ktorom sa spustí akcia vytvorenia sekcie.

- **TriggerInfo** – označuje ďalšie informácie týkajúce sa spúšťača.


#### <a name="officeonenotenavigationnavigate"></a>Office.OneNote.Navigation.Navigate

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu prechádzať medzi stranami vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu prechádzať medzi stranami, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **FromNotebook** – jedinečný identifikátor poznámkového bloku.

- **FromPage** – jedinečný identifikátor strany.

- **FromSection** – jedinečný identifikátor sekcie.

- **FromSectionGroup** – jedinečný identifikátor skupiny sekcií.

- **IsCurrentUserEduStudent** – označuje, či má aktuálny používateľ rolu študenta vo vzdelávacom poznámkovom bloku alebo nie.

- **IsEduNotebook** – označuje, či sa aktuálna strana nachádza vo vzdelávacom poznámkovom bloku alebo nie.

- **IsEduNotebookReadOnlyPage** – označuje, či aktuálna strana je stranou iba na čítanie vo vzdelávacom poznámkovom bloku alebo nie.

- **ToNotebook** – jedinečný identifikátor poznámkového bloku.

- **ToPage** – jedinečný identifikátor strany.

- **ToSection** – jedinečný identifikátor sekcie.

- **ToSectionGroup** – jedinečný identifikátor skupiny sekcií.


#### <a name="officeonenotenotebookmanagementcreatenotebook"></a>Office.OneNote.NotebookManagement.CreateNotebook

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu vytvárať poznámkové bloky vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia poznámkové bloky nemôžu vytvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:
    
- **NotebookID** – jedinečný identifikátor poznámkového bloku.


#### <a name="officeonenotenotebookmanagementopennotebook"></a>Office.OneNote.NotebookManagement.OpenNotebook

Kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov OneNotu otvárať poznámkové bloky vo OneNote.  Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia poznámkové bloky nemôžu otvoriť, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

-  **NotebookID** – jedinečný identifikátor poznámkového bloku.

    
#### <a name="officeonenotesearchsearch"></a>Office.OneNote.Search.Search

Kritický signálny identifikátor, ktorý sa používa na sledovanie schopnosti používateľov OneNotu vyhľadať informácie v rámci tisícok strán a poznámkových blokov.   Telemetria používaná na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia informácie v poznámkových blokoch nemôžu vyhľadať, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **PageSearchResultCount** – označuje počet výsledkov vyhľadávania, ktoré sa našli v režime vyhľadávania strán.

-  **PageTimeToFirstResultInMs** – označuje čas OneNotu potrebný na vyhľadanie prvej zhody v režime vyhľadávania strán.
    
-  **PageTimeToLastResultInMs** – označuje čas OneNotu potrebný na vyhľadanie poslednej zhody v režime vyhľadávania strán.

-  **PageTimeToMedianResultInMs** – označuje medián času OneNotu potrebného na vyhľadanie všetkých zhôd v režime vyhľadávania strán.

-  **SearchResultCount** – označuje počet nájdených výsledkov vyhľadávania.

-  **TagSearchResultCount** – označuje počet výsledkov vyhľadávania, ktoré sa našli v režime vyhľadávania značiek.

-  **TagTimeToFirstResultInMs** – označuje čas OneNotu potrebný na vyhľadanie prvej zhody v režime vyhľadávania značiek.

-  **TagTimeToLastResultInMs** – označuje čas OneNotu potrebný na vyhľadanie poslednej zhody v režime vyhľadávania značiek.

-  **TagTimeToMedianResultInMs** – označuje medián času OneNotu potrebného na vyhľadanie všetkých zhôd v režime vyhľadávania značiek.

-  **TimeToFirstResultInMs** – označuje čas OneNotu potrebný na vyhľadanie prvej zhody.

-  **TimeToLastResultInMs** – označuje čas OneNotu potrebný na vyhľadanie poslednej zhody.

-  **TimeToMedianResultInMs** – označuje medián času OneNotu potrebného na vyhľadanie všetkých zhôd.

### <a name="officeonenotesigscriticalerrorencountered"></a>Office.OneNote.SIGS.CriticalErrorEncountered

Táto udalosť zachytáva kritický signál, ktorý sa používa na sledovanie stavu služby Signal Ingestion Service (SIGS) zapisovaním každého výskytu kritickej chyby do denníka. Kritické chyby môžu blokovať celú službu SIGS a pomáha nám to zachytiť akékoľvek takéto problémy hneď, ako sa vyskytnú používateľom. 

Bez toho budeme závisieť od toho, aby nám samotní používatelia hlásili problémy, s ktorými sa stretávajú. Pri absencii takejto telemetrie by bol čas odozvy pre takéto problémy oveľa vyšší.

Zhromažďujú sa tieto polia: 

- **ErrorCode** – kód problému, ktorý sa vyskytol používateľovi.


#### <a name="officeonenotestickynotesnotecreated-on-ios-onenotestickynotesnotecreated-on-android"></a>Office.OneNote.StickyNotes.NoteCreated (v iOS), OneNote.StickyNotes.NoteCreated (v Androide)

Toto je kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov Rýchlych poznámok vytvárať poznámky v aplikácii.  Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu vytvoriť poznámku, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **NoteLocalId** – rozlíšiteľný jedinečný identifikátor priradený poznámke, keď používateľ vytvorí poznámku v rámci aplikácii.

- **IsExportable** – príznak označujúci, či táto udalosť bola výsledkom akcie používateľa alebo nie. Mala by byť nastavená na hodnotu True, pretože NoteCreated je akcia spustená používateľom.

- **StickyNotes-SDKVersion** – číslo verzie označujúce verziu aplikácie Rýchle poznámky, ktorú používateľ používa. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby sa správne určila jeho priorita.


#### <a name="officeonenotestickynotesnoteviewed-on-ios-onenotestickynotesnoteviewed-on-android"></a>Office.OneNote.StickyNotes.NoteViewed (v iOS), OneNote.StickyNotes.NoteViewed (v Androide)

Toto je kritický signál, ktorý sa používa na monitorovanie schopnosti používateľov Rýchlych poznámok vytvárať poznámky v aplikácii.  Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu vytvoriť poznámku, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:

- **HasImages** – príznak označujúci, či zobrazená poznámka obsahuje poznámku.

- **IsExportable** – príznak označujúci, či táto udalosť bola výsledkom akcie používateľa alebo nie. Mala by byť nastavená na hodnotu True, pretože NoteViewed je akcia spustená používateľom.

- **NoteLocalId** – rozlíšiteľný jedinečný identifikátor priradený poznámke, keď používateľ vytvorí poznámku v rámci aplikácii.

- **StickyNotes-SDKVersion** – číslo verzie označujúce verziu aplikácie Rýchle poznámky, ktorú používateľ používa. Umožňuje identifikovať, ktoré verzie produktu zobrazujú problém, aby sa správne určila jeho priorita.


#### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
Táto udalosť zaznamenáva výsledok synchronizácie poznámkového bloku. Používa sa na zistenie počtu jedinečných cieľov synchronizácie vo výpočte skóre synchronizácie OneNotu.
 
Zhromažďujú sa tieto polia:

- **CachedError_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby vo vyrovnávacej pamäti a/alebo dôvodu, prečo sa vyskytla.
    
- **CachedError_Description** – popis chyby vo vyrovnávacej pamäti.

- **CachedError_Tag** – označuje, ktoré miesto v kóde vyhodí chybu vo vyrovnávacej pamäti.

- **CachedError_Type** – typ chyby vo vyrovnávacej pamäti, napríklad Win32Error atď.

- **ExecutionTime** – čas v milisekundách, ktorý bol potrebný na replikovanie poznámkového bloku.

- **Gosid** – ID miesta globálneho objektu.

- **IdentityType** – typ identity, napríklad Windows Live, Org ID atď.

- **InitialReplicationInSession** – označuje, či je táto replikácia prvou replikáciou poznámkového bloku po otvorení alebo nie.

- **IsBackgroundSync** – označuje, či ide o synchronizáciu na pozadí alebo nie.

- **IsCachedErrorSuppressed** – označuje, či je chyba vo vyrovnávacej pamäti potlačená alebo nie.

- **IsCachedErrorUnexpected** – označuje, či je chyba vo vyrovnávacej pamäti neočakávaná alebo nie.

- **IsNotebookErrorSuppressed** – označuje, či je chyba synchronizácie úrovne poznámkového bloku potlačená alebo nie.

- **IsNotebookErrorUnexpected** – označuje, či je chyba synchronizácie úrovne poznámkového bloku neočakávaná alebo nie.

- **IsSectionErrorSuppressed** – označuje, či je chyba synchronizácie sekcie potlačená alebo nie.

- **IsSectionErrorUnexpected** – označuje, či je chyba synchronizácie sekcie neočakávaná alebo nie.

- **IsUsingRealtimeSync** – označuje, či synchronizácia poznámkového bloku používa modernú synchronizáciu obsahu strany alebo nie.

- **LastAttemptedSync** – časová pečiatka pri poslednom pokuse o synchronizáciu poznámkového bloku.

- **LastBackgroundSync** – časová pečiatka pri pokuse o najnovšiu synchronizáciu na pozadí.

- **LastNotebookViewedDate** – dátum posledného zobrazenia poznámkového bloku.

- **LastSuccessfulSync** – časová pečiatka poslednej úspešnej synchronizácie poznámkového bloku.

- **NeedToRestartBecauseOfInconsistencies** – označuje, či je potrebné reštartovať synchronizáciu z dôvodu nezrovnalostí alebo nie.

- **NotebookErrorCode** – kód chyby synchronizácie úrovne poznámkového bloku uložený v mieste grafu v poznámkovom bloku.

- **NotebookId** – ID poznámkového bloku.

- **NotebookType** – typ poznámkového bloku.

- **ReplicatingAgainBecauseOfInconsistencies** – označuje, či sa synchronizácia reštartuje z dôvodu nezrovnalostí alebo nie.

- **SectionError_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby synchronizácie sekcie a/alebo dôvodu, prečo sa vyskytla.

- **SectionError_Description** – popis chyby synchronizácie sekcie.

- **SectionError_Tag** – označuje, ktoré miesto v kóde vyhodí chybu synchronizácie sekcie.

- **SectionError_Type** – typ chyby synchronizácie sekcie, napríklad Win32Error atď.

- **Success** – označuje, či je synchronizácia poznámkového bloku úspešná alebo nie.

- **SyncDestinationType** – typ cieľa synchronizácie, ako je OneDrive alebo SharePoint Online.

- **SyncId** – číslo jedinečné pre každú synchronizáciu poznámkového bloku.

- **SyncWasFirstInSession** – označuje, či je táto synchronizácia prvou synchronizáciou v aktuálnej relácii.

- **SyncWasUserInitiated** – označuje, či je táto synchronizácia iniciovaná používateľom alebo nie.

- **TenantId** – ID nájomníka SharePointu.

- **TimeSinceLastAttemptedSync** – čas od posledného pokusu o synchronizáciu poznámkového bloku.

- **TimeSinceLastSuccessfulSync** – čas od poslednej úspešnej synchronizácie poznámkového bloku.


#### <a name="officeonenotesystemapplifecycleapplaunch"></a>Office.OneNote.System.AppLifeCycle.AppLaunch

Kritický signál sa používa na zaistenie, aby používatelia OneNotu mohli úspešne spustiť aplikáciu. Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak používatelia nemôžu spustiť aplikáciu v okne výkonu, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia:     Žiadne

#### <a name="officeoutlookdesktopaccountconfigurationcreateaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.CreateAccountResult

Výsledok pridania konta do Outlooku v novom profile v zobrazení Office Backstage alebo v dialógovom okne nastavenia konta. Údaje sú aktívne monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním.

Zhromažďujú sa tieto polia:

  - **AccountCreationResult** – výsledok (úspešnosť, zlyhanie, zrušenie atď.) pridania konta do Outlooku.

  - **AccountCreationTime** – čas trvania pokusu o vytvorenie konta

  - **AccountInfoSource** – zdroj nastavení konta (napr. automatická konfigurácia, GuessSmart, automatické zisťovanie atď.)

  - **AccountType** – typ konta, ktoré sa konfiguruje.

  - **HashedEmailAddress** – hashovaná e-mailová adresa

  - **ShowPasswordPageFlightEnabled** – indikátor povolenia skupiny funkcií ShowPopImapPasswordPage

#### <a name="officeoutlookdesktopaccountconfigurationrepairaccountresult"></a>Office.Outlook.Desktop.AccountConfiguration.RepairAccountResult

Výsledok opravy konta alebo zmeny rozšíreného nastavenia konta. Údaje sú aktívne monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Keďže ide o nové (refaktorované) prostredie, chceme si byť istí, že je to dobré.

Zhromažďujú sa tieto polia:

  - **AccountInfoSource** – zdroj informácií o konte pre konto použité pri pokuse o opravu

  - **AccountType** – typ konta, pre ktoré sa vykonal pokus o opravu konta

  - **HashedEmailAddress** – hashovaná e-mailová adresa

  - **ManualRepairRequested** – indikátor požadovanej opravy

  - **Result** – výsledok pokusu o opravu konta. Príklad: „Success“ (úspešný pokus) alebo „Fail\_SaveChangesToAccount“ (neúspešný pokus)

#### <a name="officeoutlookdesktopaccountconfigurationupdatepasswordresult"></a>Office.Outlook.Desktop.AccountConfiguration.UpdatePasswordResult

Výsledok aktualizácie hesla konta v rozbaľovacej ponuke nastavenia konta. Údaje sú aktívne monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Keďže ide o nové (refaktorované) prostredie, chceme si byť istí, že je to dobré.

Zhromažďujú sa tieto polia:

  - **AccountType** – typ konta, pre ktoré sa vykonal pokus o aktualizáciu hesla

  - **HashedEmailAddress** – hashovaná e-mailová adresa

  - **Result** – výsledok pokusu o aktualizáciu hesla. Príklad: „Success“ (úspešný pokus) alebo „Fail\_AllowLessSecureAppsDisabled“ (neúspešný pokus)


#### <a name="officeoutlookdesktopstorescreatenewstore"></a>Office.Outlook.Desktop.Stores.CreateNewStore

Zhromažďuje výsledok vytvorenia nového ukladacieho priestoru (vrátane typu a verzie) a kód výsledku. Aktívne monitorujeme túto udalosť, aby sme mohli sledovať stav schopnosti používateľa synchronizovať a ukladať poštu lokálne, archivovať e-maily (vo formáte súboru PST) alebo používať skupiny.

Zhromažďujú sa tieto polia:

  - **Štandardná aktivita HVA** s vlastnou údajovou časťou

  - **StoreType** – typ vytvoreného ukladacieho priestoru, OST/PST/NST

  - **StoreVersion** – verzia vytvoreného ukladacieho priestoru, Small/Large/Tardis

#### <a name="officeoutlookmacaccountaddworkflow"></a>Office.Outlook.Mac.AccountAddWorkflow

Výsledok pridania konta v Outlooku. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním. 

Zhromažďujú sa tieto polia:

- **AccountConfigMethod** – metóda konfigurácie konta.

- **AccountType** – typ konta, ktoré sa konfiguruje.

- **AccountWorkflowSession** – relácia s pokusom o vykonanie pracovného postupu konta.

- **SessionDuration** – trvanie relácie. 

- **ThreadId** – identifikátor vlákna.


#### <a name="officeoutlookmacaccountonboardingflow"></a>Office.Outlook.Mac.AccountOnboardingFlow

Výsledok pridania konta v Outlooku pomocou prostredia konfigurácie nového konta. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním. 

Zhromažďujú sa tieto polia:

- **AccountConfigAutoSignIn** – automatická konfigurácia konta nastavená správcom.

- **AccountConfigDomain** – doména špecifikovaná počas konfigurácie konta. 

- **AccountConfigEntryPoint** – vstupný bod, v ktorom používateľ zadal konfiguráciu konta. 

- **AccountConfigErrorCode** – kód chyby, ktorá sa vyskytla počas konfigurácie konta. 

- **AccountConfigErrorString** – chyba, ktorá sa vyskytla počas konfigurácie konta.

- **AccountConfigMethod** – metóda konfigurácie konta.

- **AccountConfigPhase** – aktuálny krok pracovného postupu konfigurácie konta.

- **AccountConfigPhaseFrom** – začiatočný krok pracovného postupu konfigurácie konta. 

- **AccountConfigPhaseTo** – posledný krok pracovného postupu konfigurácie konta. 

- **AccountType** – typ konta, ktoré sa konfiguruje.

- **AccountWorkflowSession** – relácia s pokusom o vykonanie pracovného postupu konta.

- **SessionDuration** – trvanie relácie.


#### <a name="officeoutlookmacdeleteaccountusage"></a>Office.Outlook.Mac.DeleteAccountUsage

Výsledok odstránenia konta v Outlooku. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. Naším cieľom je zvyšovať podiel úspešnosti každým vydaním. 

Zhromažďujú sa tieto polia:

- **AccountType** – typ konta, ktoré sa konfiguruje.

- **AccountID** – identifikátor konta.

- **DeprovisionAccount** – označuje, či sa konto odstráni zo servera.

- **IsFastDelete** – označuje, či sa konto odstráni vo vlákne na pozadí.

#### <a name="officepowerpointdocoperationclose"></a>Office.PowerPoint.DocOperation.Close

Zhromažďuje sa pri zatvorení powerpointových prezentácií. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú počas procesu zatvárania, ktorý zahŕňa zachovanie a synchronizáciu údajov používateľa. Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie zatvárania podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data\_Doc\_\*)? Ak nie, prečo?

  - **Data\_AutoSaveDisabledReasons:string** – preddefinovaná množina hodnôt toho, prečo bolo automatické ukladanie vypnuté pre tento dokument? (Chyba zlúčenia, chyba uloženia, skupinová politika atď.)

  - **Data\_CloseReason:long** – Ako sa zatvorenie uskutočnilo? Zatvorením dokumentu? Zatvorením aplikácie?

  - **Data\_CppUncaughtExceptionCount:long** – počet nespracovaných výnimiek

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou

  - **Data_Doc_AsyncOpenKind:long** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument)

  - **Data\_Doc\_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti

  - **Data\_Doc\_IsSyncBacked:bool** – overuje, či sa dokument otvára z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

  - **Data\_Doc\_ServerDocId:string** – nemenný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)

  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníka na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_DocHasStorage:bool** – má tento dokument lokálny ukladací priestor?

  - **Data\_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi)

  - **Data\_IsDocAutoSaveable:bool** – ukladá sa prezentácia automaticky?

  - **Data\_IsDocDirty:bool** – obsahuje prezentácia zmeny, ktoré ešte nie sú uložené?

  - **Data\_IsNewDoc:bool** – či ide o nový alebo existujúci dokument

  - **Data\_IsRecoveredDoc:bool** – je to obnovený dokument? (Ak predchádzajúca relácia zlyhala, tabla Obnovenie dokumentu bude zobrazená v ďalšej relácii.)

  - **Data\_NewDocDiscarded:bool** – či bola nová prezentácia zahodená bez uloženia

  - **Data\_OCSClosingDlgCanceled:bool** – ak nahratie čaká na OCS, keď používateľ zatvára dokument, používateľovi sa zobrazí dialógové okno s informáciou, aby čakal. Ktorú možnosť používateľ vybral?

  - **Data\_OCSClosingDlgExpired:bool** – zmizlo dialógové okno (po 1 minúte) automaticky?

  - **Data\_OCSClosingStatus:long** – označuje, aký je konečný stav OCS (In CSI (V CSI), Closable (Zatvoriteľný), In OCS Transition (V prechode OCS), In CSI transition (V prechode CSI) atď.)

  - **Data\_OCSClosingWaitDurationMS:long** – koľko času musel používateľ čakať na nahratie OCS

  - **Data\_OCSHandleTransitionResult:long** – preddefinovaná množina hodnôt výsledku prechodu vykonaného počas zavretia (pokus už prebehol, pokračovať v zatváraní atď.)

  - **Data\_ServerDocId:string** – identifikátor GUID na jedinečnú identifikáciu dokumentu

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_UserContinuedZRTClose:bool** – keď sa zobrazilo dialógové okno pri zatváraní, vybral používateľ možnosť „Continue“ (Pokračovať) na zatvorenie?

#### <a name="officepowerpointdocoperationnewdocument"></a>Office.PowerPoint.DocOperation.NewDocument

Zhromažďuje sa, keď PowerPoint vytvorí novú prezentáciu.  Obsahuje metriky úspešnosti, zlyhania a výkonu.

Tieto informácie sa používajú na zabezpečenie úspešného vytvorenia súboru bez zníženia výkonu.

Zhromažďujú sa tieto polia:

  - **NewDocumentType** – vytvoril sa nový dokument pomocou šablóny alebo otvorením prázdneho dokumentu?

  - **FLifeguarded** – či má dokument chránenú životnosť (funkciou, ktorá obnoví poškodený dokument bez zobrazenia upozornenia používateľovi)

#### <a name="officepowerpointdocoperationopencompleteprotocol"></a>Office.PowerPoint.DocOperation.OpenCompleteProtocol

Zhromažďuje sa pri otvorení powerpointových prezentácií. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú počas konečných fáz procesu otvárania.

Spoločnosť Microsoft používa tieto údaje na zabezpečenie fungovania funkcie podľa očakávaní bez toho, aby sa zhoršilo otváranie prezentácií.

Zhromažďujú sa tieto polia:

  - **Data\_AntiVirusScanMethod:long** – preddefinovaná množina hodnôt typu skenovania antivírusu (IOAV, AMSI, žiadny atď.)

  - **Data\_AntiVirusScanStatus:long** – preddefinovaná množina hodnôt skenovania antivírusu, ktoré prebieha pre každý otvorený dokument (NoThreatsDetected (Žiadne zistené hrozby), Failed (Zlyhanie), MalwareDetected (Zistil sa malvér) atď.)

  - **Data\_CloseAndReopen:bool** – bol tento dokument zatvorený a znova otvorený?

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou

  - **Data_Doc_AsyncOpenKind:long** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument)

  - **Data\_Doc\_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – otvára sa dokument z lokálnej vyrovnávacej pamäti?

  - **Data\_Doc\_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

  - **Data\_Doc\_ServerDocId:string** – nemenný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)

  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_ExecutionCount:long** – koľkokrát sme vykonali protokol IncOpen pred spustením tohto protokolu (OpenComplete)

  - **Data\_FailureComponent:long** – preddefinovaná množina hodnôt toho, ktorá súčasť spôsobila zlyhanie protokolu (Conflict, CSI, Internal atď.)

  - **Data\_FailureReason:long** – preddefinovaná množina hodnôt dôvodu zlyhania (FileIsCorrupt, BlockedByAntivirus atď.)

  - **Data_FullDownloadRoundTripCount:long** – počet návštev servera potrebných na stiahnutie celého dokumentu.
  
  - **Data_IsProtocolRunInIncOpenMode:bool** – či sa spustil protokol pre prírastkové sťahovanie, čo je sťahovanie, pri ktorom sa časti dokumentu stiahnu po jeho počiatočnom zobrazení používateľovi.

  - **Data\_MethodId:long** – zobrazuje, ktorý riadok kódu sa interne vykonal ako posledný

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_TimeToEdit:long** – čas, po ktorom bolo možné dokument upravovať

  - **Data\_TimeToView:long** – čas potrebný na vykreslenie prvej snímky dokumentu

  - **Data\_UnhandledException:bool** – existuje nejaká nespracovaná natívna výnimka?

#### <a name="officepowerpointdocoperationsave"></a>Office.PowerPoint.DocOperation.Save

Zhromažďuje sa vždy, keď PowerPoint vykoná uloženie pomocou cesty moderného kódu. Zahŕňa typ výsledku úspešnosti alebo zlyhania pre metriku výkonu pri ukladaní a metaúdaje relevantného dokumentu.  Zlyhania uloženia môžu mať za následok stratu údajov. Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie funkcie podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data\_Doc\_\*)? Ak nie, prečo?

  - **Data\_BeforeSaveEvent:long** – časový úsek, po ktorom nastala udalosť dokumentu pred uložením

  - **Data\_CheckDownRevSaveTimeMS:long** – čas potrebný na kontrolu revízie

  - **Data\_CheckMacroSaveTimeMS:long** – čas potrebný na uloženie makier

  - **Data\_ClearAutoSaveTimeMS:long** – čas potrebný na vymazanie príznaku automatického ukladania

  - **Data\_ClearDirtyFlagTimeMS:long** – čas potrebný na vymazanie príznaku zmeneného dokumentu

  - **Data\_CloneDocumentTimeMS:long** – čas potrebný na klonovanie dokumentu pred spustením ukladania

  - **Data\_CommitTransactionTimeMS:long** – čas potrebný na potvrdenie transakcie uloženia

  - **Data\_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou

  - **Data_Doc_AsyncOpenKind:long** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument)

  - **Data\_Doc\_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti

  - **Data\_Doc\_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

  - **Data\_Doc\_ServerDocId:string** – nemenný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)

  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_DurationUAEOnSaveStartedMs:long** – čas potrebný na ukončenie neznámej aplikácie počas ukladania

  - **Data\_EnsureSaveTransactionTimeMS:long** – čas potrebný na zabezpečenie vytvorenia transakcie uloženia, ak už neexistuje

  - **Data\_FailureComponent:long** – preddefinovaná množina hodnôt toho, ktorá súčasť spôsobila zlyhanie protokolu (Conflict, CSI, Internal atď.)

  - **Data\_FailureReason:long** – preddefinovaná množina hodnôt dôvodu zlyhania (FileIsCorrupt, BlockedByAntivirus atď.)

  - **Data\_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi)

  - **Data\_HandleEnsureContentType:long** – čas potrebný na zabezpečenie toho, že všetky typy obsahu sú správne

  - **Data\_HandleEnsureContentTypeTimeMS:long** – čas potrebný na zabezpečenie toho, že všetky typy obsahu sú správne

  - **Data\_HasEmbeddedFont:bool** – obsahuje tento dokument vložené písma?

  - **Data\_InitializeSaveTimeMS:long** – čas potrebný na inicializáciu obsahu dokumentu a spustenie ukladania

  - **Data\_InOCSTransition:bool** – či je toto uloženie vykonané na prechod na OCS

  - **Data\_IsSavingWithEmbeddedFont:bool** – obsahuje tento dokument vložené písma?

  - **Data\_MethodId:long** – ktorý riadok kódu sa interne vykonal ako posledný

  - **Data\_PerformEmbedFontsTimeMS:long** – čas potrebný na serializovanie vložených písiem

  - **Data\_PerformModernSaveTimeMS:long** – čas potrebný na vykonanie moderného uloženia (s novým kódom)

  - **Data\_PerformPostSaveTimeMS:long** – čas potrebný na vykonanie funkcií po uložení (oznámenia, položky vrátenia akcií)

  - **Data\_PrepareForSaveTimeMS:long** – čas potrebný na spustenie ukladania

  - **Data\_RaiseDocumentBeforeSaveEventTimeMS:long** – časový úsek, po ktorom nastala udalosť BeforeSave (Pred uložením)

  - **Data\_ReflectDocumentChangeTimeMS:long** – čas potrebný na prejavenie uložených zmien v používateľskom rozhraní (opakované vyplnenie miniatúr atď.)

  - **Data\_ReportStartTimeMS:long** – čas potrebný na dokončenie inicializácie telemetrie na ukladanie

  - **Data\_ReportSuccessTimeMS:long** – čas potrebný na dokončenie hlásenia o úspešnom uložení

  - **Data\_ResetDirtyFlagOnErrorTimeMS:long** – čas potrebný na vynulovanie príznaku zmeneného dokumentu pri chybe

  - **Data\_SaveReason:long** – preddefinovaná množina hodnôt dôvodu vykonania tohto uloženia (automatické ukladanie, ToOCSTransitionSave, ToCSITransitionSave atď.)

  - **Data\_SaveType:long** – preddefinovaná množina hodnôt typu uloženia (Uložiť ako, Publikovať, manuálne, OMSave atď.)

  - **Data\_SavingWithFont:bool** – ukladáme dokument s novými vloženými písmami?

  - **Data\_ScrubClonedDocumentTimeMS:long** – čas potrebný na odstránenie osobných informácií v klonovanej kópii dokumentu

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_TransactionType:long** – ide o transakciu uloženia alebo zlúčenia a uloženia?

#### <a name="officepowerpointdocoperationsaveas"></a>Office.PowerPoint.DocOperation.SaveAs

Zhromažďuje sa vždy, keď PowerPoint vykoná akciu Uložiť ako. Zahŕňa typ výsledku úspešnosti alebo zlyhania pre metriku výkonu pri ukladaní a metaúdaje relevantného dokumentu. Zlyhania uloženia môžu mať za následok stratu údajov.  Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie funkcie podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data_Doc_*)? Ak nie, prečo?

- **Data_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity.

- **Data_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená.

- **Data_DstDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_DstDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_DstDoc_AsyncOpenKind:long** – označuje, či bola otvorená verzia nového cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_DstDoc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_DstDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_DstDoc_Ext:string** – prípona dokumentu.

- **Data_DstDoc_Extension:string** – prípona dokumentu.

- **Data_DstDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_DstDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.
    
- **Data_DstDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_DstDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_DstDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_DstDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_DstDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).
    
- **Data_DstDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_DstDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_DstDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_DstDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_DstDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?
    
- **Data_DstDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_DstDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_DstDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_DstDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_DstDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_DstDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_DstDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_DstDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_DstDoc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_DstDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_DstDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_DstDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_DstDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_DstDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_DstDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_DstDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_DstDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_FileType:long** – preddefinovaná množina hodnôt interného typu súboru.

- **Data_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi).

- **Data_FWebCreated:bool** – má tento dokument príznak WebCreator?

- **Data_SaveReason:long** – preddefinovaná množina hodnôt dôvodu vykonania tohto uloženia. (automatické ukladanie, ToOCSTransitionSave, ToCSITransitionSave atď.)

- **Data_SaveType:long** – preddefinovaná množina hodnôt typu uloženia (Uložiť ako, Publikovať, manuálne, OMSave atď.). 

- **Data_SrcDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_SrcDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_SrcDoc_AsyncOpenKind:long** – označuje, či bola otvorená verzia pôvodného cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_SrcDoc_ChunkingType:long** – ako je dokument uložený v SharePointe. 

- **Data_SrcDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_SrcDoc_Ext:string** – prípona dokumentu.

- **Data_SrcDoc_Extension:string** – prípona dokumentu.

- **Data_SrcDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_SrcDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.

- **Data_SrcDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_SrcDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_SrcDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_SrcDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_SrcDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).

- **Data_SrcDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_SrcDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_SrcDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_SrcDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

- **Data_SrcDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_SrcDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_SrcDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_SrcDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_SrcDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_SrcDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_SrcDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_SrcDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_SrcDoc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_SrcDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_SrcDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_SrcDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_SrcDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_SrcDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_SrcDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_SrcDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_StopwatchDuration:long** – celkový čas aktivity.

- **Data_TypeOfSaveDialog:long** – preddefinovaná množina hodnôt dialógového okna (RUN_SAVEAS_DLG,RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG atď.)

- **Data_WaitForSaveOrMergeSuccess:bool** – označuje, že operácia uloženia ako bola úspešná pri čakaní na uloženie alebo zlúčenie na pozadí.
 
- **Data_WaitForSaveOrMergeTimeout:long** – označuje, že uplynul časový limit operácie uloženia ako pri čakaní na uloženie alebo zlúčenie na pozadí.

- **DstDoc** – nové umiestnenie dokumentu. 

- **SrcDoc** – pôvodné umiestnenie dokumentu.


#### <a name="officepowerpointdocoperationsavelegacy"></a>Office.PowerPoint.DocOperation.SaveLegacy

Zhromažďuje sa vždy, keď PowerPoint vykoná uloženie pomocou cesty staršieho kódu. Zahŕňa typ výsledku úspešnosti alebo zlyhania pre metriku výkonu pri ukladaní a metaúdaje relevantného dokumentu.  Zlyhania uloženia môžu mať za následok stratu údajov.  Spoločnosť Microsoft používa tieto údaje, aby sa zabezpečilo fungovanie funkcie podľa očakávaní a obsah používateľa sa úspešne zachoval.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemetryResult:long** – obsahuje tento záznam denníka celú potrebnú telemetriu dokumentu (polia Data_Doc_*)? Ak nie, prečo?

- **Data_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity.

- **Data_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená.

- **Data_Doc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_Doc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_AsyncOpenKind:long** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_Doc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_Doc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_Doc_Ext:string** – prípona dokumentu.

- **Data_Doc_Extension:string** – prípona dokumentu.

- **Data_Doc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_Doc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.

- **Data_Doc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_Doc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_Doc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_Doc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_Doc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).

- **Data_Doc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_Doc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_Doc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_Doc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_Doc_IsSyncBacked:bool** – označuje, či sa dokument otvára z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu

- **Data_Doc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_Doc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_Doc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_Doc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_Doc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_Doc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

- **Data_Doc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_Doc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_Doc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI). 

- **Data_Doc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_Doc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_Doc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_Doc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_Doc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_Doc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_Doc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_Doc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_Doc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_DstDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_DstDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_DstDoc_AsyncOpenKind:long** – označuje, či bola otvorená verzia nového cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_DstDoc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_DstDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_DstDoc_Ext:string** – prípona dokumentu.

- **Data_DstDoc_Extension:string** – prípona dokumentu.

- **Data_DstDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_DstDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.
    
- **Data_DstDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu.

- **Data_DstDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_DstDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_DstDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_DstDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).

- **Data_DstDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_DstDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_DstDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_DstDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_DstDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

- **Data_DstDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_DstDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_DstDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_DstDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_DstDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_DstDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_DstDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_DstDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_DstDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_DstDoc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_DstDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_DstDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_DstDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_DstDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_DstDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_DstDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_DstDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_DstDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_FileType:long** – preddefinovaná množina hodnôt interného typu súboru.

- **Data_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi).

- **Data_SaveReason:long** – preddefinovaná množina hodnôt dôvodu vykonania tohto uloženia. (automatické ukladanie, ToOCSTransitionSave, ToCSITransitionSave atď.)

- **Data_SaveType:long** – preddefinovaná množina hodnôt typu uloženia (Uložiť ako, Publikovať, manuálne, OMSave atď.).

- **Data_SrcDoc_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie | čítanie a zapisovanie).

- **Data_SrcDoc_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_SrcDoc_AsyncOpenKind:long** – označuje, či bola otvorená verzia pôvodného cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_SrcDoc_ChunkingType:long** – ako je dokument uložený v SharePointe.

- **Data_SrcDoc_EdpState:long** – stav ochrany podnikových údajov v dokumente.

- **Data_SrcDoc_Ext:string** – prípona dokumentu.

- **Data_SrcDoc_Extension:string** – prípona dokumentu.

- **Data_SrcDoc_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona).

- **Data_SrcDoc_Fqdn:string** – kde je dokument uložený (SharePoint.com, live.net), k dispozícii len pre domény v Office 365.

- **Data_SrcDoc_FqdnHash:string** – hodnota hash miesta uloženia dokumentu. 

- **Data_SrcDoc_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa.

- **Data_SrcDoc_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov.

- **Data_SrcDoc_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument.

- **Data_SrcDoc_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.).
    
- **Data_SrcDoc_IsCloudCollabEnabled:bool** – hodnota je True, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky na OPTIONS (Možnosti).

- **Data_SrcDoc_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnuť celý dokument).

- **Data_SrcDoc_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS.

- **Data_SrcDoc_IsOpeningOfflineCopy:bool** – overuje, či sa dokument otvára z lokálnej vyrovnávacej pamäti.

- **Data_SrcDoc_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

- **Data_SrcDoc_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.).

- **Data_SrcDoc_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.).

- **Data_SrcDoc_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu.

- **Data_SrcDoc_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu).

- **Data_SrcDoc_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.).

- **Data_SrcDoc_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerDocId:string** – nezmeniteľný identifikátor pre dokumenty uložené v cloude.

- **Data_SrcDoc_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.).

- **Data_SrcDoc_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI).

- **Data_SrcDoc_ServerVersion:long** – overuje, či je server založený na Office14, Office15 alebo Office16.

- **Data_SrcDoc_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu.

- **Data_SrcDoc_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

- **Data_SrcDoc_SizeInBytes:long** – veľkosť dokumentu v bajtoch.

- **Data_SrcDoc_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu.

- **Data_SrcDoc_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“.

- **Data_SrcDoc_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný).

- **Data_SrcDoc_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude.

- **Data_SrcDoc_UsedWrsDataOnOpen:bool** – hodnota true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa.

- **Data_SrcDoc_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“.

- **Data_StopwatchDuration:long** – celkový čas aktivity.

- **Data_TypeOfSaveDialog:long** – preddefinovaná množina hodnôt dialógového okna (RUN_SAVEAS_DLG,RUN_SAVEMEDIA_DLG, RUN_SAVEAS_VIDEO_DLG atď.).

- **Doc** – aktuálny dokument na uloženie.

- **DstDoc** – nové umiestnenie dokumentu (v prípade akcie Uložiť ako).

- **SrcDoc** – pôvodné umiestnenie dokumentu (v prípade akcie Uložiť ako).


#### <a name="officepowerpointpptiosrehearseview"></a>Office.PowerPoint.PPT.IOS.RehearseView 

Táto udalosť označuje, že používateľ ukončil reláciu skúšky. Údaje sa používajú v kombinácii s Office.PowerPoint.IOS.Android.RehearseView.StartSession ako indikátor akéhokoľvek zlyhania alebo chyby, ktorým používateľ čelí.  
 
Zhromažďujú sa tieto polia:

- **ConnectionCreationTime** – čas na vytvorenie bočných pripojení k služby.

- **CountDownAlertTime** – čas, pre ktorý sa zobrazilo upozornenie na odpočítavanie.

- **CountdownInitTime –** – čas medzi dokončením načítania prezentácie a spustením odpočítavania.

- **CritiqueSummary** – Súhrn toho, čo všetci kritici videli, spolu s ich počtami.

- **ExitEventCode** – kód na identifikáciu toho, v ktorom scenári používateľ ukončil skúšobnú reláciu, či išlo o chybový scenár, alebo úspešné ukončenie.

- **FRETime** – čas od začatia zobrazovania obrazovky FRE, kým ju používateľ nezrušil.

- **MicrophonePermissionTime** – čas, pre ktorý sa zobrazilo upozornenie na povolenie mikrofónu, kým používateľ nevybral niektorú z možností.

- **ResumeRehearsingCount** – počet kliknutí používateľa na pozastavenie skúšky.

- **RehearsalInitTime** – čas potrebný na inicializáciu skúšky.

- **ResumeRehearsingCount** – počet kliknutí používateľa na pokračovanie v skúške.

- **Sessionid** – Identifikátor relácie reči.  Používa sa na ladenie denníkov služby.

- **SlideshowViewLoadTime** – čas potrebný na načítanie prezentácie.


#### <a name="officepowerpointpptiosrehearseviewrehearsalsummarypage"></a>Office.PowerPoint.PPT.IOS.RehearseView.RehearsalSummaryPage

Udalosť sa spustí po dokončení načítania stránky súhrnu. Táto udalosť nám pomáha pri zachytávaní výkonu stránky súhrnu. Poskytuje nám informácie o tom, koľko času trvá načítanie stránky služby súhrnu skúšky na klientskom počítači. Je potrebná na udržanie výkonu funkcie.  

Zhromažďujú sa tieto polia: 

- **PayloadCreationTime** – čas v milisekundách, ktorý bol potrebný na vytvorenie údajovej časti.  

- **PostUrlCallTime** – čas v milisekundách, ktorý bol potrebný na odoslanie volania po URL adrese. 

- **RehearseSessionId** – identifikátor relácie reči. Môžeme ho použiť na ladenie denníkov služby.  

- **SummaryPageErrorReceived** – Boolovská hodnota, ktorá označuje, či bola prijatá stránka súhrnu alebo sa vyskytla chyba.

- **SummaryPageHtmlLoadTime** – čas v milisekundách, ktorý bol potrebný na načítanie html stránky súhrnu. 

- **SummaryPageHtmlLoadTime** – čas v milisekundách, ktorý bol potrebný na prijatie prvej odpovede zo servera. 

- **SummaryPageLoadTime** – trvanie (v ms) načítania stránky súhrnu. Zahŕňa čas vytvárania údajovej časti. 

- **ThumbnailsCount** – celkový počet miniatúr, ktoré budú súčasťou stránky súhrnu. 


#### <a name="officepowerpointpptiosrehearseviewstartsession"></a>Office.PowerPoint.PPT.IOS.RehearseView.StartSession 
 
Táto udalosť sa spúšťa, keď používateľ klikne na spustenie relácie. Táto udalosť nám pomáha zachytiť počet používateľov, ktorí používajú funkciu Prezentačný kouč v systéme iOS. V kombinácii s Office.PowerPoint.PPT.iOS.RehearseView nám poskytne informácie o tom, koľko používateľov úspešne dokončilo reláciu skúšky a koľko nie. Toto je náš prvý indikátor zlyhania alebo chýb vo funkcii.

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officepowerpointpptmacshellprintinfo"></a>Office.PowerPoint.PPT.Mac.Shell.PrintInfo

Zhromažďujú sa vždy, keď sa dokončí operácia exportovania PDF súboru a obsahuje informácie o úspešnosti operácie. Tieto informácie sú kritické pri identifikácii úspešnosti operácií exportovania PDF súborov pre našu aplikáciu.

Zhromažďujú sa tieto polia:

- **Data_ExportAsPDFSucceed** – boolovská hodnota označujúca, či bol export PDF súboru úspešný.

#### <a name="officepowerpointpptsharedrehearseviewrehearseclicked"></a>Office.PowerPoint.PPT.Shared.RehearseView.RehearseClicked

Táto udalosť zachytáva kliknutie na položku RehearseWithCoach.  Táto udalosť sa používa na analyzovanie kanála funkcie videné-vyskúšané-ponechané. Táto udalosť spolu s udalosťou vyskúšané a ponechané nám pomáha zistiť, či používatelia opúšťajú lievik. Pomôže nám to udržiavať stav funkcie.

Zhromažďujú sa tieto polia:

- Žiadne


#### <a name="officepowerpointpptsharedslideshowfailure"></a>Office.PowerPoint.PPT.Shared.SlideShow.Failure

Zhromažďuje informácie o zlyhaniach počas prezentácie ako kľúčovej funkcie pre PowerPoint. Spoločnosť Microsoft zhromažďuje tieto údaje v prípade výskytu chyby počas prezentácie na zlepšenie používateľského prostredia prezentácie. Spoločnosť Microsoft používa tieto údaje na získanie diagnostických informácií o tom, kde chyba sa vyskytuje, keď používateľ používa prezentáciu.

Zhromažďujú sa tieto polia:

- **CountOArtErrors** – celkový počet chýb v OArt

- **CountOtherErrors** – zobrazuje celkový počet ostatných chýb

- **CountPPTErrors** – celkový počet chýb v PPT

- **CountSlideShowErrors** – celkový počet chýb prezentácie

- **FirstOArtError** – prvý výskyt chyby v OArt

- **FirstOtherError** – prvý výskyt chyby v inej oblasti

- **FirstPPTError** – prvý výskyt chyby v PPT

- **FirstSlideShowError** – prvý výskyt chyby v prezentácii

    
#### <a name="officepowerpointrunprintoperation"></a>Office.PowerPoint.RunPrintOperation

Zhromažďujú sa vždy, keď sa dokončí operácia tlače PDF súboru a obsahuje informácie o type rozloženia, použití čísel snímok a úspešnosti operácie. Tieto informácie sú kritické pri identifikácii úspešnosti operácií tlače PDF súborov pre našu aplikáciu.

Zhromažďujú sa tieto polia:

- **Data_PrintWithSlideNumbers** – boolovská hodnota označujúca, či používateľ tlačí s číslami snímok.

- **Data_SavePrintLayoutType** – typ rozloženia pri tlači v čase začatia operácie tlače alebo exportu.

- **Data_Success** – boolovská hodnota označujúca, či bola tlač úspešná.


#### <a name="officeprojectprojectfilesave"></a>Office.Project.ProjectFileSave

Project uloží súbor. Táto udalosť označuje uloženie v Projecte. Umožňuje spoločnosti Microsoft merať úspešnosť uloženia súboru v Projecte, čo je dôležité, aby nedochádzalo k stratám údajov dokumentu.

Zhromažďujú sa tieto polia:

  - **Data\_TriggerTime** – čas uloženia

  - **Data\_FileType** – typ súboru, v ktorom sa projekt uloží
 
#### <a name="officesessionactivitystart"></a>Office.Session.Activity.Start

Umožňuje zistiť, kedy sa spustila relácia doplnku Data Streamer.  Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Activity_Name** – názov aktivity „Session“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – spustenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officesessionactivitystop"></a>Office.Session.Activity.Stop

Umožňuje zistiť, kedy sa skončila relácia doplnku Data Streamer. Používa sa na sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Activity_Name** – názov aktivity „Session“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – zastavenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officestreamdeviceactivitystart"></a>Office.StreamDevice.Activity.Start

Umožňuje zistiť, či je začiatok streamovania zdroja údajov úspešný.   Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „StreamDeviceData“ alebo „StreamFileData“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – spustenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officestreamdeviceactivitystop"></a>Office.StreamDevice.Activity.Stop

Umožňuje zistiť, či je koniec streamovania zdroja údajov úspešný.   Umožňuje sledovanie stavu funkcie a monitorovanie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Datasource_Type** -informácia o sériovom zariadení alebo službe aplikácie

- **DataSource_Name** – názov pripojeného zdroja údajov

- **Activity_Name** – názov aktivity „StreamDeviceData“ alebo „StreamFileData“

- **Activity_CV** – ID na koreláciu udalostí počas relácie pripojenia

- **Activity_StartStopType** – zastavenie

- **Activity_DateTimeTicks** – dátum a čas aktivity

#### <a name="officetargetedmessagingabexperimentmessagetrigger"></a>Office.TargetedMessaging.ABExperimentMessageTrigger

Sleduje počet používateľov, ktorí prijímajú správy BizBar a správy dynamického plátna zo služby TargetedMessagingService (TMS). Tieto údaje sú veľmi dôležité pri zisťovaní, aké správy používatelia dostávajú a na akom povrchu, aby sme mohli zabezpečiť, že dostanú všetky správy, ktoré pre nich môžu byť dôležité v súvislosti s ďalším používaním produktu. Tiež sú potrebné na presné meranie úspešnosti našich experimentov a kampaní spustených prostredníctvom TMS.

Zhromažďujú sa tieto polia:

  - **Data\_Surface** – názov povrchu, pre ktorý je táto správa doručená službou určená

  - **Data\_Flight** – identifikátor skupiny funkcií ECS/CT, ktorý sa použil na doručenie tejto správy

  - **Data\_CampaignId** – identifikátor kampane, ktorej je táto správa súčasťou

  - **Data\_MessageId** – identifikátor tejto správy doručenej službou

  - **Data\_TransactionId** – identifikátor tejto transakcie so službou

  - **Data\_TriggerPoint** – krok, v ktorom bola táto udalosť zaznamenaná (prijatie správy, zobrazenie správy)

#### <a name="officetextfontpickerfontselectedwin32"></a>Office.Text.FontPickerFontSelected.Win32

Táto udalosť označuje, či bolo stiahnuté písmo vykreslené správne. Používa sa na označenie úspešnosti alebo zlyhania stiahnutia písma.

Zhromažďujú sa tieto polia:

  - **Názov písma (Data\_Font)** – názov písma vybratého vo výbere písma

  - **Kliknutie používateľa (Data\_FClick)** – označuje výber položky používateľom pomocou myši

#### <a name="officetextresourceclientrequestresourceinternal"></a>Office.Text.ResourceClient.RequestResourceInternal

Táto udalosť označuje, či bolo písmo stiahnuté správne. Používa sa na označenie úspešnosti alebo zlyhania vykreslenia stiahnutého písma.

Zhromažďujú sa tieto polia:

  - **Data\_FontToken** – názov súboru prostriedkov, ktorý sa uloží

  - **Data\_HTTPResult** – výsledok požiadavky HTTP

  - **Data\_HTTPStatusCode** – kód HTTP vrátený z požiadavky HTTP

  - **Data\_isInternetOn** – či sme mali pripojenie pri pokuse o načítanie zdroja

  - **Data\_RequestUrl** – URL adresa zdroja CDN, ktorý sa pokúšame načítať



#### <a name="officetranslatordocumenttranslated"></a>Office.Translator.DocumentTranslated

Zhromažďuje informácie o úspešnosti alebo zlyhaní prekladu celého dokumentu pomocou používateľského spúšťača v službe Translator SDX. Je to veľmi dôležité na vyhodnotenie stavu funkcie prekladača a reagovanie na všetky výpadky, ktoré sa môžu vyskytnúť. Monitoruje stav scenára „Preložiť dokument“ vo Worde.

Zhromažďujú sa tieto polia:

- **Data.actionSource** – ako bol spustený preklad vybratého textu.

- **Data.bodyBackgroundColor** – farba pozadia kontajnera motívu balíka Office.

- **Data.bodyForegroundColor** – farba popredia kontajnera motívu balíka Office.

- **Data.browserLang** – jazyk aktuálneho zobrazenia prehliadača.

- **Data.browserOnline** – zastarané.

- **Data.browserPlatform** – platforma prehliadača.

- **Data.browserUserAgent** – agent používateľa prehliadača.

- **Data.colorDepth** – hĺbka systémovej farby.

- **Data.contentLanguage** – zistený jazyk obsahu, ktorý sa má preložiť.

- **Data.controlBackgroundColor** – farba pozadia ovládacieho prvku motívu balíka Office.

- **Data.controlForegroundColor** – farba popredia ovládacieho prvku motívu balíka Office.

- **Data.correlationId** – jedinečný identifikátor požiadavky odoslanej do služby.

- **Data.crossSessionId** – jedinečný identifikátor používateľa.

- **Data.crossSessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.currentTime** – časová pečiatka UTC odoslania správy telemetrie.

- **Data.displayLanguage** – jazyk zobrazenia balíka Office.

- **Data.documentSourceLang** – jazyk obsahu dokumentu.

- **Data.documentTargetLang** – jazyk, do ktorého sa preloží dokument.

- **Data.environment** – prostredie služby, kam je požiadavka odoslaná.

- **Data.errorMessage** – chybové hlásenie poskytnuté službou.

- **Data.eventActionType** – typ udalosti telemetrie.

- **Data.eventTagId"** – jedinečný identifikátor riadka kódu, ktorý vytvoril túto správu telemetrie.

- **Data.flights** – povolené skupiny funkcií.

- **Data.fileSize** – veľkosť wordového súboru, ktorý sa má preložiť.

- **Data.fileSource** – miesto, kde je wordový súbor hosťovaný (offline, online).

- **Data.fileType** – prípona wordového súboru.

- **Data.innerHeight** – výška kontajnera bočnej tably.

- **Data.innerWidth** – šírka kontajnera bočnej tably.

- **Data.lookupSourceLang** – nepoužíva sa v prípade prekladu dokumentu.

- **Data.lookupTargetLang** – nepoužíva sa v prípade prekladu dokumentu.

- **Data.officeHost** – aplikácia balíka Office, ktorá hosťuje bočnú tablu.

- **Data.officeLocale** – jazyk používateľa balíka Office.

- **Data.officeMachineId** – jedinečný identifikátor zariadenia.

- **Data.officePlatform** – platforma zariadenia.

- **Data.officeSessionId** – identifikátor relácie balíka Office.

- **Data.officeUserId** – jedinečný identifikátor používateľa balíka Office.

- **Data.officeVersion** – verzia balíka Office.

- **Data.pageXOffset** – vodorovná poloha posúvania bočnej tably z ľavej strany tably.

- **Data.pageYOffset** – zvislá poloha posúvania bočnej tably z hornej strany tably.

- **Data.pixelDepth** – farebné rozlíšenie obrazovky.

- **Data.responseCode** – kód odpovede na požiadavku zo služby.

- **Data.responseTime** – uplynutý čas požiadavky. 

- **Data.resultType** – výsledok požiadavky.

- **Data.screenHeight** – výška obrazovky v pixeloch.

- **Data.screenLeft** – vodorovná súradnica okna vo vzťahu k obrazovke.

- **Data.screenTop** – zvislá súradnica okna vo vzťahu k obrazovke.

- **Data.screenWidth** – šírka obrazovky v pixeloch.

- **Data.selectedTab** – označuje, či je vybratá karta výberu alebo dokumentu.

- **Data.serverUrl** – URL adresa prekladateľskej služby.

- **Data.sessionId** – identifikátor relácie bočnej tably.

- **Data.sessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.sourceTextHash** – hodnota hash textu na preklad.

- **Data.sourceTextLength** – dĺžka textu na preklad.

- **Data.sourceTextWords** – počet slov v texte na preklad.

- **Data.warningMessage** – upozorňujúca správa hlásená službou.


#### <a name="officetranslatortexttranslated"></a>Office.Translator.TextTranslated

Zhromažďuje informácie o úspešnosti alebo zlyhaní prekladu výberu, ktorý sa spustí akciou používateľa v službe Translator SDX. Je to veľmi dôležité na vyhodnotenie stavu funkcie prekladača a reagovanie na všetky výpadky, ktoré sa môžu vyskytnúť. Používa na monitorovanie stavu scenára „Preložiť vybratý text“ v Exceli, v PowerPointe a vo Word.

Zhromažďujú sa tieto polia:

- **Data.actionSource** – ako bol spustený preklad vybratého textu.

- **Data.bodyBackgroundColor** – farba pozadia kontajnera motívu balíka Office.

- **Data.bodyForegroundColor** – farba popredia kontajnera motívu balíka Office.

- **Data.browserLang** – jazyk aktuálneho zobrazenia prehliadača.

- **Data.browserOnline** – zastarané.

- **Data.browserPlatform** – platforma prehliadača.

- **Data.browserUserAgent** – agent používateľa prehliadača.

- **Data.colorDepth** – hĺbka systémovej farby.

- **Data.contentLanguage** – zistený jazyk obsahu, ktorý sa má preložiť.

- **Data.controlBackgroundColor** – farba pozadia ovládacieho prvku motívu balíka Office.

- **Data.controlForegroundColor** – farba popredia ovládacieho prvku motívu balíka Office.

- **Data.correlationId** – jedinečný identifikátor požiadavky odoslanej do služby.

- **Data.crossSessionId** – jedinečný identifikátor používateľa.

- **Data.crossSessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.currentTime** – časová pečiatka UTC odoslania správy telemetrie.

- **Data.displayLanguage** – jazyk zobrazenia balíka Office.

- **Data.documentSourceLang** – nepoužíva sa v prípade vybratého textu.

- **Data.documentTargetLang** – nepoužíva sa v prípade vybratého textu.

- **Data.environment** – prostredie služby, kam je požiadavka odoslaná.

- **Data.errorMessage** – chybové hlásenie poskytnuté službou.

- **Data.eventActionType** – typ udalosti telemetrie.

- **Data.eventTagId"** – jedinečný identifikátor riadka kódu, ktorý vytvoril túto správu telemetrie.

- **Data.flights** – povolené skupiny funkcií.

- **Data.innerHeight** – výška kontajnera bočnej tably.

- **Data.innerWidth** – šírka kontajnera bočnej tably.

- **Data.lookupSourceLang** – jazyk aktuálne vybratého textu.

- **Data.lookupTargetLang** – jazyk, do ktorého sa aktuálne vybratý text preloží.

- **Data.officeHost** – aplikácia balíka Office, ktorá hosťuje bočnú tablu.

- **Data.officeLocale** – jazyk používateľa balíka Office.

- **Data.officeMachineId** – jedinečný identifikátor zariadenia.

- **Data.officePlatform** – platforma zariadenia.

- **Data.officeSessionId** – identifikátor relácie balíka Office.

- **Data.officeUserId** – jedinečný identifikátor používateľa balíka Office.

- **Data.officeVersion** – verzia balíka Office.

- **Data.pageXOffset** – vodorovná poloha posúvania bočnej tably z ľavej strany tably.

- **Data.pageYOffset** – zvislá poloha posúvania bočnej tably z hornej strany tably.

- **Data.pixelDepth** – farebné rozlíšenie obrazovky.

- **Data.responseCode** – kód odpovede na požiadavku zo služby.

- **Data.responseTime** – uplynutý čas požiadavky.

- **Data.resultType** – výsledok požiadavky.

- **Data.screenHeight** – výška obrazovky v pixeloch.

- **Data.screenLeft** – vodorovná súradnica okna vo vzťahu k obrazovke.

- **Data.screenTop** – zvislá súradnica okna vo vzťahu k obrazovke.

- **Data.screenWidth** – šírka obrazovky v pixeloch.

- **Data.selectedTab** – označuje, či je vybratá karta výberu alebo dokumentu.

- **Data.serverUrl** – URL adresa prekladateľskej služby.

- **Data.sessionId** – identifikátor relácie bočnej tably.

- **Data.sessionStartTime** – časová pečiatka UTC spustenia relácie prekladu.

- **Data.sourceTextHash** – hodnota hash textu na preklad.

- **Data.sourceTextLength** – dĺžka textu na preklad.

- **Data.sourceTextWords** – počet slov v texte na preklad.

- **Data.warningMessage** – upozorňujúca správa hlásená službou.


#### <a name="officeuxacccheckeracccheckerfinalviolationcountperrule"></a>Office.UX.AccChecker.AccCheckerFinalViolationCountPerRule

Táto udalosť sa spustí, keď sa pre aktuálne otvorený dokument oznamujú problémy so zjednodušením ovládania. Táto udalosť predstavuje porušenia zjednodušenia ovládania (chyby, upozornenia a tipy), ktoré existujú pre jednotlivé pravidlá pre otvorený dokument na začiatku a na konci relácie.  Táto udalosť sa používa na zaznamenanie počtov porušení zjednodušenia ovládania (chyby, upozornenia a tipy) pre jednotlivé pravidlá pre otvorený dokument na začiatku a na konci relácie.

Podrobnosti o počtoch porušení pre jednotlivé pravidlá pomáhajú spoločnosti Microsoft zistiť, ktoré problémy so zjednodušeným ovládaním sú najbežnejšie v dokumentoch balíka Office. Pomáha to pri práci na ich odstraňovaní a podporuje to vytváranie inkluzívneho prostredia na pracoviskách a v triedach pre osoby s postihnutím.

Zhromažďujú sa tieto polia:

- **Data_FinalCount_RuleID_0** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_1** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_2** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_3** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_4** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_5** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_6** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_7** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_8** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_9** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_10** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_11** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_12** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_13** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_14** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_15** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_16** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_FinalCount_RuleID_17** – počet porušení ID pravidla = n, ktoré zostali pri poslednom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_0** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_1** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_2** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_3** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_4** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_5** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_6** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_7** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_8** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_9** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_10** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_11** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_12** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_13** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_14** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_15** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_16** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **Data_InitialCount_RuleID_17** – počet porušení ID pravidla = n, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **FinalDocID** – konečné ID skontrolovaného dokumentu

- **FinalDocUrlHash** – konečná hodnota hash URL adresy skontrolovaného dokumentu
    
- **InitialDocID** – počiatočné ID skontrolovaného dokumentu

- **InitialDocUrlHash** – počiatočná hodnota hash URL adresy skontrolovaného dokumentu

- **PaneOpened** – Boolovská hodnota, ktorá sleduje, či sa otvorila tabla kontroly zjednodušenia ovládania

- **ServerDocID** – ID dokumentu na serveri pre dokument skontrolovaný kontrolou zjednodušenia ovládania


#### <a name="officeuxacccheckeracccheckerviolationinformation"></a>Office.UX.AccChecker.AccCheckerViolationInformation

Táto udalosť sa spustí, keď sa pre aktuálne otvorený dokument oznamujú problémy so zjednodušením ovládania. Predstavuje súhrnné počty porušení zjednodušenia ovládania (chyby, upozornenia a tipy) pre otvorený dokument na začiatku a na konci relácie. Táto udalosť sa používa na zaznamenanie súhrnných počtov porušení zjednodušenia ovládania (chyby, upozornenia a tipy) pre otvorený dokument na začiatku a na konci relácie. Informácie o používaní kontroly zjednodušenia ovládania umožňujú spoločnosti Microsoft zlepšovať aplikácie, aby boli inkluzívnejšie pre osoby s postihnutím v scenároch používania balíka Office pre pracoviskách a v triedach.

Zhromažďujú sa tieto polia:
    
- **FinalDocID** – konečné ID skontrolovaného dokumentu

- **FinalDocUrlHash** – konečná hodnota hash URL adresy skontrolovaného dokumentu

- **FinalErrorCount** – výsledný počet chýb nahlásených kontrolou zjednodušenia ovládania pre dokument

- **FinalIntelligentServiceCount** – výsledný počet problémov inteligentných služieb nahlásených kontrolou zjednodušenia ovládania pre dokument

- **FinalTipCount** – výsledný počet tipov nahlásených kontrolou zjednodušenia ovládania pre dokument

- **FinalViolationCount** – výsledný počet narušení nahlásených kontrolou zjednodušenia ovládania pre dokument

- **FinalWarningCount** – výsledný počet výstrah nahlásených kontrolou zjednodušenia ovládania pre dokument

- **InitialDocID** – počiatočné ID skontrolovaného dokumentu

- **InitialDocUrlHash** – počiatočná hodnota hash URL adresy skontrolovaného dokumentu

- **InitialErrorCount** – Počet všetkých porušení typu Chyba, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **InitialIntelligentServicesCount** – Počet všetkých porušení typu Inteligentná služba, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **InitialTipCount** – Počet všetkých porušení typu Tip, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **InitialUrlHash** – Počet všetkých porušení typu Chyba, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **InitialViolationCount** – Počet všetkých narušení, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **InitialWarningCount** – Počet všetkých porušení typu Výstraha, ktoré sa zistili pri prvom spustení kontroly zjednodušenia ovládania v relácii.

- **PaneOpened** – Boolovská hodnota, ktorá sleduje, či sa otvorila tabla kontroly zjednodušenia ovládania

- **ServerDocID** – ID dokumentu na serveri pre dokument skontrolovaný kontrolou zjednodušenia ovládania


#### <a name="officeuxacccheckerbackgroundacccheckerenabledstate"></a>Office.UX.AccChecker.BackgroundAccCheckerEnabledState

Táto udalosť sa spustí, keď používateľ alebo správca IT zapne kontrolu zjednodušenia ovládania na pozadí pre používateľa balíka Office. Táto udalosť sa používa na pochopenie inštancií, keď kontrola zjednodušenia ovládania je zapnutá pre používateľov balíka Office. Zapnutý stav kontroly zjednodušenia ovládania na pozadí umožňuje spoločnosti Microsoftu určiť, či sa dokumenty dajú automaticky kontrolovať na pozadí. Pomáha to pri vytváraní inkluzívnejšieho prostredia na pracoviskách a v triedach pre osoby s postihnutím.

Zhromažďujú sa tieto polia:

- **BackgroundAccCheckerEnabled** – Boolovská hodnota na sledovanie stavu zapnutia alebo vypnutia kontroly zjednodušenia ovládania


#### <a name="officeuxacccheckerbackgroundscanningcheckboxclicked"></a>Office.UX.AccChecker.BackgroundScanningCheckboxClicked

Táto udalosť sa spustí, keď používateľ IT zapne kontrolu zjednodušenia ovládania na pozadí z tably úloh Kontrola zjednodušenia ovládania.  Táto udalosť sa používa na pochopenie inštancií, keď kontrola zjednodušenia ovládania na pozadí je zapnutá pre dokumenty balíka Office. Zapnutý stav kontroly zjednodušenia ovládania na pozadí umožňuje spoločnosti Microsoftu určiť, či sa dokumenty dajú automaticky kontrolovať na pozadí. Pomáha to pri vytváraní inkluzívnejšieho prostredia na pracoviskách a v triedach pre osoby s postihnutím.

Zhromažďujú sa tieto polia:
    
- **FinalBackgroundScanningState** – konečný stav začiarkavacieho políčka, ktoré umožňuje kontrolu na pozadí

- **InitialBackgroundScanningState** – počiatočný stav začiarkavacieho políčka, ktoré umožňuje kontrolu na pozadí


#### <a name="officeuxacccheckerdisabledresults"></a>Office.UX.AccChecker.DisabledResults

Táto udalosť sa spustí, keď sa kontrola zjednodušenia ovládania vypne pre otvorený dokument. Táto udalosť sa používa na pochopenie inštancií, keď sa kontrola zjednodušenia ovládania vypne z dôvodu staršieho alebo nepodporovaného dokumentu balíka Office. Stav vypnutia kontroly zjednodušenia ovládania umožňuje spoločnosti Microsoft pochopiť, ako často sa dokument nedá skontrolovať, a pomôcť používateľom v umožnení kontroly takýchto dokumentov – skonvertovaním dokumentu do moderného formátu súborov. Pomáha to pri vytváraní inkluzívnejšieho prostredia na pracoviskách a v triedach pre osoby s postihnutím.

Zhromažďujú sa tieto polia:
    
- **Data_Disabled_ID** – ID chyby spôsobujúcej vypnutie

- **Data_Disabled_Reason** – dôvod vypnutia kontroly zjednodušenia ovládania

- **Data_IsUpConvertEnabled** – sleduje, či je pre dokument k dispozícii možnosť konvertovania na moderný formát súboru


#### <a name="officeuxacccheckershowtaskpane"></a>Office.UX.AccChecker.ShowTaskPane

Táto udalosť sa spustí, keď sa karta úloh Kontrola zjednodušenia ovládania spustí pre aktuálne otvorený dokument.  Táto udalosť sa používa na pochopenie používania kontroly zjednodušenia ovládania balíka Office. Kontrola zjednodušenia ovládania sa používa na identifikáciu a riešenie problémov so zjednodušeným ovládaním v dokumentoch balíka Office. Informácie o používaní kontroly zjednodušenia ovládania umožňujú spoločnosti Microsoft zlepšovať aplikácie, aby boli inkluzívnejšie pre osoby s postihnutím v scenároch používania balíka Office pre pracoviskách a v triedach.

Zhromažďujú sa tieto polia:

- **BackgroundScanCheckboxEnabled** – sleduje, či je kontrola zjednodušenia ovládania na pozadí zapnutá
    
- **Column** – účel

- **DocUrlHash** – jedinečná hodnota hash ID skontrolovaného dokumentu

- **HasAccessibilityViolations** – sleduje, či dokument obsahuje porušenia zjednodušenia ovládania v čase otvorenia tably

- **IsPaneDisabled** – sleduje, či je tabla Kontrola zjednodušenia ovládania otvorená v stave vypnutia (starší alebo nepodporovaný dokument)

- **PaneOpenedBefore** – sleduje, či tabla Kontrola zjednodušenia ovládania bola predtým otvorená

- **WAC_ServerDocId** – ID dokumentu na serveri pre dokument, ktorý bol skontrolovaný


#### <a name="officevisiosharedfeatureexperimentation"></a>Office.Visio.Shared.FeatureExperimentation

Táto udalosť sleduje zoskupovanie funkcií pre používateľov. Pomáha nám určiť úspech alebo neúspech skupín funkcií.

Zhromažďujú sa tieto polia:

  - **Data\_Enable:bool** – hodnota true označuje, že funkcia je povolená pre aktuálneho používateľa

  - **Data\_Feature:string** – názov funkcie

  - **Data\_Flighted:bool** – hodnota true označuje, že funkcia je povolená

  - **Data\_Licensed:bool** – hodnota true označuje, že na funkciu sa vzťahuje kontrola licencie

  - **Data\_Subscriber:bool** – hodnota true označuje, že používateľ má predplatenú licenciu

#### <a name="officevisiosharedrefreshsmartdiagram"></a>Office.Visio.Shared.RefreshSmartDiagram

Táto udalosť zachytáva zlyhania obnovenia diagramu, keď je súbor vytvorený cez DV. Pomáha nám to ladiť zlyhania a problémy v obnovení údajov v diagrame DV.

Zhromažďujú sa tieto polia:

  - **Data\_ConnectorsBasedOnSequence:bool** – má hodnotu true, ak obnovený diagram bol pôvodne vytvorený pomocou konektora na základe možnosti postupnosti

  - **Data\_DialogError**:**string** – chyba počas obnovovania inteligentného diagramu

  - **Data\_FileError:string** – reťazec chyby, keď pripojený excelový súbor je neplatný

  - **Data\_OverwriteSelected**:**bool** – má hodnotu true, ak používateľ počas obnovenia vybral možnosť prepísania diagramu

  - **Data\_WarningShown**:**bool** – má hodnotu true, ak sa počas obnovenia údajov používateľovi zobrazila nejaká výstraha

#### <a name="officevisiosharedwritebacktoexcel"></a>Office.Visio.Shared.WritebackToExcel

Táto udalosť zachytáva zlyhania spätného zapisovania Excelu, keď je súbor vytvorený cez DV. Pomáha nám to ladiť zlyhania a problémy v spätnom zapisovaní údajov do Excelu v diagrame DV.

Zhromažďujú sa tieto polia:

  - **Data\_ConnectorsBasedOnSequence:bool** – hodnota true znamená, že konektory sú vytvorené na základe nastavení postupnosti

  - **Data\_DataSourceType:string** – toto pole označuje, či je diagram vytvorený z tabuľky alebo z vlastného rozsahu

  - **Data\_DialogError:string** – typ vlastnej chyby počas vytvárania inteligentného diagramu prostredníctvom Excelu

  - **Data\_NoOfShapesAdded:int** – počet tvarov pridaných počas funkcie spätného zapisovania do Excelu

  - **Data\_NoOfShapesDeleted:int** – počet tvarov odstránených počas funkcie spätného zapisovania do Excelu

  - **Data\_OverwriteSelected:bool** – má hodnotu true, ak používateľ vybral možnosť prepísania údajov

  - **Data\_SourceDataModified:bool** – hodnota true označuje, že zdrojové údaje sú upravené

  - **Data\_WarningShown:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha aktualizácie údajov

  - **Data\_WarningShownBecauseOfPresenceOfFormula:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha z dôvodu prítomnosti vzorca v Exceli

  - **Data\_WarningShownToAddNextStepID:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha z dôvodu chýbajúceho identifikátora ďalšieho kroku v Exceli

  - **Data\_WarningShownToConvertToTable:bool** – hodnota true označuje, že používateľovi sa zobrazila výstraha na skonvertovanie excelových údajov do tabuľkového formátu


#### <a name="officewordfilenewcreatenewfile"></a>Office.Word.FileNew.CreateNewFile

Táto udalosť označuje vytvorenie nového dokumentu v programe Office Word a sleduje úspešnosť alebo zlyhanie tejto operácie. Udalosť sa používa na monitorovanie, či tvorba nového dokumentu funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

  - **Data\_DirtyState** – či bol dokument vytvorený v zmenenom stave (so zmenami, ktoré je potrebné uložiť)

  - **Data\_ErrorID** – identifikátor chyby v prípade zlyhania operácie

  - **Data\_MainPdod** – identifikátor dokumentu počas tejto relácie procesu

  - **Data\_UsesCustomTemplate** – označuje, či bol dokument vytvorený pomocou vlastnej šablóny

#### <a name="officewordfileopenuserinitiatedopen"></a>Office.Word.FileOpen.UserInitiatedOpen 

Táto udalosť označuje, že Office Word otvára dokument na základe akcie používateľa, nie priamo z programu. Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa.  Udalosť monitoruje, či otvorenie súboru funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu. 
 
Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov. 

- **Data_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť. 

- **Data_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, ale vyžadovalo by to značné investície do kódu. 

- **Data_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor. 

- **Data_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme. 

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť. 

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou. 

- **Data_Doc_ChunkingType** – jednotky slúžiace na prírastkové otvorenie dokumentu. 

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu. 

- **Data_Doc_Ext** – prípona dokumentu (docx, xlsb, pptx atď.). 

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru. 

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online. 

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény. 

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia. 

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený. 

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky. 

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa. 

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo. 

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce. 

- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline. 

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu. 

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint). 

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument. 

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav. 

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie. 

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie. 

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov. 

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov. 

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou. 

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.). 

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu. 

- **Data_Doc_SessionId** – verzia servera, ktorý ponúka službu. 

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online. 

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu. 

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu. 

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý. 

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby). 

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu. 

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI. 

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania. 

- **Data_EditorsCount** – počet editorov v dokumente. 

- **Data_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania. 

- **Data_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu. 

- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o otvorenie zlyhá dvakrát (používa sa na diagnostiku kvality údajov). 

- **Data_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny. 

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word. 

- **Data_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na diagnostikovanie výkonu otvárania. 

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu. 

- **Data_MoveFlightEnabled** – označuje, či je zapnutá skupina funkcií premiestňovania. 

- **Data_OpenInitiateKind** – typ scenára, v ktorom používatelia spustili túto operáciu otvorenia súboru. 

- **Data_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje. 

- **Data_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením. 

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu. 

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania. 

- **Data_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie. 

- **Data_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený. 

- **Data_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne. 

- **Data_VerboseMeasurements** – šifrovaný reťazec obsahujúci podrobné časové rozdelenie jednotlivých častí otvárania.  Používa sa na meranie výkonu, je zapnutý len pre interné okruhy. 



#### <a name="officewordfilesaveactcmdgosubsaveas"></a>Office.Word.FileSave.ActCmdGosubSaveAs

Táto udalosť označuje, že používateľ ukladá zmeny do nového dokumentu. Udalosť monitoruje, či ukladanie do nového dokumentu funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_Doc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.
    
- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.
    
- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o uloženie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

    

#### <a name="officewordfilesaveactfconfirmsavedoccorequerysave"></a>Office.Word.FileSave.ActFConfirmSaveDocCoreQuerySave

Táto udalosť označuje, že Office Word zobrazí používateľovi výzvu na uloženie zmien pri pokuse o zatvorenie dokumentu. Umožňuje spoločnosti Microsoft monitorovať, či ukladanie pri ukončení funguje podľa očakávaní, aby nedochádzalo k strate údajov dokumentu. Udalosť monitoruje, či ukladanie pri ukončení funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_Doc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.
    
- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_DstDoc_AccessMode** – označuje, či je cieľový dokument iba na čítanie alebo editovateľný.

- **Data_DstDoc_EdpState** – nastavenie ochrany elektronických údajov cieľového dokumentu.

- **Data_DstDoc_Ext** – prípona cieľového dokumentu (docx, xlsb, pptx atď.).

- **Data_DstDoc_FileFormat** – verzia protokolu formátu súboru cieľového dokumentu.

- **Data_DstDoc_Location** – označuje, ktorá služba poskytne ukladací priestor pre cieľový dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_DstDoc_LocationDetails** – označuje, ktorý známy lokálny priečinok uložil cieľový dokument.

- **Data_DstDoc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_DstDoc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu pre cieľový dokument.

- **Data_FailureClass** – celé číslo predstavujúce triedu zlyhania pri zlyhaniach prechodu na OCS.

- **Data_LocationPickerSaveStatus** – celočíselná hodnota označujúca akciu, ktorá spustila uloženie z dialógového okna Uložiť pri skončení.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_OCSSyncbackSaveStarted** – príznak, ktorý označuje, že toto uloženie súvisí s uložením so synchronizáciou zálohovania. 

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SaveInitiateKind** – celé číslo, ktoré označuje spôsob spustenia ukladania.

- **Data_SrcDocIsUnnamedOrNew** – označuje, či ukladaný dokument je nový.


#### <a name="officewordfilesavesaveassavefile"></a>Office.Word.FileSave.SaveAsSaveFile

Táto udalosť označuje, že Office Word ukladá dokument do nového dokumentu. Umožňuje spoločnosti Microsoft zisťovať chyby funkcie Uložiť ako, čo je dôležité na zabránenie strate údajov dokumentu. Udalosť monitoruje, či funkcia Uložiť ako funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_AddDocTelemResDst** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti pre cieľový dokument. Používa sa na diagnostiku kvality údajov.

- **Data_AddDocTelemResSrc** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti pre zdrojový dokument. Používa sa na diagnostiku kvality údajov.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_Doc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_DstDoc_AccessMode** – označuje, či je cieľový dokument iba na čítanie alebo editovateľný.

- **Data_DstDoc_AssistedReadingReasons** – preddefinovaná množina hodnôt toho, prečo bol cieľový dokument otvorený v režime čítania s asistenciou.

- **Data_DstDoc_AsyncOpenKind** – označuje, či bola otvorená verzia nového cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.
    
- **Data_DstDoc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_DstDoc_EdpState** – nastavenie ochrany elektronických údajov cieľového dokumentu.

- **Data_DstDoc_Ext** prípona dokumentu (docx, xlsb, pptx atď.).

- **Data_DstDoc_FileFormat** – verzia protokolu formátu súboru.

- **Data_DstDoc_Fqdn** – názov domény OneDrivu alebo SharePointu Online pre cieľový dokument.

- **Data_DstDoc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény pre cieľový dokument.

- **Data_DstDoc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_DstDoc_InitializationScenario** – zaznamenáva, ako bol cieľový dokument otvorený.

- **Data_DstDoc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností otvorenej požiadavky pre cieľový dokument.
    
- **Data_DstDoc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre cieľový dokument alebo používateľa.

- **Data_DstDoc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_DstDoc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_DstDoc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_DstDoc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_DstDoc_Location** – označuje, ktorá služba poskytla ukladací priestor pre cieľový dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_DstDoc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_DstDoc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_DstDoc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie pre cieľový dokument.

- **Data_DstDoc_ReadOnlyReasons** – dôvody, prečo bol cieľový dokument otvorený iba na čítanie. 

- **Data_DstDoc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_DstDoc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_DstDoc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_DstDoc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).
    
- **Data_DstDoc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_DstDoc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_DstDoc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_DstDoc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_DstDoc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_DstDoc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_DstDoc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_DstDoc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu pre cieľový dokument.
    
- **Data_DstDoc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_FailureClass** – celé číslo predstavujúce triedu zlyhania pri zlyhaniach prechodu na OCS.

- **Data_LocationPickerPropagateToSaveTime,spLapsedMsec** – čas v milisekundách, ktorý trvalo, kým sa spustilo ukladanie po získaní výsledku z okna výberu umiestnenia.

- **Data_LocationPickerSaveStatus** – stav vrátený oknom na výber umiestnenia.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SaveInitiateKind** – celé číslo, ktoré označuje spôsob spustenia ukladania.

- **Data_SrcDoc_AccessMode** – označuje, či je zdrojový dokument iba na čítanie alebo editovateľný.

- **Data_SrcDoc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_SrcDoc_AsyncOpenKind** – označuje, či bola otvorená verzia pôvodného cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_SrcDoc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_SrcDoc_EdpState** – nastavenie ochrany elektronických údajov zdrojového dokumentu.

- **Data_SrcDoc_Ext** – prípona zdrojového dokumentu (docx, xlsb, pptx atď.).

- **Data_SrcDoc_FileFormat** – verzia protokolu formátu súboru zdrojového dokumentu.

- **Data_SrcDoc_Fqdn** – názov domény OneDrivu alebo SharePointu Online pre zdrojový dokument.

- **Data_SrcDoc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény pre zdrojový dokument.

- **Data_SrcDoc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_SrcDoc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_SrcDoc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_SrcDoc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_SrcDoc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_SrcDoc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_SrcDoc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_SrcDoc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.
    
- **Data_SrcDoc_Location** – označuje, ktorá služba poskytla zdrojový dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_SrcDoc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_SrcDoc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_SrcDoc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_SrcDoc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_SrcDoc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_SrcDoc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_SrcDoc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_SrcDoc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_SrcDoc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_SrcDoc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_SrcDoc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_SrcDoc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_SrcDoc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_SrcDoc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_SrcDoc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_SrcDoc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_SrcDoc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_SrcDocIsUnnamedOrNew** – označuje, či ukladaný dokument je nový.


#### <a name="officewordworddocumentdirtyflagchanged"></a>Office.Word.Word.DocumentDirtyFlagChanged

Táto udalosť označuje, že Office Word upravuje dokument, v ktorom sa zmenil interný stav dokumentu na zmenený (dirty). Umožňuje spoločnosti Microsoft vyhodnotiť stav funkcie úpravy dokumentu. Udalosť predstavuje signál úprav používateľa. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac.

Zhromažďujú sa tieto polia:

  - **Data\_CollectionTime** – časová pečiatka udalosti

  - **Data\_DocumentLocation** – typ umiestnenia dokumentu

  - **Data\_DocumentLocationDetails** – podtyp umiestnenia dokumentu

  - **Data\_FAlwaysSaveEnabled** – označuje, či bola povolená možnosť Vždy uložiť

  - **Data\_FirstEditTime** – časová pečiatka prvej úpravy

  - **Data\_NumberCoAuthors** – počet spoluautorov upravujúcich dokument počas relácie

  - **Data\_NumberOfTimesDocumentDirtied** – počet úprav dokumentu

  - **Data\_Pdod** – identifikátor dokumentu v procese programu Office Word

  - **Data\_UrlHash** – hodnota hash cesty dokumentu

  - **Data\_ViewKind** – typ zobrazenia Wordu



#### <a name="onenoteappnavigationratingreminderdialogshown"></a>OneNote.App.Navigation.RatingReminderDialogShown

Kritický signál, ktorý sa používa na meranie efektivity logiky spúšťača pre pripomenutie hodnotenia. Toto dialógové okno sa zobrazí, keď používateľ splnil všetky podmienky na zobrazenie pripomenutia hodnotenia (počet aktívnych dní, v minulosti hodnotil alebo nie atď.). Používa sa na zaručenie logiky spúšťača pre pripomenutie hodnotenia. Ak sa používateľom zobrazí toto dialógové okno, poskytne nám spôsoby, ako získať pripomienky od zákazníkov v správnom čase a zlepšiť stav aplikácie.

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="parselicenseop"></a>ParseLicenseOp

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM.  Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú pri vykonávaní operácie analýzy licencií. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera zapisovača.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.Duration** – celkový čas na dokončenie operácie.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z operácie, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.Result** – úspech alebo zlyhanie operácie.

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu výsledku operácie.

- **RMS.VerifyCertChainDuration** – čas trvania na overenie reťazca certifikátu.

- **RMS.VerifySignatureDuration** – čas trvania na overenie podpisu.

#### <a name="readconversation"></a>read.conversation

Slúži na sledovanie možného nepriaznivého vplyvu na stav a výkon vykresľovania e-mailovej správy

Zhromažďujú sa tieto polia: 

- **above_40fps** – počet snímok vykreslených nad 40 fps
 
- **above_50fps** – počet snímok vykreslených nad 50 fps
 
- **above_55fps** – počet snímok vykreslených nad 55 fps

- **adal_id** – ID overenia konta v službe Active Directory, jedinečný identifikátor v systéme overovania spoločnosti Microsoft 

- **component_name** – názov súčasti/zobrazenia, ktoré je aktívne počas filtrovania

- **event_mode** – umiestnenie v aplikácii, kam zadal používateľ konverzáciu (skupiny alebo iné)

- **internet_message_id** – ID sledovania pre najnovšiu správu v konverzácii
      
- **orientation** – orientácia obrazovky v čase udalosti (na výšku alebo na šírku)

- **recent_message_id** – ID najnovšej správy v konverzácii

- **suggested_reply_state** – stav navrhovaných odpovedí pre túto konverzáciu (nedostupné, dostupné, zobrazené, použité alebo zahodené)

- **suggested_reply_types** – označuje typ a počet navrhovaných odpovedí zobrazených/použitých pre túto konverzáciu. Ide o slovník. Príklad {text: 2, send_avail: 1}.
  
- **total_count** – celkový počet snímok zobrazených súčasťou
 
- **view_duration** – ako dlho mal používateľ zobrazenú súčasť

#### <a name="saveattempt"></a>save.attempt

Umožňuje identifikovať vplyv problémov spôsobených používateľmi pokúšajúcimi sa uložiť súbor vyhodnotením počtu ovplyvnených relácií a toho, či existujú spoločné prvky týchto relácií.

Zhromažďujú sa tieto polia: 

- **file_type** – typ súboru, ktorý sa používateľ pokúsil uložiť (napríklad .doc)

- **origin** – označuje umiestnenie pôvodu pokusu o uloženie súboru (napríklad z e-mailu), aby sme mohli zistiť problémy s ukladaním súboru z určitého umiestnenia v aplikácii

- **token_type** – typ tokenu slúžiaci na overenie konta s cieľom uloženia súboru, aby sme mohli zistiť problémy s overovaním týkajúce sa ukladania súboru

#### <a name="searchsubtabselected"></a>search.subtab.selected

Udalosť zhromažďuje miesta pôvodu z dôvodu, že ste vybrali podkartu vyhľadávania. Podkarty sa nachádzajú pod primárnym panelom vyhľadávania aplikácií na filtrovanie údajov. Táto akcia nám umožňuje sledovať typ entity (všetko, pošta, kontakty a kalendár), ktorý používatelia používajú pri vyhľadávaní, aby sme mohli zabezpečiť, že mechanizmy filtrovania vyhľadávania fungujú správne.

Zhromažďujú sa tieto polia:

- **properties_general** – všeobecné vlastnosti, ktoré zhromažďujú všetky udalosti Aria

- **selected_reason** – príčina vybratia typu, čo môže byť niektorá z týchto hodnôt (glyph je ikona): tap_on_header, tap_on_see_all, enter_search_mode, mail_glyph, calendar_glyph.

- **subtab_type** – typ, ktorý sa vybral, čo môže byť niektorá z týchto štyroch hodnôt: všetko, pošta, kontakt, udalosť.

#### <a name="sendmessage"></a>send.message

Slúži na sledovanie možného nepriaznivého vplyvu na výkon a stav odosielania e-mailových správ.

Zhromažďujú sa tieto polia:
  
- **account** – sleduje konto, v ktorom sa akcia vykonala

- **compose_duration** – sleduje celkový čas, ktorý používateľ strávil vytváraním správy vrátane viacerých relácií konceptov

- **draft_message_id** – sleduje ID odosielanej vytvorenej správy

- **event_mode** – sleduje režim udalosti, ak sa vzťahuje na správu, („skupiny“ alebo „iné“)

- **has_attachment** – označuje, či správa obsahuje prílohy

- **has_mip_label** – označuje, či bola na správe označená značka MIP

- **is_group_escalation** – označuje, či ide o skupinovú eskalovanú správu, „eskalovaná správa“ je správa, ktorá bola odoslaná do poštovej schránky používateľa z dôvodu eskalácie (odber skupiny).

- **is_groups** – sleduje, či je odoslaná správa skupinová správa alebo nie

- **key_stroke_count** – sleduje počet stláčania klávesov v odosielanej správe

- **message_id** – sleduje ID správy, na ktorú sa odpovedá alebo ktorá sa preposiela

- **origin** – označuje miesto spustenia vytvárania, t. j. nové, odpoveď, rýchla odpoveď atď.

- **send_draft_origin** – označuje miesto spustenia odoslania, t. j. vytvorenie alebo rýchla odpoveď

- **smart_compose_model_version** – sleduje, aká verzia modelu inteligentného písania sa používa

- **source_inbox** – označuje typ zdrojovej doručenej pošty pre referenčnú správu, 

- **suggested_reply_state** – zachytáva stav navrhovanej odpovede pre odoslanú poštu, t. j. nedostupné, dostupné, zobrazené, použité alebo zahodené

- **suggested_reply_types** – označuje typ a počet navrhovaných odpovedí zobrazených/použitých pre tento odoslaný e-mail. Ide o slovník. Príklad {text: 2,  send_avail: 1}.

- **suggestions_requested** – udáva počet požadovaných návrhov inteligentného písania

- **suggestions_results** – výsledok návrhov inteligentného písania, t. j. prijaté, odmietnuté

- **suggestions_returned** – udáva počet návrhov inteligentného písania vrátených zo servera

- **suggestions_shown** – udáva počet návrhov inteligentného písania zobrazených používateľovi

- **thread_id** – označuje ID vlákna konverzácie, na ktorú sa odpovedá alebo ktorá sa preposiela

#### <a name="session"></a>session

Umožňuje zistiť a vyriešiť situácie prílišného využívania batérie zariadenia a pomáha zistiť možnú príčinu.

Zhromažďujú sa tieto polia: 

- **battery_level** – uvádza úroveň nabitia batérie zariadenia, aby sme mohli určiť, kedy naša aplikácia negatívne vplýva na úroveň nabitia batérie zariadenia

- **has_hx** – uvádza, že konto používa našu novú službu synchronizácie, aby sme mohli zistiť problémy spôsobené touto službou

- **Session.Duration** – dĺžka relácie v sekundách

- **Session.DurationBucket** – sektor dĺžky času trvania *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **Session.FirstLaunchTime** – prvý zaznamenaný čas spustenia aplikácie *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **Session.State** – indikátor, či ide o začiatok alebo koniec relácie

#### <a name="settingsaction"></a>settings.action

Táto udalosť zhromažďuje informácie o konfigurácii v nastaveniach. Tieto údaje umožňujú zistiť situácie, ktoré môžu mať nepriaznivý vplyv na schopnosť používateľov konfigurovať nastavenia aplikácie, ako sú napríklad nastavenia oznámení, primárneho e-mailového konta a konfigurácia podpisu v e-mailoch.

Zhromažďujú sa tieto polia: 

- **account_order_changed** – kontroluje, či ste zmenili poradie kont na zabezpečenie správneho fungovania tejto konfigurácie 

- **action** – možné akcie v nastaveniach ako napríklad odstránenie konta, aby sme mohli zistiť problémy a vylúčiť nepriaznivý vplyv

- **auth_type** – typ overenia používaného v konte, vďaka ktorému zistíme, ktorú vrstvu synchronizácie servera používame, čo nám pomôže pri diagnostikovaní problémov 

- **changed_folder** – zaznamenáva, či sa zmenil priečinok, čo pomáha pri diagnostikovaní problémov. 

- **delete_scope** – počas odstránenia konta označuje, či ste konto odstránili z tohto zariadenia alebo zo všetkých zariadení s Outlookom.  

- **enabled_state** – označuje, či sú správne nakonfigurované nastavenia automatických odpovedí, ukladania kontaktov a blokovania externých obrázkov  

- **notification_action** – slúži na kontrolu, či ste nakonfigurovali nejaké akcie oznámení na triedenie e-mailov, aby sme mohli zabezpečiť správne fungovanie tohto nastavenia 

- **notification_action_number** – na kontrolu, či sú akcie oznámení (prvá akcia alebo druhá akcia) nakonfigurované správne

- **server_type** – podobne ako auth_type uvádza, aký typ konta máte s cieľom lepšej diagnostiky problémov.  Príklady: Office365, Gmail, Outlook

- **setting_properties** – sleduje vzťah vlastností k akcii nastavenia, podrobnosti sú uvedené nižšie: 
   - **alternate_app_icon_setting** – vybratá alternatívna ikona aplikácie (svetlá, tmavá)
   - **auth_type** – označuje typ overenia servera, vďaka ktorému zistíme, či sa vyskytol problém s určitým typom konta
   - **badge_count_state** – označuje, o aký počet štítkov používateľ požiadal, t. j. žiadne štítky, iba prioritná doručená pošta atď. 
   - **changed_folder** – určuje, či bola táto akcia archivovaná, plánovaná alebo to bola iná akcia.
   - **delete_scope** – sleduje, či sa táto akcia týkala odstránenia osoby v tomto zariadení alebo vo všetkých zariadeniach (ak je k dispozícii). 
  - **enabled_state** – označuje, či je povolený stav súvisiaci s akciou
  - **in_app_language** – vybratý jazyk v aplikácii, typ reťazca (predvolený, en-US, fa, ru atď.)
  - **notification_action_setting** – označuje podrobnosti nastavení akcie oznámení súvisiace s touto akciou (ak je k dispozícii)
    - **notification_action** – označuje, čo sa používateľ pokúšal urobiť, t. j. označiť príznakom, odstrániť, archivovať, umožňuje zistiť, akú akciu správy chcel používateľ vykonať na oznámení a či zlyhala alebo nie. 
    - **notification_action_number** – označuje, ktoré číslo akcie (dve z troch akcií sú prispôsobiteľné) bolo priradenej akcii s oznámením, t. j. (prvá akcia alebo druhá akcia). Umožňuje nám to zistiť, či sa vyskytol problém s určitou akciou.
   - **notification_state** – označuje, o aký typ počtu štítkov používateľ požiadal, t. j. žiadne štítky, iba prioritná doručená pošta atď.
   - **server_type** – označuje typ servera, vďaka ktorému zistíme, či sa vyskytol problém s určitým typom servera
   - **source** – označuje, čo je v nastaveniach alebo nastavení nerušiť zdrojom oznámení (ak je k dispozícii)
   - **swipe_setting** – označuje podrobnosti nastavení potiahnutia prstom súvisiace s touto akciou (ak je k dispozícii)
     - **swipe_action** – označuje, čo sa používateľ pokúšal urobiť, t. j. označiť príznakom, odstrániť, archivovať, umožňuje zistiť, akú akciu chcel používateľ vykonať a či zlyhala alebo nie. 
     - **swipe_direction** – označuje smer, ktorým používateľ nastavil potiahnutie prstom, t. j. zľava doprava alebo sprava doľava. Umožňuje nám to zistiť, či sa vyskytol problém s určitým smerom potiahnutia prstom.
   - **temperature_unit_setting** – vybratá jednotka teploty, ktorá sa použije na počasie 
   - **theme_color_setting** – vlastná farba motívu aplikácie vybratá používateľom 
   - **ui_mode_setting** – vybraný režim používateľského rozhrania (tmavé, svetlé, predvolené systémom, vybitá batéria atď.)
   - **signature_setting** – označuje, či sa nastavenie použilo na všetky kontá alebo na jedno konto

- **state_changed_to** – slúži na kontrolu, či máte správne nakonfigurované nastavenie zapnúť/vypnúť prioritnej doručenej pošty 

- **swipe_action** – slúži na kontrolu, či ste nakonfigurovali nejaké akcie potiahnutia na triedenie e-mailov, aby sme mohli zabezpečiť správne fungovanie tohto nastavenia 

- **swipe_direction** – slúži na kontrolu, či boli pokyny na potiahnutie prstom (vľavo alebo vpravo) nakonfigurované správne


#### <a name="sidebaraction"></a>sidebar.action

Umožňuje zistiť situácie, ktoré môžu mať nepriaznivý vplyv na vašu schopnosť konfigurovať nastavenia aplikácie, ako sú napríklad nastavenia oznámení, primárneho e-mailového konta a konfigurácia podpisu v e-mailoch.

Údajové polia, ktoré sú bežné pre aplikáciu Outlook Mobile pre túto udalosť v zariadeniach so systémom iOS a Android:

- **Account** – sleduje konto a jeho údaje priradené k udalosti, hodnoty sledované v tomto údaji sa nachádzajú v spoločnej dokumentácii poľa *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **action** – sleduje typ akcie bočného panela, t. j. zamietnuté, vybraté tlačidlo Pomocník, bočný panel pošty atď., 

- **from_favorites** – sleduje, či akcia pochádza z položky v priečinku Obľúbené položky 

- **mail_folder_type** – aký typ priečinka bol vybraný pri akcii bočného panela (ak bol nejaký vybraný).

- **sidebar_type** – sleduje typ bočného panela, ktorý je priradený k tejto udalosti, t. j. pošta alebo kalendár, aby sme mohli zabezpečiť správne fungovanie navigácie v nastavení obľúbených položiek

Zhromažďujú sa tieto polia: 

- **account_type** – označuje typ overenia konta, t. j. Gmail, Outlook atď. 

- **account_has_groups** – pomáha so správnou konfiguráciou skupín, ak sa nachádzajú v konte

- **calendar_accounts_count** – počet kont kalendára, ktorý nám pomôže so správnou konfiguráciou kont kalendára 

- **calendar_apps_count** – počet aplikácií kalendára, ktorý nám pomôže so správnou konfiguráciou aplikácií zaujímavého kalendára 

- **calendar_type** – typ kalendára, ktorý vlastníte (primárny kalendár, kalendár skupiny atď.) 

- **has_favorite_folders** – pomáha so správnou konfiguráciou obľúbených priečinkov 

- **has_favorite_people** – pomáha so správnou konfiguráciou obľúbených ľudí/kontaktov 

- **has_group_calendar** – pomáha so správnou konfiguráciou kalendárov skupín, ak ich máte 

- **has_group_calendar_account** – pomáha nám so správnou konfiguráciou kalendárov skupín, ak ich máte 

- **has_group_toggled** – pomáha so správnou konfiguráciou v prípade prepnutia kalendárov skupín 

- **interesting_calendars_accounts_count** – počet kont zaujímavého kalendára, ktorý nám pomôže so správnou konfiguráciou kont zaujímavého kalendára 

- **mail_accounts_count** – celkový počet e-mailových kont v bočnom paneli na zabezpečenie správnej konfigurácie 

- **mail_folder_type** – typ priečinka, na ktorý používateľ ťukol, aby sa zabezpečila správna konfigurácia Môže to byť napríklad odstránený priečinok, nevyžiadaná pošta alebo priečinok odoslanej pošty. 

- **mail_inbox_unread_count** – pomáha zabezpečiť, aby bol správne zobrazený a nakonfigurovaný počet neprečítaných správ 

- **mail_subfolder_depth** – pomáha zabezpečiť úspešné zobrazenie konfigurácií poštového podpriečinka používateľa

#### <a name="storeop"></a>StoreOp

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM.  Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú pri vykonávaní operácie priestoru na ukladanie licencií služby správy prístupových práv. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.ContentId** – ID obsahu v licencii koncového používateľa.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z operácie, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.OperationName** – názov operácie

- **RMS.Result** – úspech alebo zlyhanie operácie.

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu výsledku operácie.

- **RMS.Url** – URL adresa servera služby správy prístupových práv.

#### <a name="watchappv2"></a>watchAppV2

Táto udalosť umožňuje zistiť a vyriešiť možné problémy s možnosťami hodiniek Apple Watch, ako je napríklad prijímanie oznámení a odpovedanie na e-maily.

Zhromažďujú sa tieto polia: 

- **app_action** – uvádza typy akcií, ktoré používateľ vykonal v hodinkách Apple Watch, napríklad „archive_message“, aby sme mohli zistiť problémy s konkrétnou akciou, ako je napríklad neschopnosť úspešne archivovať správy v hodinkách Apple Watch

- **is_watch_app_installed** – uvádza, či používateľ nainštaloval aplikáciu Apple Watch vo svojom zariadení

- **is_complication_enabled** – uvádza, či si používateľ pridal Outlook na obrazovku hodiniek Apple Watch, aby sme mohli zistiť problémy s obrazovkami hodiniek Apple Watch

- **watch_os** – uvádza nainštalovanú verziu operačného systému hodiniek Apple Watch, aby sme mohli zistiť problémy s konkrétnymi verziami operačného systému hodiniek Apple Watch


### <a name="application-status-and-boot-subtype"></a>*Podtyp Stav aplikácie a podtyp spustenia*

Určenie, či sa vyskytli konkrétne udalosti funkcie, napríklad spustenie alebo ukončenie, a či je funkcia spustená.

#### <a name="appstartup"></a>app.startup

Táto udalosť nám umožňuje zistiť a vyriešiť problémy spôsobujúce pomalé alebo neúplné spúšťanie Outlooku, čo používateľom sťažuje používanie aplikácie.  Patria sem informácie o konkrétnych povolených funkciách a o dĺžke trvania spustenia konkrétnych častí.

Zhromažďujú sa tieto polia: 

- **attach_base_context_millis** – čas medzi začiatkom základného kontextu a onCreate()

- **device_ram_in_mb** – pamäť RAM dostupná v zariadení

- **has_company_portal** – označuje, či je nainštalovaná aplikácia Company Portal

- **hx_okhttp_mode** – označuje, či sa pri odosielaní a prijímaní sieťových požiadaviek protokolu HTTP používa súčasť novej služby na synchronizáciu e-mailov

- **initial_activity_name** – aktivita operačného systému Android, ktorá spustila aplikáciu

- **manufacturer** – výrobca zariadenia

- **model** – model zariadenia

- **on_create_millis** – čas potrebný v metóde onCreate()

- **on_resume_millis** – čas potrebný v metóde onResume()

- **time_until_attach** čas medzi načítaním triedy a začiatkom základného kontextu

- **total_millis** – celkový čas od začiatku načítania triedy po dokončenie obnovenia aktivity operačného systému Android

#### <a name="boottime"></a>boot.time 

Táto udalosť umožňuje zistiť výskyt kritických chýb aplikácie, ktoré by mohli spôsobiť jej zlyhanie alebo závažné problémy, ako je napríklad zobrazenie prázdnych riadkov v doručenej pošte. Táto udalosť zhromažďuje informácie, ktoré umožňujú kategorizovať a klasifikovať problémy, vďaka čomu dokážeme uprednostniť vplyv problémov na zákazníkov.

Zhromažďujú sa tieto polia:

- **black_list_reason** – uvádza, či existuje dôvod na ignorovanie týchto údajov. Medzi príklady patrí spustenie v dôsledku vzdialeného oznámenia a spustenie v dôsledku načítania na pozadí.

- **step_premain** – – uvádza čas, ktorý v Outlooku uplynul, odkedy používateľ ťukol na ikonu, po krok step0_main, „hlavný“ krok definovaný v tomto dokumente.

- **step0_main** – uvádza čas, ktorý Outlook potreboval na presun do „hlavného“ kroku, ktorý definuje spoločnosť Apple.

- **step1_appWillFinishLaunching** – uvádza čas, ktorý Outlook potreboval na prechod z „hlavného“ kroku do kroku „appWillFinishLaunching“, ktorý definuje spoločnosť Apple.

- **step2_appDidFinishLaunching** – uvádza čas, ktorý Outlook potreboval na prechod z kroku „appWillFinishLaunching“ do kroku „appDidFinishLaunching“, ktorý definuje spoločnosť Apple.

- **step3_engineStarted** – uvádza čas, ktorý Outlook potreboval na prechod z kroku „appDidFinishLaunching“ k spusteniu nástroja aplikácie, ktorý ukladá a synchronizuje údaje.

- **step4_runLoopFirstIdle** – uvádza čas, ktorý Outlook potreboval na prechod z kroku „engineStarted“ do stavu bez ďalších krokov.

- **total_time** – uvádza celkový čas, ktorý Outlook potreboval na dokončenie procesu spustenia.

#### <a name="dnslookupop"></a>DnsLookupOp

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM.  Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú pri vykonávaní operácie vyhľadania informácií o serveri DNS. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.Duration** – celkový čas na dokončenie operácie.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z operácie, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.NoOfDomainsSearched** – Počet prehľadaných domén.    

- **RMS.NoOfDomainsSkipped** – Počet vynechaných domén. 

- **RMS.Result** – úspech alebo zlyhanie operácie.

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu výsledku operácie.

#### <a name="firstvisible"></a>first.visible

Táto udalosť nám umožňuje zistiť, kedy bola aplikácia prvýkrát zámerne spustená používateľom. Táto udalosť sa vyžaduje, aby sa zaistilo, že aplikácia úspešne funguje v zostavách OEM (Original Equipment Manufacturer).

Zhromažďujú sa tieto polia:

- **is_oem** – pole sledovania, ktoré označuje, či je aplikácia spustená na variante OEM

- **is_system_install** – pole sledovanie prítomnosti predinštalovaného súboru vlastností, ktorý by mal určovať, že táto inštalácia je OEM 

- **manufacturer** – výrobca zariadenia

- **model** – model zariadenia

- **systemFlagSet** – hodnota príznaku systému Android (ApplicationInfo.FLAG_SYSTEM), ktorá označuje, či bola aplikácia nainštalovaná ako súčasť obrazu systému zariadenia

#### <a name="getuserop"></a>GetUserOp

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM.  Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú pri vykonávaní operácie získavania používateľských certifikátov. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.ContentId** – ID obsahu.

- **RMS.Duration** – celkový čas na dokončenie operácie.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z operácie.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.Result** – úspech alebo zlyhanie operácie.

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu výsledku operácie.

- **RMS.Type** – typ používateľských informácií.

#### <a name="httpop"></a>HttpOp

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM.  Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú pri vykonávaní operácie požiadavky http.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.
    
- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.CallBackStatus** – stav vráteného výsledku spätného volania overovania.

- **RMS.CallbackTime** – čas trvania spätného volania overovania. 

- **RMS.CorrelationId** – ID korelácie požiadavky http

- **RMS.DataSize** – veľkosť údajov požiadavky HTTP

- **RMS.Duration** – celkový čas na dokončenie operácie.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z operácie, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha vnorená operácia HTTP. 

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.OperationName** – názov operácie.

- **RMS.Result** – úspech alebo zlyhanie operácie.

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu výsledku operácie.

- **RMS.Url** – URL adresa servera služby správy prístupových práv.

- **RMS.WinhttpCallbackStatus** – stav výsledku spätného volania winhttp.

#### <a name="initialized"></a>Initialized

Umožňuje analyzovať stav rozhrania, ktoré umožňuje mobilným aplikáciám načítať nastavenia používateľov a ochrany osobných údajov v službách Office a diagnostikovať problémy s pripojiteľnosťou a nastavením ochrany osobných údajov.

Zhromažďujú sa tieto polia:

- **roamingSettingType** – identifikuje umiestnenie, z ktorého sa pokúšame čítať nastavenia

#### <a name="ipccreateoauth2token"></a>IpcCreateOauth2Token

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcCreateOauth2Token.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.
    
- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.


#### <a name="officeandroidaccountstorageinfo"></a>Office.Android.AccountStorageInfo

Táto udalosť určuje počet kont MSA a ADAL v databáze Registry a zdieľaných preferenciách. Umožňuje analýzu nezrovnalostí medzi ukladacím priestorom údajov a pomáha nám stabilizovať výkon aplikácií.

Zhromažďujú sa tieto polia:

- **RegistryADALCount** – označuje počet kont ADAL v databáze Registry.

- **RegistryLiveIdCount** – označuje počet kont MSA v databáze Registry.

- **SharedPrefADALCount** – označuje počet kont ADAL v zdieľaných preferenciách.

- **SharedPrefLiveIdCount** – označuje počet kont MSA v zdieľaných preferenciách.


#### <a name="officeandroidandroidoffice16bootlatency"></a>Office.Android.AndroidOffice16BootLatency

Dôležité pri zachytávaní metriky výkonu aplikácie s ohľadom na čas odozvy aplikácie od spustenia.  Spoločnosť Microsoft používa túto možnosť na zber času potrebného na odozvu aplikácie a tiež na zisťovanie scenárov, ktoré môžu mať vplyv na čas spustenia v aplikáciách Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **AppLaunchResponsiveTimeInMilliSec** – čas odozvy spustenia aplikácie

- **AppSuspendedDuringBoot** – Boolovská hodnota, ktorá označuje, či bola aplikácia pozastavená počas štartu

- **CollectionTime** – čas udalosti

- **FileActivationAttempted** – Boolovská hodnota, ktorá označuje, či došlo k pokusu o aktiváciu súboru

- **FirstIdleOnAppThreadTimeInMilliSec** – čas nečinnosti vlákna aplikácie

- **IsThisFirstLaunch** – Boolovská hodnota, ktorá označuje, či ide o prvé spustenie aplikácie

- **UserDialogInterruptionDuringBoot** – Boolovská hodnota, ktorá označuje, či sa počas štartu zobrazilo nejaké blokujúce používateľské rozhranie

#### <a name="officeextensibilityofficejsappactivated"></a>Office.Extensibility.OfficeJS.Appactivated

Táto udalosť zaznamenáva informácie o neočakávaných vypnutiach balíka Office. Umožňuje nám to identifikovať zlyhania alebo nereagovania v produkte, aby ich bolo možné riešiť.

Zhromažďujú sa tieto polia:

  - **Data\_AirspaceInitTime:integer** – čas potrebný na inicializovanie komponentu Airspace balíka Office

  - **Data\_AllShapes:integer** – počet tvarov v dokumente

  - **Data\_APIInitTime:integer** – čas potrebný na inicializovanie modulu API Visia

  - **Data\_AppSizeHeight** – výška okna doplnku

  - **Data\_AppSizeWidth** – šírka okna doplnku

  - **Data\_AppURL** – URL adresa doplnku; zaznamenáva úplnú URL adresu doplnkov z obchodu a URL doménu pre doplnky, ktoré nie sú z obchodu.

  - **Data_Doc_AsyncOpenKind:long** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data\_AuthorsCount:integer** – počet autorov, ktorí upravovali dokument v tejto relácií.

  - **Data\_BackgroundPages:integer** – počet strán na pozadí v diagrame

  - **Data\_BootTime:integer** – čas potrebný na spustenie Visia

  - **Data\_Browser** – reťazec prehliadača s informáciami o prehliadači, ako sú napríklad typ a verzia

  - **Data\_ChildWindowMixedModeTime:integer** – čas potrebný na zapnutie zmiešaného režimu vo Visiu (podriadené okno môže mať iné DpiAwareness z nadradeného okna)

  - **Data\_CommentsCount:integer** – počet komentárov v dokumente

  - **Data\_ConnectionCount:integer** – počet pripojení údajov v diagrame

  - **Data\_ContentMgrInitTim:integer** –čas potrebný na inicializovanie správcu obsahu

  - **Data\_CreateMainFrameTime:integer** – vytvorenie času hlavného rámu

  - **Data\_CreatePaletteTime:integer** – čas potrebný na vytvorenie globálnej palety farieb

  - **Data\_DispFormatCount:integer** – počet údajových grafík v diagrame

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Fqdn:string** – miesto uloženia dokumentu (SharePoint.com, live.net), k dispozícii len pre domény v Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IsIncrementalOpen:bool** – či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnutia celého dokumentu)

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – či sa dokument otvára z lokálnej vyrovnávacej pamäte

  - **Data\_Doc\_IsSyncBacked:bool** – má hodnotu true, ak ide o serverový dokument, ktorý existuje lokálne a je synchronizovaný so serverom (napr. prostredníctvom klientskej aplikácie OneDrive alebo ODB)

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude.

  - **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

  - **Data\_Doc\_ServerDocId:string** – nemenný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – dlhá bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_SyncBackedType** – indikátor typu dokumentu (lokálny alebo v službe) 

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_DpiAwarenessTime:integer** – čas potrebný na zapnutie funkcie Per Monitor Dpi Awareness

  - **Data\_DurationToCompleteInMilliseconds:double** – čas potrebný na dokončenie funkcie Uložiť ako v milisekundách

  - **Data\_ErrorCode:int** – 0 pre úspech, celé číslo pre zlyhanie pri ukladaní

  - **Data\_FailureReason:integer** – dôvod zlyhania asynchrónneho ukladania

  - **Data\_FileExtension** – prípona súboru otvoreného diagramu

  - **Data\_FileHasDGMaster:bool** – má hodnotu true, keď súbor obsahuje údajovú grafiku

  - **Data\_FileHasImportedData:bool** – má hodnotu true, keď súbor obsahuje importované údaje

  - **Data\_FileHasShapesLinked:bool** – má hodnotu true, keď súbor má prepojené tvary na údaje

  - **Data\_FileIOBytesRead:int** – celkový počet bajtov prečítaných počas ukladania

  - **Data\_FileIOBytesReadSquared:int** – druhá mocnina poľa Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten:int** – celkový počet bajtov zapísaných počas ukladania

  - **Data\_FileIOBytesReadWritten:int** – druhá mocnina poľa Data\_FileIOBytesWritten

  - **Data\_FilePathHash:binary** – binárna hodnota hash cesty k súboru

  - **Data\_FilePathHash: binary** – identifikátor GUID cesty k súboru

  - **Data\_FileSize** – veľkosť dokumentu v bajtoch

  - **Data\_ForegroundPages:integer** – počet strán v popredí v diagrame

  - **Data\_ForegroundShapes:integer** – celé číslo počtu tvarov na stranách v popredí

  - **Data\_GdiInitTime:integer** – čas potrebný na inicializovanie modulu GDI

  - **Data\_HasCoauthUserEdit:bool** – má hodnotu true, ak dokument bol upravený v relácii spolutvorby

  - **Data\_HasCustomPages:bool** – má hodnotu true, ak dokument obsahuje vlastné strany

  - **Data\_HasCustPatterns:bool** – má hodnotu true, ak súbor obsahuje vlastné vzory

  - **Data\_HasDynConn:bool** – má hodnotu true, ak dokument obsahuje dynamické pripojenie.

  - **Data\_HasScaledPages:bool** – má hodnotu true, ak dokument obsahuje strany so zmenou mierky

  - **Data\_HasUserWaitTime:bool** – má hodnotu true, ak sa počas ukladania zobrazí dialógové okno súboru

  - **Data\_InitAddinsTime:integer** – čas potrebný na inicializovanie a načítanie COM Add

  - **Data\_InitBrandTime:integer** – čas potrebný na inicializovanie úvodnej obrazovky a značkových komponentov balíka Office

  - **Data\_InitGimmeTime:integer** – čas potrebný na inicializovanie komponentu balíka Office

  - **Data\_InitLicensingTime:integer** – čas potrebný na inicializovanie licenčného komponentu balíka Office

  - **Data\_InitMsoUtilsTime:integer** – čas inicializovania komponentu MSOUTILS balíka Office

  - **Data\_InitPerfTime:integer** – čas inicializovania komponentu Performance balíka Office

  - **Data\_InitTCOTime:integer** – čas potrebný na inicializovanie správcu komponentov balíka Office

  - **Data\_InitTrustCenterTime:integer** – čas potrebný na inicializovanie komponentu centra dôveryhodnosti balíka Office

  - **Data\_InitVSSubSystemsTime:integer** – čas potrebný na inicializovanie komponentov Visia

  - **Data\_InternalFile:bool** – má hodnotu true, ak súbor je interný. Napríklad vzorkovnica

  - **Data\_IsAsyncSave:bool** – má hodnotu true, ak ukladanie bolo asynchrónne

  - **Data\_IsAutoRecoveredFile:bool** – má hodnotu true, ak súbor bol automaticky obnovený

  - **Data\_IsEmbedded:bool** – má hodnotu true, ak súbor Visia bol vložený v inej aplikácii

  - **Data\_IsInfinitePageDisabledForAllPages:bool** – určuje, či je funkcia Infinite Page zakázaná pre všetky strany v dokumente

  - **Data\_IsIRMProtected:bool** – má hodnotu true, ak súbor je chránený technológiou IRM

  - **Data\_IsLocal:bool** – má hodnotu true, ak súbor je lokálny

  - **Data\_IsRecoverySave:bool**  – má hodnotu true, ak sa ukladanie spustilo z dôvodu obnovenia

  - **Data\_IsShapeSearchPaneHiddenState:bool** – má hodnotu true, ak bola tabla vyhľadávania tvaru skrytá pre dokument

  - **Data\_IsSmartDiagramPresentInActivePageOfFile:bool** – má hodnotu true, ak sa vizuálny diagram inteligentných údajov nachádza na aktívnej strane súboru

  - **Data\_IsSmartDiagramPresentInFile:bool** – má hodnotu true, ak sa vizuálny diagram inteligentných údajov nachádza v súbore

  - **Data\_IsUNC:bool** – má hodnotu true, ak cesta k súboru je v súlade s konvenciou UNC

  - **Data\_LandscapePgCount:integer** – počet strán s orientáciou na šírku v diagrame

  - **Data\_Layers:integer** – počet vrstiev v diagrame

  - **Data\_LoadProfileTime:integer** – počas potrebný na načítanie nástroja na profilovanie balíka Office

  - **Data\_LoadRichEditTim:integer** – čas načítania komponentu Rich edit

  - **Data\_LoadVisIntlTime:integer** – čas potrebný na načítanie medzinárodnej knižnice DLL Visia

  - **Data\_Location:integer** – umiestnenie súboru, z ktorého bol otvorený, 0 lokálny, 1 sieť, 2 SharePoint, 3 web

  - **Data\_MasterCount:integer** – počet predlôh v diagrame

  - **Data\_MaxCoauthUsers:integer** – maximálny počet používateľov spolutvoriacich v ľubovoľnom čase v relácii Filesystem, Registry, First Party, SDX

  - **Data\_MaxTilesAutoSizeOn:integer** – maximálny počet dlaždíc strany, pre ktoré bola automatická veľkosť povolená

  - **Data\_MsoBeginBootTime:integer** čas spustenia MSO

  - **Data\_MsoDllLoadTime:integer** – čas potrebný na načítanie knižnice DLL MSO

  - **Data\_MsoEndBootTime:integer** – čas potrebný na dokončenie spúšťania MSO

  - **Data\_MsoInitCoreTime:integer** – čas potrebný na spustenie komponentu balíka Office MSO

  - **Data\_MsoInitUITime:integer** – čas potrebný na spustenie používateľského rozhrania komponentu balíka Office MSO

  - **Data\_MsoMigrateTime:integer**  – čas potrebný na migrovanie nastavení používateľa pri prvom spustený, ak používateľ inovoval z predchádzajúcej verzie

  - **Data\_NetworkIOBytesRead:int** – celkový počet sieťových bajtov prečítaných počas ukladania

  - **Data\_NetworkIOBytesReadSquared:int** – druhá mocnina poľa Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten:int** – celkový počet sieťových bajtov zapísaných počas ukladania

  - **Data\_NetworkIOBytesWrittenSquared: int** – druhá mocnina poľa NetworkIOBytesWritten

  - **Data\_OartStartupTime:integer** – čas potrebný na inicializovanie komponentu balíka Office OART

  - **Data\_OleInitTime:integer** – čas inicializovania komponentu OLE balíka Office

  - **Data\_OpenDurationTimeInMs:integer** – čas do otvorenia súboru v milisekundách

  - **Data\_OriginatedFromTemplateID:integer** – identifikátor šablóny, z ktorej bol vytvorený diagram. NULL pre šablóny tretích strán

  - **Data\_Pages:integer** – počet strán v dokumente

  - **Data\_PositionToolbarsTime:integer** – čas potrebný na umiestnenie panelov s nástrojmi na svoje miesto

  - **Data\_ReadOnly:bool** – má hodnotu true, ak súbor je len na čítanie

  - **Data\_RecordSetCount:integer** – počet množín záznamov v diagrame

  - **Data\_RecoveryTime:integer** – čas potrebný na otvorenie súborov obnovenia

  - **Data\_ReviewerPages:integer** – počet strán recenzentov v diagrame

  - **Data\_RibbonTime:integer** – čas potrebný na zobrazenie stavového riadka

  - **Data\_RoamingSettingsStartupTime:integer** – čas potrebný na vytvorenie a načítanie všetkých momentálne prenesených nastavení Visia

  - **Data\_SchemeMgrStartupTime:integer** – čas potrebný na inicializovanie správcu schémy

  - **Data\_SDX\_AssetId** – existuje LEN pre doplnky z obchodu. OMEX priradí doplnku AssetId, keď sa zaradí do obchodu

  - **Data\_SDX\_BrowserToken** – identifikátor, ktorý sa nachádza vo vyrovnávacej pamäti prehliadača

  - **Data\_SDX\_HostJsVersion** – verzia Office.js špecifická pre platformu (napr. outlook web16.01.js). Obsahuje povrch rozhrania API pre doplnky

  - **Data\_SDX\_Id** – identifikátor GUID doplnku, ktorý ho jedinečne identifikuje

  - **Data\_SDX\_InstanceId** – predstavuje pár dokumentov k doplnku

  - **Data\_SDX\_MarketplaceType** – označuje, odkiaľ bol doplnok nainštalovaný

  - **Data\_SDX\_OfficeJsVersion** – toto je verzia Office.js, ktorá sa presmeruje na verziu špecifickú pre platformu.

  - **Data\_SDX\_Version** – verzia doplnku

  - **Data\_ShellCmdLineTime:integer** – čas potrebný na analyzovanie a vykonanie príkazov jadra na príkazovom riadku

  - **Data\_Size:long** – veľkosť súboru v bajtoch

  - **Data\_StartEndTransactionTime:integer** – čas potrebný na inicializovanie komponentov Visia

  - **Data\_STNInitTime:integer** – čas potrebný na inicializovanie konfigurácie okna vzorkovnice

  - **Data\_Tag:string** – jedinečný identifikátor na identifikáciu udalosti Uložiť ako

  - **Data\_ThemeCount:integer** – počet motívov v diagrame

  - **Data\_TimeStamp** – časová pečiatka času zavretia dokumentu

  - **Data\_UIInitTime:integer** – čas inicializovania používateľského rozhrania

  - **Data\_WasSuccessful:bool** – má hodnotu true, ak uloženie ako bolo úspešné

  - **Data\_WinLaunchTime:integer** – čas potrebný na spustenie úvodnej tably Visia atď.)

  
#### <a name="officeextensibilitysandboxodpactivationhanging"></a>Office.Extensibility.Sandbox.ODPActivationHanging

Zhromažďuje informácie, keď spúšťanie balíka Office trvá neočakávane dlho (> 5 sekúnd). Používa sa na zisťovanie a riešenie problémov so spúšťaním doplnkov balíka Office.
 
Zhromažďujú sa tieto polia:

- **AppID** – ID aplikácie.

- **AppInfo** – údaje týkajúce sa typu doplnku (pracovná tabla alebo režimu bez používateľského rozhrania alebo obsahu atď.) a typu poskytovateľa (omen, SharePoint, systém súborov atď.).

- **AppInstanceId** – ID inštancie aplikácie. 

- **AssetId** – ID položky aplikácie.

- **IsPreload** – označuje, či je doplnok predinštalovaný na pozadí na zlepšenie výkonu aktivácie

- **NumberOfAddinsActivated** – počítadlo aktivovaných doplnkov.

- **RemoterType** – špecifikuje typ služby Remoter (dôveryhodná, nedôveryhodná, Win32webView, dôveryhodná funkcia definovaná používateľom atď.), ktorý sa používa na aktiváciu doplnku.

- **StoreType** – pôvod aplikácie.

- **TimeForAuth** – čas strávený na overenie. 

- **TimeForSandbox** – čas strávený v Sandboxe.

- **TimeForServerCall** – čas strávený volaním servera. 

- **TotalTime** – celkový strávený čas.

- **UsesSharedRuntime** – označuje, či aplikácia používa sharedRuntime alebo nie.

#### <a name="officelenslenssdklaunchlens"></a>Office.Lens.LensSdk.LaunchLens

Keď používateľ spustí Lens na zachytenie alebo importovanie obrázkov v ľubovoľnej aplikácii, spustí sa súprava SDK Lensu a táto udalosť sa zhromaždí. Údaje spustenia nám pomáhajú určiť počet používateľov alebo zariadení, ktoré spúšťajú aplikáciu, a ďalej porozumieť používaniu funkcií. Pomáha to sledovať objem používateľov, ktorí produkt používajú, ako aj identifikovať zmeny trendov a vyhľadávať a riešiť problémy v produkte.

Zhromažďujú sa tieto polia:

- **Data_isResumeSession** – či bola aplikácia spustená ako pokračovanie alebo či ju používateľ spustil nanovo. (booleovské pole) 

- **Data_launchPerf** – celé číslo označujúce čas spúšťania aplikácie (v Androide)

- **Data_LaunchWorkFlowItem** – Pole určuje, či je aplikácia spustená z obrazovky fotoaparátu alebo obrazovky úprav. 

- **Data_mediaCompressionFactor** – faktor, ktorým sú obrázky skomprimované aplikáciou.

- **Data_RecoveryMode** – booleovské pole označujúce, či bola táto relácia obnovená po tom, ako bola aplikácia ukončená (v Androide)

- **IsDexModeEnabled** – booleovské pole označujúce, či zariadenie podporuje funkcie Samsung Dex.

- **IsEmbeddedLaunch** – booleovské pole označujúce, či používateľ spustil ovládací prvok v režime obrazu v obraze.

- **IsInterimCropEnabled** – booleovské pole označujúce, či sa používateľ rozhodol manuálne orezať každý obrázok.

- **IsMultiWindowEnabled** – booleovské pole označujúce, či je možné spustiť aplikáciu na rozdelenej obrazovke.

- **LaunchPerf** – celé číslo označujúce čas spúšťania aplikácie (v iOS)

- **RecoveryMode** – booleovské pole označujúce, či bola táto relácia obnovená po tom, ako bola aplikácia ukončená (v iOS)

- **SDKMode** – režim, v ktorom boli obrázky zachytené.


#### <a name="officeofficemobileappactivationlaunch"></a>Office.OfficeMobile.AppActivation.Launch

Táto udalosť identifikuje prvú a ďalšie aktivácie prostredníctvom externých spúšťačov, ktoré aktivujú aplikáciu. Aktivácia aplikácie načíta určité závislosti, ktoré sú zodpovedné za fungovanie aplikácie bez problémov a táto udalosť sa zaznamená, keď sa načíta úspešne. Tiež zaznamená zdroj aktivácie a zámer aplikácie, ktorý bol zodpovedný za aktiváciu aplikácie.

Zhromažďujú sa tieto polia:

- **ActionName** – celé číslo priradenia k názvu akcie/funkcie, ktorá je vyvolaná z bodu aktivácie.
 
- **ActivationType** – celé číslo priradenia k zdroju aktivácie
  
- **IsActionTriggered** – Boolovská hodnota určujúca, či sa akcia spustila po úspešnej aktivácii aplikácie.

- **IsFirstRun** – Boolovská hodnota určujúca, či išlo o prvé spustenie aplikácie alebo jej následné spustenie.
 

#### <a name="officeofficemobilefrefirstrunsetup"></a>Office.OfficeMobile.FRE.FirstRunSetup

Táto udalosť prezenčného signálu sa spustí pri prvom spustení aplikácie po inštalácii. Pomáha identifikovať inštalácie a automatické inovácie zo starších verzií aplikácie a umožňuje nám identifikovať chyby v automatických inováciách vrátane zlyhaní pri načítavaní knižníc a sťahovaní rozšírení/jazykových balíkov.

Zhromažďujú sa tieto polia:

- **IsFlightAssigned** – Boolovská hodnota určujúca, či používateľ bol súčasťou nejakej vopred priradenej skupiny funkcií, ktorá môže spôsobiť vystavenie určitým funkciám.

- **IsFRELoadSuccessful** – celé číslo uvádzajúce stav výsledku

#### <a name="officeonenoteandroidappappbootcomplete-officeandroidearlytelemetryappbootcomplete"></a>Office.OneNote.Android.App.AppBootComplete, Office.Android.EarlyTelemetry.AppBootComplete

*[Táto udalosť sa predtým nazývala OneNote.App.AppBootComplete.]*

Kritický signál, ktorý sa používa na zaistenie, že noví individuálni používatelia (konto Microsoft) môžu úspešne spustiť a používať OneNote po prvýkrát.  Používa sa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby.  Ak používatelia nemôžu spustiť aplikáciu po prvýkrát, môže to vyvolať incident s vysokou závažnosťou.

Zhromažďujú sa tieto polia: 

- **ACTIVITY_BOOT_TIME_IN_MS** – čas potrebný na dokončenie vytvorenia aktivity

- **ACTIVITY_NAME** – názov aktivity otvorenej pri spustení 

- **ANY_DIALOG_SHOWN** – označuje, či sa počas spúšťania zobrazí dialógové okno

- **APP_SUSPEND_DURING_EVENT** – označuje, či bolo spustenie preložené

- **APP_THREAD_CREATION_WAIT_TIME_TIME_FOR_APP_THREAD_CREATION** – čas potrebný na vytvorenie vlákien aplikácie

- **AVAILABLE_MEMORY_IN_MB** – celková pamäť dostupná v zariadení 

- **AVG_SNAPSHOT_POPULATION_TIME** – priemerný čas potrebný na načítanie štruktúr poznámkového bloku počas používania aplikácie

- **BOOT_END_AT_VIEW** – podkategória názvu aktivity (názov zobrazenia)

- **BOOT_SNAPSHOTS** – detail načítaní štruktúr poznámkového bloku pre kontá použité v aplikácii

- **COREAPP_STARTUP_ACCOUNT_SETUP_STARTUP_ACCOUNT_SETUP** – čas potrebný na kontrolu a spustenie skúsenosti jediného prihlásenia

- **CRASH_INTERACTION_DURING_BOOT> 0** – označuje, či aplikácia zlyhala počas poslednej relácie

- **DALVIK_HEAP_LIMIT_IN_MB** – zastarané

- **DELAY_LOAD_STICKY_NOTES** – označuje, či sa rýchle poznámky zobrazujú s oneskorením alebo nie

- **FISHBOWL_SHOWN_DURING_EVENT** – označuje inštancie, kde sa obsah nesynchronizuje

- **HAS_LOGCAT_LOGGING_IMPACT_ON_BOOT** – označuje, či majú protokoly vplyv na čas spúšťania

- **INIT_SNAPSHOT_DURATION** – čas potrebný na získanie štruktúry poznámkového bloku pre používateľské kontá

- **IS_COLD_BOOT** – označuje, či sa aplikácia spustí, keď nebola spustená na pozadí

- **IS_FIRST_LAUNCH** – označuje, či ide o prvé spustenie aplikácie v zariadení

- **IS_FOLDABLE_TYPE** – označuje, či zariadenie je skladacie

- **IS_PHONE** – označuje, či zariadenie je telefón alebo tablet

- **IS_RECENT_PAGES_AVAILABLE_ON_FRAGMENT_CREATION** – označuje, či je používateľské rozhranie pripravené a čaká, kedy bude obsah k dispozícii 

- **IS_REHYDRATE_LAUNCH** – označuje, či aplikáciu vypol systém

- **IS_UPGRADE** – označuje, či sa aplikácia spúšťa po inovácii

- **JOT_MAIN_APP_CREATE_TIME_MAIN_APP_CREATE_TIME** – čas potrebný na vytvorenie súčasti JOT (súčasť so zdieľaným kódom) 

- **JOT_MAIN_APP_INIT_TIME_MAIN_APP_INIT_TIME** – čas potrebný na inicializáciu súčasti JOT

- **LAUNCH_POINT** – označuje, či je aplikácia otvorená z miniaplikácie alebo ikony aplikácie alebo hypertextového prepojenia alebo zo zdieľania atď.

- **MSO_ACTIVATION_TIME_ACTIVATION_TIME** – čas potrebný na inicializáciu MSO

- **NATIVE_LIBRARIES_LOAD_TIME** – čas potrebný na načítania knižníc

- **NAVIGATION_CREATE_TO_NAVIGATION_RESUME_CREATE_TO_NAVIGATION_RESUME** – čas potrebný na dokončenie navigácie

- **NAVIGATION_RESUME_TO_BOOT_END_RESUME_TO_BOOT_END** – čas potrebný na meranie oneskorenia v načítaní stránky po štarte.

- **NAVIGATION_SET_CONTENT_VIEW_TIME_SET_CONTENT_VIEW_TIME** – čas potrebný na zobrazenie obsahu

- **NUMBER_Of_RUNNING_PROCESSES** – označuje počet spustených aktívnych procesov

- **NUMBER_OF_SNAPSHOTS** – počet načítaní štruktúry poznámkového bloku počas štartu

- **OFFICEASSETMANAGER_INITIALIZATION_TIME** – čas potrebný na rozbalenie a inicializáciu správcu položiek

- **PROCESS_BOOT_TIME_IN_MS** – čas potrebný na dokončenie vytvorenia procesu

- **ROOT_ACTIVITY_CREATE_ACTIVITY_CREATE** – čas potrebný na prechod z koreňovej vrstvy 

- **ROOT_ACTIVITY_DISK_CHECK_ACTIVITY_DISK_CHECK** – zastarané

- **ROOT_ACTIVITY_LAUNCH_NEXTACTIVITY_ACTIVITY_LAUNCH_NEXTACTIVITY** – zastarané

- **ROOT_ACTIVITY_PROCESS_INTENT_ACTIVITY_PROCESS_INTENT** – zastarané 

- **ROOT_ACTIVITY_SESSION_ACTIVITY_SESSION** – čas potrebný na prechod z koreňovej vrstvy 

- **ROOT_TO_NAVIGATION_TRANSITION_TO_NAVIGATION_TRANSITION** – čas potrebný na spracovanie navigácie z koreňa

- **SNAPSHOT_PUBLISH_TO_RENDERING_END_PUBLISH_TO_RENDERING_END** – čas potrebný na dokončenie vykresľovania obsahu

- **SPLASH_ACTIVITY_SESSION_ACTIVITY_SESSION** – čas potrebný na zobrazenie úvodnej obrazovky

- **SPLASH_TO_ROOT_TRANSITION_TO_ROOT_TRANSITION** – čas potrebný na prechod z koreňovej vrstvy 

- **TIME_BETWEEN_PROCESS_BOOT_AND_ACTIVITY_BEGIN_IN_MS** – čas medzi vytvorením procesu a aktivity 

- **TIME_TAKEN_IN_MS** – čas potrebný na dokončenie štartu
 
- **TOTAL_MEMORY_IN_MB** – celková pamäť zariadenia
 
- **USER_INTERACTED_DURING_EVENT** – označuje, či došlo k interakcii používateľa počas štartovania

#### <a name="officeonenoteandroidapponenoteappforeground-officeandroidearlytelemetryonenoteappforeground"></a>Office.OneNote.Android.App.OneNoteAppForeground, Office.Android.EarlyTelemetry.OneNoteAppForeground

*[Táto udalosť sa predtým nazývala OneNote.App.OneNoteAppForeground.]*

Signál, ktorý sa používa na označenie toho, že aplikácia OneNote sa nachádza v popredí.  Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. 

Zhromažďujú sa tieto polia: 

- Žiadne

#### <a name="officeonenoteandroidapplaunch-officeandroidearlytelemetryapplaunch"></a>Office.OneNote.Android.AppLaunch, Office.Android.EarlyTelemetry.AppLaunch

*[Táto udalosť sa predtým nazývala OneNote.AppLaunch.]*

Kritický signál sa používa na zaistenie, aby používatelia OneNotu mohli úspešne spustiť aplikáciu.  Telemetria sa používa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. 

Zhromažďujú sa tieto polia: 

- **ANDROID_SDK_VERSION** – označuje verziu Android SDK

- **FirstLaunchTime** – zaznamenáva čas, kedy bola aplikácia spustená prvýkrát

- **InstallLocation** – označuje, či je aplikácia predinštalovaná alebo stiahnutá z obchodu

- **is_boot_completed_ever** – označuje, či sa aplikácia v zariadení už niekedy úspešne spustila

- **IS_DARK_MODE_ENABLED** – Boolovská hodnota, ktorá označuje, či je aplikácia v tmavom režime alebo nie

- **NewOneNoteUser** – identifikujte, či je používateľ novým používateľom

#### <a name="officeoutlookdesktopexchangepuidandtenantcorrelation"></a>Office.Outlook.Desktop.ExchangePuidAndTenantCorrelation

Táto udalosť zhromažďuje identifikátor PUID používateľa a identifikátor nájomníka raz za reláciu. Korelácia identifikátora PUID a nájomníka je nevyhnutná na porozumenie a diagnostiku problémov s Outlookom na základe jednotlivých nájomníkov.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – časová pečiatka udalosti

  - **ConnId** – identifikátor spojenia: identifikátor spojenia analyzujúceho identifikátor PUID a identifikátor nájomníka OMS

  - **OMSTenantId** – jedinečný identifikátor nájomníka generovaný spoločnosťou Microsoft

  - **PUID** – identifikátor PUID Exchangeu na jedinečnú identifikáciu používateľov


#### <a name="officeoutlookmacmacolkactivationstate"></a>Office.Outlook.Mac.MacOLKActivationState

Zhromažďuje informácie o tom, ako je Outlook aktivovaný, napríklad s predplatným alebo multilicenciou. Údaje sú monitorované, aby sa nezobrazovali žiadne výkyvy v zlyhaniach. Údaje tiež analyzujeme preto, aby sme zistili oblasti na vylepšenie. 

Zhromažďujú sa tieto polia:

- **SetupUIActivationMethod** – spôsob aktivácie Outlooku, ako je napríklad predplatné alebo multilicencia.

#### <a name="officepowerpointdocoperationopen"></a>Office.PowerPoint.DocOperation.Open 

Táto udalosť sa zhromažďuje vždy, keď PowerPoint otvorí súbor. Zahŕňa informácie o úspechu, podrobnosti o zlyhaní, metriku výkonu a základné podrobnosti o súbore vrátane typu formátu súboru a metaúdajov dokumentu. Tieto informácie sú potrebné na zabezpečenie, že PowerPoint dokáže úspešne otvoriť súbory bez zníženia výkonu. Umožňuje nám diagnostikovať problémy, ktoré zistíme.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemetryResult** – označuje, či tento záznam denníka má všetku potrebnú telemetriu dokumentu (polia Data\_Doc\_\*)

  - **Data\_AddDocumentToMruList** – trvanie spustenia metódy AddDocumentToMruList

  - **Data\_AlreadyOpened** – označuje, či bol tento dokument už niekedy otvorený (v rámci kontextu tej istej relácie procesu)

  - **Data\_AntiVirusScanMethod** – preddefinovaná množina hodnôt typu skenovania antivírusu (IOAV, AMSI, žiadny atď.)

  - **Data\_AntiVirusScanStatus** – preddefinovaná množina hodnôt skenovania antivírusu, ktoré prebieha pre každý otvorený dokument (NoThreatsDetected, Failed, MalwareDetected atď.)

  - **Data\_AsyncOpenKind** – preddefinovaná množina hodnôt možností asynchrónnosti (Collab, ServerOnly, SyncBacked, NotAsync)

  - **Data\_CancelBackgroundDownloadHr** – označuje, či bolo sťahovanie dokumentu prerušené. Ak áno, aký bol výsledok prerušenia.

  - **Data\_CheckForAssistedReadingReasons** – trvanie spustenia metódy CheckForAssistedReadingReasons v milisekundách

  - **Data\_CheckForDisabledDocument** – trvanie spustenia metódy CheckForDisabledDocument v milisekundách

  - **Data\_CheckForExistingDocument** – trvanie spustenia metódy CheckForExistingDocument v milisekundách

  - **Data\_CheckIncOpenResult** – trvanie spustenia metódy CheckIncOpenResult v milisekundách

  - **Data\_CheckLambdaResult** – trvanie spustenia metódy CheckLambdaResult v milisekundách

  - **Data\_CheckPackageForRequiredParts** – trvanie spustenia metódy CheckPackageForRequiredParts v milisekundách

  - **Data\_CheckPackageForSpecialCases** – trvanie spustenia metódy CheckPackageForSpecialCases v milisekundách

  - **Data\_CheckRequiredPartsLoaded** – trvanie spustenia metódy CheckRequiredPartsLoaded v milisekundách

  - **Data\_CheckWebSharingViolationForIncOpen** – trvanie spustenia metódy CheckWebSharingViolationForIncOpen v milisekundách
   
  - **Data_CloseAndReopenWithoutDiscard** – označuje, či bol dokument zavretý a opäť otvorený počas otvoreného procesu bez vyhodenia.

  - **Data\_ContentTransaction** – preddefinovaná množina hodnôt určujúcich, kedy je možné vytvoriť transakciu (AllowedOnLoadDocument, AllowedOnOpenComplete atď.)

  - **Data_CorrelationId** – identifikátor GUID odoslaný do PowerPointu procesom ProtocolHandler na koreláciu telemetrie. ProtocolHandler je samostatný proces, ktorý spracováva prepojenia balíka Office pre operačný systém.

  - **Data\_CppUncaughtExceptionCount:long** – nezachytené natívne výnimky počas spustenej aktivity

  - **Data\_CreateDocumentTimeMS** – trvanie spustenia metódy CreateDocumentTimeMS v milisekundách

  - **Data\_CreateDocumentToken** – trvanie spustenia metódy CreateDocumentToken v milisekundách

  - **Data\_CreateDocumentToW** – trvanie spustenia metódy CreateDocumentToW v milisekundách

  - **Data\_CreateDocWindow** – trvanie spustenia metódy CreateDocWindow v milisekundách

  - **Data\_CreateLocalTempFile** – trvanie spustenia metódy CreateLocalTempFile v milisekundách

  - **Data\_DetachedDuration:long** – časový úsek, počas ktorého bola aktivita odpojená/nespustená

  - **Data\_** – trvanie spustenia metódy DetermineFileType v milisekundách

  - **Data\_Doc\_AccessMode:long** – ako bol otvorený tento dokument (iba na čítanie alebo na čítanie a zapisovanie)

  - **Data\_Doc\_AssistedReadingReasons:long** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou

  - **Data_Doc_AsyncOpenKind:long** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data\_Doc\_ChunkingType:long** – ako je dokument uložený v SharePointe

  - **Data\_Doc\_EdpState:long** – stav ochrany podnikových údajov v dokumente

  - **Data\_Doc\_Ext:string** – prípona dokumentu

  - **Data\_Doc\_Extension:string** – prípona dokumentu

  - **Data\_Doc\_FileFormat:long** – preddefinovaná množina hodnôt formátu súboru (podrobnejšie ako prípona)

  - **Data\_Doc\_Fqdn:string** – miesto uloženia dokumentu (SharePoint.com, live.net), k dispozícii len pre domény Office 365

  - **Data\_Doc\_FqdnHash:string** – hodnota hash miesta uloženia dokumentu

  - **Data\_Doc\_IdentityTelemetryId:string** – jedinečný identifikátor GUID používateľa

  - **Data\_Doc\_IdentityUniqueId:string** – jedinečný identifikátor identity, ktorý sa použil pre akciu zdieľaných dokumentov

  - **Data\_Doc\_IOFlags:long** – bitová maska pre rôzne príznaky súvisiace s OI pre daný dokument

  - **Data\_Doc\_IrmRights:long** – preddefinovaná množina hodnôt toho, aký typ správy prístupových práv k informáciám je použitý v tomto dokumente (preposielanie, odpovedanie, SecureReader, úpravy atď.)

  - **Data\_Doc\_IsCloudCollabEnabled:bool** – má hodnotu true, ak už bola prijatá hlavička protokolu HTTP „IsCloudCollabEnabled“ z požiadavky OPTIONS.

  - **Data\_Doc\_IsIncrementalOpen:bool** – určuje, či bol dokument otvorený prírastkovo (novou funkciou, ktorá otvorí dokument bez potreby stiahnutia celého dokumentu)

  - **Data\_Doc\_IsOcsSupported:bool** – či dokument podporuje spoluautorstvo pomocou novej služby OCS

  - **Data\_Doc\_IsOpeningOfflineCopy:bool** – otvára sa dokument z lokálnej vyrovnávacej pamäti?

  - **Data\_Doc\_IsSyncBacked:bool** – otvára sa dokument z priečinka, ktorý používa aplikáciu synchronizácie zálohovania OneDrivu?

  - **Data\_Doc\_Location:long** – preddefinovaná množina hodnôt miesta uloženia dokumentu (lokálne, SharePoint, WOPI, sieť atď.)

  - **Data\_Doc\_LocationDetails:long** – preddefinovaná množina hodnôt podrobnejšieho umiestnenia (priečinok pre dočasné súbory, priečinok na ukladanie stiahnutých súborov, dokumenty vo OneDrive, obrázky vo OneDrive atď.)

  - **Data\_Doc\_NumberCoAuthors:long** – počet spoluautorov v čase otvorenia dokumentu

  - **Data\_Doc\_PasswordFlags:long** – preddefinovaná množina hodnôt šifrovania dokumentu pomocou hesla (bez hesla, heslo na čítanie, heslo na úpravu)

  - **Data\_Doc\_ReadOnlyReasons:long** – preddefinovaná množina hodnôt dôvodu označenia dokumentu Len na čítanie (uzamknutý na serveri, konečná verzia dokumentu, úpravy chránené heslom atď.)

  - **Data\_Doc\_ResourceIdHash:string** – hodnota hash identifikátora zdroja pre dokumenty uložené v cloude

  - **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

  - **Data\_Doc\_ServerDocId:string** – nemenný identifikátor pre dokumenty uložené v cloude

  - **Data\_Doc\_ServerProtocol:long** – preddefinovaná množina hodnôt toho, ktorý protokol sa používa na komunikáciu so serverom (HTTP, Cobalt, WOPI atď.)
 
  - **Data\_Doc\_ServerType:long** – preddefinovaná množina hodnôt typu servera (SharePoint, DropBox, WOPI)

  - **Data\_Doc\_ServerVersion:long** – určuje, či je server založený na Office14, Office15 alebo Office16

  - **Data\_Doc\_SessionId:long** – vygenerovaný identifikátor GUID, ktorý identifikuje inštanciu dokumentu v rámci tej istej relácie procesu

  - **Data\_Doc\_SharePointServiceContext:string** – nepriehľadný reťazec, zvyčajne GridManagerID.FarmID. Pomáha pri korelácii denníkov na strane klienta a na strane servera

  - **Data\_Doc\_SizeInBytes:long** – veľkosť dokumentu v bajtoch

  - **Data\_Doc\_SpecialChars:long** – bitová maska označujúca špeciálne znaky v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StorageProviderId:string** – reťazec, ktorý identifikuje poskytovateľa ukladacieho priestoru dokumentu, napríklad „DropBox“

  - **Data\_Doc\_StreamAvailability:long** – preddefinovaná množina hodnôt stavu streamu dokumentu (dostupný, natrvalo vypnutý, nedostupný)

  - **Data\_Doc\_UrlHash:string** – hodnota hash celej URL adresy dokumentov uložených v cloude

  - **Data\_Doc\_UsedWrsDataOnOpen:bool** – má hodnotu true, ak bol súbor otvorený prírastkovo pomocou údajov WRS vopred uložených vo vyrovnávacej pamäti u hostiteľa

  - **Data\_Doc\_WopiServiceId:string** – identifikátor služby WOPI, napríklad „Dropbox“

  - **Data\_DownloadExcludedData** – trvanie spustenia metódy DownloadExcludedData v milisekundách

  - **Data\_DownloadExcludedDataTelemetry** – preddefinovaná množina hodnôt stavu synchrónneho čakania na stiahnutie (SynchronousLogicHit, UserCancelled RunModalTaskUnexpectedHResult atď.)

  - **Data\_** – trvanie spustenia metódy DownloadFileInBGThread v milisekundách

  - **Data\_DownloadFragmentSize** – veľkosť fragmentu (stiahnuteľného kúska súboru), zvyčajne 3,5 MB

  - **Data\_ExcludedEmbeddedItems** – počet zip častí, ktoré sú vylúčené pre prvé vykreslenie

  - **Data\_ExcludedEmbeddedItemsSize** – celková veľkosť zip častí, ktoré sú vylúčené pre prvé vykreslenie

  - **Data\_ExcludedRequiredItems** – počet zip častí, ktoré sú vylúčené, ale požadované pre prvé vykreslenie

  - **Data\_ExcludedRequiredItemsSize** – celková veľkosť zip častí, ktoré sú vylúčené, ale požadované pre prvé vykreslenie

  - **Data\_ExecutionCount** – počet spustení protokolu IncOpen

  - **Data\_FailureComponent:long** – preddefinovaná množina hodnôt toho, ktorá súčasť spôsobila zlyhanie protokolu (Conflict, CSI, Internal atď.)

  - **Data\_FailureReason:long** – preddefinovaná množina hodnôt dôvodu zlyhania (FileIsCorrupt, BlockedByAntivirus atď.)

  - **Data\_FCreateNew** – označuje, či ide o nový prázdny dokument

  - **Data\_FCreateNewFromTemplate** – označuje, či ide o nový dokument zo šablóny

  - **Data_FErrorAfterDocWinCreation:boolean** – zobrazuje, či sa po vytvorení okna dokumentu vyskytla nejaká chyba alebo výnimka.

  - **Data\_FileUrlLocation** – preddefinovaná množina hodnôt miesta uloženia dokumentu (NetworkShare, LocalDrive, ServerOther atď.)

  - **Data\_FirstSlideCompressedSize** – komprimovaná veľkosť zip časti prvej snímky (zvyčajne Slide1.xml)

  - **Data_FIsAutoBackupFile** – Je tento súbor automatický záložný súbor?

  - **Data\_FIsDownloadFileInBgThreadEnabled** – označuje, či je povolené sťahovanie vo vlákne na pozadí

  - **Data\_fLifeguarded:bool** – či mal dokument niekedy chránenú životnosť (funkciou na riešenie chýb dokumentov bez zobrazenia výzvy používateľovi)

  - **Data\_ForceReopenOnIncOpenMergeFailure** – príznak vyjadrujúci, či sme boli nútení znova otvoriť z dôvodu zlyhania zlúčenia v prírastkovom otváraní

  - **Data\_ForegroundThreadPass0TimeMS** (len Mac) – celkový čas strávený vo vlákne v popredí pri prvom prechode

  - **Data\_ForegroundThreadPass1TimeMS** (len Mac) – celkový čas strávený vo vlákne v popredí pri druhom prechode

  - **Data\_FWebCreatorDoc** – či je dokument vytvorený zo šablóny alebo rýchleho štartu

  - **Data\_HasDocToken** – či má tento dokument token dokumentu CSI (interný kód)

  - **Data\_HasDocument** – či má tento dokument dokument CSI (interný kód)

  - **Data\_InclusiveMeasurements -** – či trvania merania metód obsahujú trvanie volania podriadenej metódy

  - **Data\_IncompleteDocReasons** – preddefinovaná množina hodnôt toho, prečo bolo otvorenie neúplné (Unknown, DiscardFailure atď.)

  - **Data\_IncOpenDisabledReasons** – preddefinovaná množina hodnôt dôvodov zakázania prírastkového otvárania

  - **Data\_IncOpenFailureHr** – výsledok, prečo prírastkové otváranie zlyhalo

  - **Data\_IncOpenFailureTag** – značka (ukazovateľ na miesto v kóde) miesta zlyhania prírastkového otvárania

  - **Data\_IncOpenFallbackReason** – prečo sa prírastkové otváranie nespustilo

  - **Data\_IncOpenRequiredTypes** – preddefinovaná množina hodnôt typov obsahu potrebných na prvé vykreslenie (RequiredXmlZipItem, RequiredNotesMaster atď.)

  - **Data\_IncOpenStatus** – preddefinovaná množina hodnôt stavu prírastkového otvárania (Attempted, FoundExcludedItems, DocIncOpenInfoCreated atď.)

  - **Data\_InitFileContents** – trvanie spustenia metódy InitFileContents v milisekundách

  - **Data\_InitialExcludedItems** – počet zip častí, ktoré sú spočiatku vylúčené

  - **Data\_InitialExcludedItemsSize** – celková veľkosť zip častí, ktoré sú spočiatku vylúčené

  - **Data\_InitializationTimeMS** – (len Mac) čas na spustenie

  - **Data\_InitialRoundtripCount** – počet odpovedí servera potrebných na vytvorenie počiatočného zip archívu

  - **Data\_InitLoadProcess** – trvanie spustenia metódy InitLoadProcess v milisekundách

  - **Data\_InitPackage** – trvanie spustenia metódy InitPackage v milisekundách

  - **Data\_InitSecureReaderReasons** – trvanie spustenia metódy InitSecureReaderReasons v milisekundách

  - **Data\_IsIncOpenInProgressWhileOpen** – či je v prípade viacnásobného otvárania toho istého dokumentu protokol Inc open spustený spoločne s protokolom open

  - **Data\_IsMultiOpen** – či podporujeme viacnásobné otvorenie

  - **Data\_IsOCS** – či bol dokument vo svojom poslednom známom stave v režime OCS

  - **Data\_IsODPFile** – či je dokument vo formáte Open Document Format používanom softvérom OpenOffice.org

  - **Data\_IsPPTMetroFile** – či je dokument vo formáte metro (pptx)

  - **Data\_LoadDocument** – trvanie spustenia metódy LoadDocument v milisekundách

  - **Data\_MeasurementBreakdown** – rozdelenie šifrovaných meraní (skrátená podrobná metóda perf)

  - **Data\_Measurements** – šifrované merania

  - **Data\_MethodId** – naposledy spustená metóda

  - **Data\_NotRequiredExcludedItems** – celkový počet položiek balíka PowerPointu, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data\_NotRequiredExcludedItemsSize** – celková veľkosť položiek balíka PowerPointu, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data\_NotRequiredExcludedParts** – celkový počet položiek zip častí, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data\_NotRequiredExcludedPartsSize** – celková veľkosť zip častí, ktoré nie sú požadované pre prvé vykreslenie a vylúčené

  - **Data_OngoingBlockingOpenCount** – počet aktuálne spustených blokovacích otvorených protokolov.
  
  - **Data_OngoingOpenCount** – počet aktuálne spustených otvorených protokolov.

  - **Data\_OpenCompleteFailureHR** – výsledok dôvodu zlyhania protokolu OpenComplete

  - **Data\_OpenCompleteFailureTag** – značka (ukazovateľ na miesto v kóde) miesta zlyhania protokolu OpenComplete

  - **Data\_OpenLifeguardOption**– preddefinovaná množina hodnôt volieb pre operáciu ochrany životnosti (None, TryAgain, OpenInWebApp atď.)

  - **Data\_OpenReason** – preddefinovaná množina hodnôt spôsobu otvorenia tohto dokumentu (FilePicker, OpenFromMru, FileDrop atď.)

  - **Data\_OSRPolicy** – politika SecureReader

  - **Data\_OSRReason** – dôvody otvorenia tohto dokumentu v Secure Reader

  - **Data\_OtherContentTypesWithRequiredParts** – neštandardné typy obsahu, ktoré boli vylúčené, ale požadované pre prvé vykreslenie

  - **Data\_PrepCacheAsync** – príznak pre OcsiOpenPerfPrepCacheAsync

  - **Data\_PreviousDiscardFailed** – označuje, že predchádzajúci pokus o otvorenie/zavretie dokumentu neuvoľnil správne všetku pamäť

  - **Data\_PreviousFailureHr** – v prípade opätovného otvárania toho istého dokumentu, aký bol výsledok posledného zlyhania

  - **Data\_PreviousFailureTag** – v prípade opätovného otvárania toho istého dokumentu, aká bola značka posledného zlyhania (ukazovateľ na miesto v kóde)

  - **Data\_RemoteDocToken** – je povolené vzdialené otváranie (funkcia v štádiu prototypu, ktorá umožňuje otvoriť súbor zo služby namiesto z hostiteľa)?

  - **Data\_Repair** – či sa nachádzame v režime opravy dokumentu (pre poškodené dokumenty, ktoré sú opraviteľné)

  - **Data\_RequestPauseStats** – koľkokrát kód požadoval pozastavenie zaznamenávania výkonu

  - **Data\_RequiredPartsComressedSize** – celková veľkosť požadovaných častí PowerPointu potrebných na prvé vykreslenie

  - **Data\_RequiredPartsDownload** – celková veľkosť požadovaných častí PowerPointu, ktoré sú stiahnuté

  - **Data\_RequiredPartsRoundtripCount** – celkový počet cyklov (volaní hostiteľa) potrebných na získanie všetkých požadovaných častí PowerPointu na prvé vykreslenie

  - **Data\_RequiredZipItemsDownload** – celková veľkosť požadovaných zip položiek potrebných na prvé vykreslenie

  - **Data\_RequiredZipItemsRoundtripCount** – celkový počet cyklov (volaní hostiteľa) potrebných na získanie všetkých požadovaných zip položiek na prvé vykreslenie

  - **Data\_RoundtripsAfterMissingRequiredParts** – celkový počet cyklov (volaní hostiteľa) potrebných po nájdení chýbajúcich požadovaných častí PowerPointu

  - **Data\_RoundtripsAfterMissingRequiredZipItems** – celkový počet cyklov (volaní hostiteľa) potrebných po nájdení chýbajúcich požadovaných zip položiek

  - **Data\_** – celkový počet cyklov (volaní hostiteľa) potrebných po vytvorení balíka

  - **Data\_** – celkový počet cyklov (volaní hostiteľa) potrebných po stiahnutí všetkých požadovaných častí

  - **Data\_SetDocCoAuthAutoSaveable** – trvanie spustenia metódy SetDocCoAuthAutoSaveable v milisekundách

  - **Data\_SniffedFileType** – vzdelaný odhad navrhovaného typu súboru poškodeného dokumentu

  - **Data\_StartTime** – počítadlo výkonu po začatí otvárania

  - **Data\_StopwatchDuration:long** – celkový čas aktivity

  - **Data\_SyncSlides** – trvanie spustenia metódy SyncSlides v milisekundách

  - **Data\_TimerStartReason** – preddefinovaná množina hodnôt spôsobu spustenia časovača (CatchMissedSyncStateNotification, WaitingForFirstDownload atď.)

  - **Data\_TimeSplitMeasurements** – rozdelenie šifrovaných meraní (skrátená podrobná metóda perf)

  - **Data\_TimeToInitialPackage** – čas potrebný na vytvorenie počiatočného balíka

  - **Data\_TimeToRequiredPackage** – čas potrebný na vytvorenie požadovaného balíka

  - **Data\_TimeToRequiredParts** – čas potrebný na vytvorenie balíka so všetkými požadovanými časťami

  - **Data\_TotalRequiredParts** – celkový počet častí PowerPointu potrebných na prvé vykreslenie

  - **Data\_UnknownRequiredParts** – celkový počet neštandardných častí potrebných na prvé vykreslenie

  - **Data\_UnpackLinkWatsonId** – identifikátor Watson chyby pri otváraní dokumentu prostredníctvom URL adresy zdieľania cez OneDrive

  - **Data\_UnpackResultHint** – preddefinovaná množina hodnôt rozbalenia výsledkov URL adresy zdieľania (NavigateToWebWithoutError, UrlUnsupported, AttemptOpen atď.)

  - **Data\_UnpackUrl** – trvanie spustenia metódy UnpackUrl v milisekundách

  - **Data\_UpdateAppstateTimeMS** – trvanie spustenia metódy UpdateAppstate v milisekundách

  - **Data\_UpdateCoauthoringState** – trvanie spustenia metódy UpdateCoauthoringState v milisekundách

  - **Data\_UpdateReadOnlyState** – trvanie spustenia metódy UpdateReadOnlyState v milisekundách

  - **Data\_WACCorrelationId** – v prípade otvárania súboru v prehliadači získanie korelácie denníkov WebApp

  - **Data\_WasCachedOnInitialize** – či bol tento dokument uložený do vyrovnávacej pamäte počas inicializácie

  - **Data\_WBDirtyBeforeDiscard** – či sa pracovná vetva stala zmenenou (dirty) pred otvorením dokumentu

  - **Data\_ZRTOpenDisabledReasons** – prečo sa nepodarilo dokument z vyrovnávacej pamäte (Zero Round Trip)

#### <a name="officepowerpointpptdesktopbootime"></a>Office.PowerPoint.PPT.Desktop.Bootime

Táto udalosť zhromažďuje informácie o spustení PowerPointu. Zahŕňa spustenie PowerPointu v chránenom zobrazení, v režime asistovaného čítania, z makra, tlače, nového a prázdneho dokumentu, obnovenia dokumentu, z automatizácie a či ide o technológiu Klikni a spusti. Tiež zhromažďuje, ako dlho trvá spustenie PowerPointu. Tento údaj je veľmi dôležitý na to, aby sa zaručilo, že PowerPoint funguje správne pri spúšťaní z rôznych režimov. Spoločnosť Microsoft používa tieto údaje na zachytenie dlhého času spustenia pri otváraní PowerPointu z rôznych režimov.

Zhromažďujú sa tieto polia:

  - **AssistedReading** – v režime asistovaného čítania

  - **Automation** – z automatizácie

  - **Benchmark** – spustenie benchmarku výkonu

  - **Blank** – prázdny dokument

  - **BootTime** – čas spustenia relácie

  - **Embedding** – vloženie dokumentu

  - **IsC2R** – či ide o technológiu Klikni a spusti

  - **IsNew** – nový dokument

  - **IsOpen** – je otvorený

  - **Macro1** – spustenie makra

  - **Macro2** – spustenie makra

  - **NonStandardSpaceInCmdLine** – v príkazovom riadku je neštandardná medzera

  - **Print** – tlač dokumentu

  - **PrintDialog** – tlač dokumentu s dialógovým oknom

  - **PrintPrinter** – tlač dokumentu s tlačiarňou

  - **ProtectedView** – v chránenom zobrazení

  - **Regserver** – registrácia PowerPointu ako servera COM

  - **Restore** – obnovenie dokumentu

  - **Show** – zobrazenie dokumentu

  - **Time** – čas relácie

  - **UnprotectedView** – v nechránenom zobrazení

#### <a name="officepowerpointppthasuserediteddocument"></a>Office.PowerPoint.PPT.HasUserEditedDocument

Zhromažďuje sa, keď používateľ začne upravovať dokument. Spoločnosť Microsoft používa tieto údaje na vypočítanie aktívnych používateľov, ktorí upravovali powerpointový dokument.

Zhromažďujú sa tieto polia:

  - **CorrelationId** – identifikátor korelácie dokumentu

#### <a name="officeprojectbootandopenproject"></a>Office.Project.BootAndOpenProject

Project je spustený otvorením súboru. Táto udalosť označuje, že používateľ otvoril Office Project priradeným súborom. Obsahuje dôležité údaje o úspechu zaručenia, že Project sa môže spustiť a načítať súbor.

Zhromažďujú sa tieto polia:

  - **Data\_AlertTime** – čas, počas ktorého bolo aktívne dialógové okno spustenia.

  - **Data\_BootTime** – čas potrebný na spustenie Projectu

  - **Data\_CacheFileSize** – ak bol súbor uložený vo vyrovnávacej pamäti, veľkosť súboru

  - **Data\_EntDocType** – typ súboru, ktorý bol otvorený

  - **Data\_IsInCache** – označuje, či otvorený súbor bol uložený vo vyrovnávacej pamäti

  - **Data\_LoadSRAs** – či používateľ chce načítať SRA alebo nie

  - **Data\_Outcome** – celkový čas spustenia a otvorenia súboru.

  - **Data\_OpenFromDocLib** – či otvorný súbor Projectu bol z knižnice dokumentov

  - **Data\_ProjectServerVersion** – aktuálna verzia a zostava Projectu

#### <a name="officeprojectbootproject"></a>Office.Project.BootProject

Project je spustený bez otvorenia súboru. Táto udalosť označuje, že používateľ otvoril Office Project bez priradeného súboru. Obsahuje dôležité údaje o úspechu zaručenia, že Project sa môže spustiť.

Zhromažďujú sa tieto polia:

  - **Data\_BootTime** – čas potrebný na spustenie Projectu

  - **Data\_FileLoaded** – má hodnotu false, ak ide o otvorenie z vonkajšieho alebo nového prázdneho projektu

  - **Data\_IsEntOfflineWithProfile** – označuje, či používatelia sú v profesionálnej jednotke SKU a nie sú pripojení k serveru

  - **Data\_IsEntOnline** – označuje, či relácia Projectu je pripojená k projectovému serveru s podnikovými funkciami

  - **Data\_IsLocalProfile** – označuje, či relácia Projectu je pripojená k projectovému serveru s podnikovými funkciami

  - **Data\_ProjectServerVersion** – aktuálna verzia a zostava Projectu


#### <a name="officeprojectopenproject"></a>Office.Project.OpenProject

Project otvorí súbor. Táto udalosť označuje, že používateľ priamo otvára súbor Projectu. Obsahuje dôležité údaje o úspechu otvárania súborov v Projecte.

Zhromažďujú sa tieto polia:

  - **Data\_AgileMode** – definuje, či otvorený projekt je vodopádový alebo agilný

  - **Data\_AlertTime** – čas, počas ktorého bolo aktívne dialógové okno spustenia

  - **Data\_CacheFileSize** – ak bol súbor uložený vo vyrovnávacej pamäti, veľkosť súboru

  - **Data\_EntDocType** – typ súboru, ktorý bol otvorený

  - **Data\_IsInCache** – označuje, či otvorený súbor bol uložený vo vyrovnávacej pamäti

  - **Data\_LoadSRAs** – či používateľ chce načítať SRA alebo nie

  - **Data\_OpenFromDocLib** – či otvorný súbor Projectu bol z knižnice dokumentov

  - **Data\_Outcome** – celkový čas spustenia a otvorenia súboru

  - **Data\_Outcome** – celkový čas spustenia a otvorenia súboru.

  - **Data\_ProjectServerVersion** – aktuálna verzia a zostava Projectu

#### <a name="officesessionidproviderofficeprocesssessionstart"></a>Office.SessionIdProvider.OfficeProcessSessionStart

Vzťahuje sa na všetky aplikácie balíka Office pre Windows: win32 a UWP

Zhromažďujú sa tieto polia:

- **OfficeProcessSessionStart** – odosiela základné informácie na začiatku novej relácie balíka Office. Používa sa na spočítanie počtu jedinečných relácií, ktoré sa vyskytujú v danom zariadení. Používa sa ako signálna udalosť na uistenie sa, či je aplikácia v zariadení spustená alebo nie. Okrem toho slúži ako dôležitý signál pre celkovú spoľahlivosť aplikácie

- **AppSessionGuid** – identifikátor konkrétnej relácie aplikácie, ktorá sa začína v čase vytvorenia procesu a pretrváva až do konca procesu. Je formátovaný ako štandardný 128-bitový identifikátor GUID, ale skladá sa zo štyroch častí. Tieto štyri časti sú v poradí 1. ID procesu 32-bitovej verzie, 2. ID relácie 16-bitovej verzie, 3. ID spustenia 16-bitovej verzie, 4. čas vytvorenia procesu 64-bitovej verzie v UTC 100 ns.

- **processSessionId** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

- **UTCReplace_AppSessionGuid** – konštantná boolovská hodnota. Vždy hodnota True.

#### <a name="officesystemsessionhandoff"></a>Office.System.SessionHandoff

Označuje, že aktuálna relácia balíka Office je relácia odovzdania. To znamená, že manipulácia s požiadavkou používateľa na otvorenie dokumentu sa odovzdáva do už spustenej inštancie tej istej aplikácie.

Zhromažďujú sa tieto polia:

- **ParentSessionId** – ID relácie, ktorá prevezme spracovanie žiadosti používateľov.

#### <a name="officetelemetryengineisprelaunch"></a>Office.TelemetryEngine.IsPreLaunch

Vzťahuje sa na všetky aplikácie UWP balíka Office.  Táto udalosť sa spustí pri prvom spustení aplikácie balíka Office po inovácii/inštalácii z obchodu. Je súčasťou základných diagnostických údajov, ktoré sa používajú na sledovanie, či ide o reláciu spustenia alebo nie.

Zhromažďujú sa tieto polia:

- **appVersionBuild** – číslo verzie zostavy aplikácie.

- **appVersionMajor** – číslo hlavnej verzie aplikácie.

- **appVersionMinor** – číslo vedľajšej verzie aplikácie.

- **appVersionRev** – číslo verzie revízie aplikácie.

- **sessionID** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

#### <a name="officetelemetryenginesessionhandoff"></a>Office.TelemetryEngine.SessionHandOff

Vzťahuje sa na všetky aplikácie Win32 balíka Office.  Táto udalosť nám pomáha zistiť, či sa vytvorila nová relácia na spracovanie udalosti otvorenia súboru iniciovanej používateľom. Ide o dôležité diagnostické informácie, ktoré sa používajú na odvodenie signálu spoľahlivosti a uistenie, že aplikácia funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

- **appVersionBuild** – číslo verzie zostavy aplikácie.

- **appVersionMajor** – číslo hlavnej verzie aplikácie.

- **appVersionMinor** – číslo vedľajšej verzie aplikácie.

- **appVersionRev** – číslo verzie revízie aplikácie.

- **childsessionID** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

- **parentsessionId** – náhodne vytvorený identifikátor GUID na identifikáciu relácie aplikácie

#### <a name="officevisiovisioiosappboottime"></a>Office.Visio.VisioIosAppBootTime

Toto sa spúšťa pri každom spustení aplikácie Visio pre iOS. Je dôležité pochopiť výkon spustenia aplikácie Visio pre iOS. Používa sa na riešenie problémov so slabým výkonom. 

Zhromažďujú sa tieto polia:

- **Data_AppBootTime** – Čas potrebný na spustenie aplikácie v milisekundách.

#### <a name="officevisiovisioiosappresumetime"></a>Office.Visio.VisioIosAppResumeTime 

Táto udalosť sa spúšťa pri každom obnovení zamerania aplikácie Visio pre iOS. Dôležité je merať výkon obnovenia aplikácie a vyriešiť problémy s výkonom aplikácie Visio pre iOS.

Zhromažďujú sa tieto polia:

- **Data_AppResumeTime** – Čas potrebný na obnovenie aplikácie v milisekundách.

#### <a name="officewordfileopenopencmdfilemrupriv"></a>Office.Word.FileOpen.OpenCmdFileMruPriv

Táto udalosť označuje, že Office Word otvára dokument zo zoznamu naposledy použitých súborov (MRU). Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru zo zoznamu naposledy použitých súborov funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť.

- **Data_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu.

- **Data_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor.

- **Data_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme. 

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_Doc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov. 

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese dokumentu. 

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania.

- **Data_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu.

- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o otvorenie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na meranie výkonu.

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje.

- **Data_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie. 

- **Data_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

- **Data_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.

- **PathData_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.


#### <a name="officewordfileopenopenffileopenxstzcore"></a>Office.Word.FileOpen.OpenFFileOpenXstzCore

Táto udalosť označuje, že Office Word otvára dokument, na ktorý používateľ dvakrát klikol. Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru dvojitým kliknutím na súbor funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.
    
- **Data_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť.
    
- **Data_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu.

- **Data_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor.
    
- **Data_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_Doc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.

- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.
    
- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).
    
- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).
    
- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu. 

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_Doc_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu.

- **Data_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania.
    
- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o otvorenie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na meranie výkonu.
    
- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje.

- **Data_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie.

- **Data_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

- **Data_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.


#### <a name="officewordfileopenopenifrinitargs"></a>Office.Word.FileOpen.OpenIfrInitArgs

Táto udalosť označuje, že Office Word otvára dokument prostredníctvom aktivácie COM alebo príkazového riadka. Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru z príkazového riadka funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

  - **Data\_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

  - **Data\_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť

  - **Data\_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu

  - **Data\_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor

  - **Data\_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme.

  - **Data\_Doc\_AccessMode** – označuje, či je dokument iba na čítanie alebo editovateľný

  - **Data\_Doc\_AssistedReadingReasons** – preddefinovaná množina hodnôt toho, prečo bol dokument otvorený v režime čítania s asistenciou.

  - **Data_Doc_AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

  - **Data\_Doc\_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu

  - **Data\_Doc\_EdpState** – nastavenie ochrany elektronických údajov dokumentu

  - **Data\_Doc\_Ext** – prípona dokumentu (docx, xlsb, pptx atď.)

  - **Data\_Doc\_FileFormat** – verzia protokolu formátu súboru

  - **Data\_Doc\_Fqdn** – názov domény OneDrivu alebo SharePointu Online

  - **Data\_Doc\_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény

  - **Data\_Doc\_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností otvorenej požiadavky

  - **Data\_Doc\_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia

  - **Data\_Doc\_InitializationScenario** – zaznamenáva, ako bol dokument otvorený

  - **Data\_Doc\_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa

  - **Data\_Doc\_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo

  - **Data\_Doc\_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce

  - **Data\_Doc\_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline

  - **Data\_Doc\_IsSyncBacked** – príznak, ktorý označuje, že v počítači existuje automaticky synchronizovaná kópia dokumentu

  - **Data\_Doc\_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.)

  - **Data\_Doc\_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument

  - **Data\_Doc\_NumberCoAuthors** – počet používateľov v relácii spoločných úprav

  - **Data\_Doc\_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie

  - **Data\_Doc\_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie

  - **Data\_Doc\_ResourceIdHash** – anonymizovaný identifikátor dokumentu, ktorý sa používa na diagnostiku problémov

  - **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

  - **Data\_Doc\_ServerDocId** – nemenný anonymizovaný identifikátor dokumentu, ktorý sa používa na diagnostiku problémov

  - **Data\_Doc\_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou

  - **Data\_Doc\_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.)

  - **Data\_Doc\_ServerVersion** – verzia servera, ktorý ponúka službu

  - **Data\_Doc\_SessionId** – verzia servera, ktorý ponúka službu

  - **Data\_Doc\_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online

  - **Data\_Doc\_SizeInBytes** – indikátor veľkosti dokumentu

  - **Data\_Doc\_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu

  - **Data\_Doc\_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý

  - **Data\_Doc\_SyncBackedType** – indikátor typu dokumentu (lokálny alebo v službe)

  - **Data\_Doc\_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu

  - **Data\_Doc\_WopiServiceId** – obsahuje jedinečný identifikátor poskytovateľa služieb WOPI

  - **Data\_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania

  - **Data\_EditorsCount** – počet editorov v dokumente

  - **Data\_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu

  - **Data\_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania

  - **Data\_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o otvorenie zlyhá dvakrát (používa sa na diagnostiku kvality údajov)

  - **Data\_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny

  - **Data\_MainPdod** – identifikátor dokumentu v procese programu Office Word

  - **Data\_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na diagnostikovanie výkonu otvárania.

  - **Data\_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu

  - **Data\_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania

  - **Data\_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje

  - **Data\_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením

  - **Data\_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu

  - **Data\_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania

  - **Data\_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie.

  - **Data\_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

  - **Data\_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.


#### <a name="officewordfileopenopenloadfile"></a>Office.Word.FileOpen.OpenLoadFile

Táto udalosť označuje, že Office Word otvára dokument prostredníctvom dialógového okna Otvoriť. Obsahuje aj kritické údaje o výkone otvárania súboru a je udalosťou spustenia aplikácie z pohľadu používateľa. Udalosť monitoruje, či otvorenie súboru z dialógového okna Otvoriť funguje podľa očakávaní. Používa sa aj na vypočítanie počtu aktívnych používateľov a zariadení za mesiac a metriky spoľahlivosti cloudu.

Zhromažďujú sa tieto polia:

- **Data_AddDocTelemRes** – hlási, či sme dokázali správne vyplniť ďalšie hodnoty týkajúce sa telemetrie dokumentu v udalosti. Používa sa na diagnostiku kvality údajov.

- **Data_BytesAsynchronous** – počet bajtov (komprimovaných), bez ktorých podľa nás dokážeme otvoriť dokument, ak by sme ich dostali predtým, než používateľ chce začať upravovať, prípadne uložiť.

- **Data_BytesAsynchronousWithWork** – počet bajtov (komprimovaných), bez ktorých by sme možno dokázali otvoriť súbor, alebo vyžadovalo by si to značné investície do kódu.
    
- **Data_BytesSynchronous** – počet bajtov (komprimovaných), ktoré musíme mať predtým, než môžeme začať otvárať súbor.

- **Data_BytesUnknown** – počet bajtov v častiach dokumentu, ktoré podľa nás nenájdeme.

- **Data_DetachedDuration** – ako dlho bola aktivita odpojená od vlákna.

- **Data_Doc_AccessMode** – označuje, či je dokument iba na čítanie alebo sa dá upraviť.

- **Data_Doc_AssistedReadingReasons** – preddefinovaná množina hodnôt, prečo bol dokument otvorený v režime čítania s asistenciou.

- **Data_Doc_AsyncOpenKind** – označuje, či bola otvorená verzia cloudového dokumentu uložená vo vyrovnávacej pamäti a ktorá logika asynchrónneho obnovenia sa použila.

- **Data_Doc_ChunkingType** – jednotky použité na prírastkové otvorenie dokumentu.

- **Data_Doc_EdpState** – nastavenie ochrany elektronických údajov dokumentu.

- **Data_Doc_Ext** prípona dokumentu (docx, xlsb, pptx atď.)

- **Data_Doc_FileFormat** – verzia protokolu formátu súboru.

- **Data_Doc_Fqdn** – názov domény OneDrivu alebo SharePointu Online.

- **Data_Doc_FqdnHash** – jednosmerná hodnota hash zákazníkom identifikovateľného názvu domény.

- **Data_Doc_IdentityTelemetryId** – jednosmerná hodnota hash identity používateľa, ktorá sa používa na vykonanie otvorenia.

- **Data_Doc_InitializationScenario** – zaznamenáva, ako bol dokument otvorený.

- **Data_Doc_IOFlags** – hlási údaje o príznakoch vo vyrovnávacej pamäti, ktoré sa používajú na nastavenie možností požiadavky.

- **Data_Doc_IrmRights** – akcie povolené politikou ochrany elektronických údajov, ktorá platí pre dokument alebo používateľa.
    
- **Data_Doc_IsIncrementalOpen** – príznak, ktorý označuje, že dokument bol otvorený prírastkovo.

- **Data_Doc_IsOcsSupported** – príznak, ktorý označuje, že dokument je podporovaný v službe spolupráce.

- **Data_Doc_IsOpeningOfflineCopy** – príznak, ktorý označuje, že bola otvorená kópia dokumentu v režime offline.

- **Data_Doc_IsSyncBacked** – príznak, ktorý označuje, že v počítači sa nachádza automaticky synchronizovaná kópia dokumentu.

- **Data_Doc_Location** – označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **Data_Doc_LocationDetails** – označuje, ktorý známy priečinok poskytol lokálne uložený dokument.

- **Data_Doc_NumberCoAuthors** – počet používateľov v relácii spoločných úprav.

- **Data_Doc_PasswordFlags** – označuje množinu príznakov hesla Na čítanie alebo Na čítanie a zapisovanie.

- **Data_Doc_ReadOnlyReasons** – dôvody, prečo bol dokument otvorený iba na čítanie.

- **Data_Doc_ResourceIdHash** – anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov.

- **Data_Doc_RtcType** – označuje, ako bol kanál v reálnom čase (RTC) nastavený pre aktuálny súbor (vypnutý, nepodporovaný, na požiadanie, vždy zapnutý atď.).

- **Data_Doc_ServerDocId** – nezmeniteľný anonymný identifikátor dokumentov, ktorý sa používa na diagnostiku problémov. 

- **Data_Doc_ServerProtocol** – verzia protokolu použitá na komunikáciu so službou.

- **Data_Doc_ServerType** – typ servera, ktorý ponúka službu (SharePoint, OneDrive, WOPI atď.).

- **Data_Doc_ServerVersion** – verzia servera, ktorý ponúka službu.

- **Data_Doc_SessionId** – identifikuje konkrétnu reláciu úprav dokumentu v rámci plnej relácie.

- **Data_Doc_SharePointServiceContext** – diagnostické informácie z požiadaviek v SharePointe Online.

- **Data_Doc_SizeInBytes** – indikátor veľkosti dokumentu.

- **Data_Doc_SpecialChars** – indikátor špeciálnych znakov v URL adrese alebo ceste k dokumentu.

- **Data_Doc_StreamAvailability** – indikátor označujúci, či je stream dokumentu k dispozícii alebo vypnutý.

- **Data_Doc_SyncBackedType** – indikátor typu dokumentu (lokálne alebo podľa služby).

- **Data_Doc_UrlHash** – jednosmerná hodnota hash na vytvorenie identifikátora Naïve dokumentu.

- **Data_EditorDisablingRename** – identifikátor prvého editora, ktorý spôsobil vypnutie možnosti premenovania.

- **Data_EditorsCount** – počet editorov v dokumente.

- **Data_ForceReadWriteReason** – celočíselná hodnota vyjadrujúca príčinu vynútenia prechodu súboru do režimu čítania/zapisovania.
    
- **Data_FSucceededAfterRecoverableFailure** – označuje, že otvorenie bolo úspešné po oprave zlyhania počas otvárania dokumentu.

- **Data_LastLoggedTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie, keď pokus o uloženie zlyhá dvakrát (používa sa na diagnostiku kvality údajov).

- **Data_LinkStyles** – označuje, či vytvárame prepojenie na štýly šablóny.

- **Data_MainPdod** – identifikátor dokumentu v procese programu Office Word.

- **Data_Measurements** – šifrovaný reťazec obsahujúci časové rozdelenie jednotlivých častí otvárania. Používa sa na meranie výkonu.

- **Data_MoveDisabledReason** – chyba, pri ktorej sa vypne možnosť premiestnenia dokumentu.

- **Data_MoveFlightEnabled** – či je zapnutá skupina funkcií premiestňovania.

- **Data_PartsUnknown** – počet častí dokumentu, pre ktoré sa nám nepodarilo získať údaje.

- **Data_RecoverableFailureInitiationLocationTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na identifikovanie miesta v kóde, kde sme sa pokúsili opraviť súbor pred jeho otvorením.

- **Data_RenameDisabledReason** – chyba, ktorá spôsobuje vypnutie možnosti premenovania tohto dokumentu.

- **Data_RenameFlightEnabled** – či je zapnutá skupina funkcií premenovania.

- **Data_SecondaryTag** – jedinečná značka pre lokalitu volania kódu, ktorá sa používa na pridanie doplňujúcich údajov o zlyhaní na otvorenie.

- **Data_TemplateFormat** – formát súboru šablóny, na ktorej je dokument založený.

- **Data_UsesNormal** – označuje, či otvorený dokument je založený na normálnej šablóne.


#### <a name="renewuserop"></a>RenewUserOp

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM.  Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú pri vykonávaní operácie obnovenia používateľských certifikátov. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera zapisovača.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.Duration** – celkový čas na dokončenie operácie.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z operácie, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.Result** – úspech alebo zlyhanie operácie.

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu výsledku operácie.

- **RMS.Type** – typ používateľských informácií.

#### <a name="servicediscoveryop"></a>ServiceDiscoveryOp

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM.  Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú pri vykonávaní operácie zisťovania služby. 

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.Duration** – celkový čas na dokončenie operácie.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z operácie, ak sa vyskytla.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.OperationName** – názov operácie

- **RMS.Result** – úspech alebo zlyhanie operácie.

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu výsledku operácie.


### <a name="office-accessibility-configuration-subtype"></a>*Podtyp Konfigurácia zjednodušenia ovládania balíka Office*

Funkcie zjednodušenia ovládania balíka Office

#### <a name="officeaccessibilityaccessibilitytoolsessionpresencewin32"></a>Office.Accessibility.AccessibilityToolSessionPresenceWin32

Umožňuje zistiť, či má používateľ nástroj pomocných technológií pre ľudí s postihnutím, a jeho názov. Vďaka tomu môžeme zistiť, či sa u používateľa balíka Office vyskytnú problémy s konkrétnym nástrojom pomocných technológií pre ľudí s postihnutím.

Zhromažďujú sa tieto polia:

  - **Data\_Data\_Jaws** – označuje, či bol nástroj Jaws spustený počas relácie **Data\_Data\_Magic** – označuje, či bol nástroj Magic spustený počas relácie

  - **Data\_Data\_Magnify** – označuje, či bol nástroj Zväčšovacie sklo spustený počas relácie

  - **Data\_Data\_Narrator** – označuje, či bol nástroj Moderátor spustený počas relácie

  - **Data\_Data\_NVDA** – označuje, či bol nástroj NVDA spustený počas relácie

  - **Data\_Data\_SA** – označuje, či bol nástroj SA spustený počas relácie

  - **Data\_Data\_Supernova** – označuje, či bol nástroj Supernova spustený počas relácie

  - **Data\_Data\_SuperNovaessSuite** – označuje, či bol balík SuperNovaAccessSuite spustený počas relácie

  - **Data\_Data\_WinEyes** – označuje, či bol nástroj WinEyes spustený počas relácie

  - **Data\_Data\_ZoomText** – označuje, či bol nástroj ZoomText spustený počas relácie

#### <a name="officeappledarkmode"></a>Office.Apple.DarkMode

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám hovorí, či používateľ používa systém v režime DarkMode a či používateľ prepísal nastavenie systému v režime DarkMode v Office.  Túto udalosť používame na to, aby sme pomohli zabezpečiť zjednodušenie ovládania a určovať prioritu optimalizácie používateľskej skúsenosti.

Zhromažďujú sa tieto polia:

- **Data_DarkModeIsEnabled** – Či je v systéme povolený režim DarkMode.

- **Data_RequiresAquaSystemAppearanceEnabled** – Či je režim DarkMode prepísaný v Office.

#### <a name="officeapplehardwarekeyboardinuseapple"></a>Office.Apple.HardwareKeyboardInUse.Apple

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám oznamuje, že používateľ pripája k mobilnému zariadeniu klávesnicu. Udalosť nám pomáha zlepšovať zjednodušenie ovládania a optimalizovať používateľskú skúsenosť.

Zhromažďujú sa tieto polia:

- **Data_CollectionTime** – Časová pečiatka označujúca čas zberu udalosti.

#### <a name="officeapplembuinstrumentdeviceaccessibilitysettings"></a>Office.Apple.MbuInstrument.DeviceAccessibilitySettings

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zhromažďuje stav rôznych možností zjednodušenia ovládania, ktoré sú k dispozícii počas relácie. Túto udalosť používame na to, aby sme pomohli zabezpečiť zjednodušenie ovládania a určovať prioritu optimalizácie používateľskej skúsenosti.

Zhromažďujú sa tieto polia:

- **Data_AccessibilityContentSize** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_AssistiveTouchRunning** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_BoldTextEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_CollectionTime** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_DarkerSystemColorsEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_DifferentiateWithoutColor** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_GrayscaleEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_GuidedAccessEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_IncreaseContrast** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_InvertColorsEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_PreferredContentSizeCategory** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_ReduceMotionEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_ReduceTransparency** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_ReduceTransparencyEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_ShakeToUndeEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené. (Neschválené – používa sa len v starých zostavách.)

- **Data_ShakeToUndoEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_SpeakScreenEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_SpeakSelectionEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_SwitchControlRunning** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_UAZoomEnabled** – Príznak, ktorý označuje, či je toto nastavenie povolené.

- **Data_VoiceOverRunning** – Príznak, ktorý označuje, či je toto nastavenie povolené.

#### <a name="officewordaccessibilitylearningtoolsreadaloudplayreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.PlayReadAloud

Táto udalosť označuje, že Office Word číta nahlas text v dokumente. Predstavuje prezenčný signál funkcie zjednodušenia ovládania, ktorá umožňuje spoločnosti Microsoft vyhodnotiť stav funkcie čítania textu nahlas.

Zhromažďujú sa tieto polia:

  - **Data\_ParagraphCount** – počet odsekov v dokumente

  - **Data\_Play** – či Word číta nahlas prvýkrát

  - **Data\_ViewKind** – typ zobrazenia dokumentu

#### <a name="officewordaccessibilitylearningtoolsreadaloudstopreadaloud"></a>Office.Word.Accessibility.LearningTools.ReadAloud.StopReadAloud

Táto udalosť označuje, že Office Word prestal čítať nahlas text v dokumente. Umožňuje spoločnosti Microsoft vyhodnotiť stav funkcie čítania textu nahlas meraním trvania fungovania.

Zhromažďujú sa tieto polia:

  - Žiadne

### <a name="privacy-subtype"></a>*Podtyp ochrany osobných údajov*

Nastavenia ochrany osobných údajov v Office 

#### <a name="officeintelligentserviceprivacyconsentprivacyevent"></a>Office.IntelligentService.PrivacyConsent.PrivacyEvent

Táto udalosť predstavuje akciu spustenú používateľom alebo systémom, ktorá je súčasťou ochrany osobných údajov pre Office. Spustí sa v dialógových oknách ochrany osobných údajov First Run, dialógové okno Ochrana osobných údajov konta a upozornenia na ochranu osobných údajov. Udalosť sa používa na pochopenie nasledujúcich krokov: používateľský súhlas s nastavením ochrany osobných údajov v Office, používateľská zmena nastavenia ochrany osobných údajov v Office a aktualizácia nastavenia ochrany osobných údajov balíka Office v používateľských reláciách.

Zhromažďujú sa tieto polia:

  - **Data_ActionId** – akcia používateľa v dialógovom okne Ochrana osobných údajov

  - **Data_ControllerConnectedServicesState** – nastavenie politiky používateľa s doplnkovými voliteľnými online funkciami

  - **Data_DownloadedContentServiceGroupState** – používateľské nastavenie pre stiahnutý obsah 
 
  - **Data_ForwardLinkId** – prepojenie na dokumentáciu k ochrane osobných údajov pre scenár používateľa

  - **Data_HRESULT** – záznam chýb počas interakcie s dialógovým oknom Ochrana osobných údajov

  - **Data_IsEnterpriseUser** – Kategória používateľských licencií

  - **Data_OfficeServiceConnectionState** – nastavenie pre používateľov online funkcií

  - **Data_RecordRegistry** – záznam zobrazujúci dialógové okno podnikovej ochrany osobných údajov

  - **Data_Scenario** – scenár prvého spustenia založený na používateľskej licencii a kategórii

  - **Data_SeenInsidersDialog** – záznam znázorňujúci dialógové okno Ochrana osobných údajov insiderov

  - **Data_SendTelemetryOption** – používateľské nastavenie pre telemetriu

  - **Data_SendTelemetryOptionPolicy** – používateľské nastavenie ochrany osobných údajov pre telemetriu

  - **Data_UserCategory** – typ používateľského konta  

  - **Data_UserCCSDisabled** – prepísanie používateľom pre doplnkové voliteľné online funkcie

   - **Data_UserContentServiceGroupState** – nastavenie používateľa na analyzovanie obsahu

  - **Data_WillShowDialogs** – záznam používateľa, ktorý potrebuje vidieť dialógové okná ochrany osobných údajov First Run



## <a name="product-and-service-performance-data-events"></a>Udalosti údajov v kategórii Výkon produktov a služieb

Toto sú podtypy údajov v tejto kategórii:
- [Neočakávané ukončenie (zlyhanie) aplikácie](#unexpected-application-exit-crash-subtype)
- [Výkon funkcie aplikácie](#application-feature-performance-subtype)
- [Chyba aktivity aplikácie](#application-activity-error-subtype)

### <a name="unexpected-application-exit-crash-subtype"></a>*Podtyp Neočakávané ukončenie (zlyhanie) aplikácie*

Neočakávané ukončenia aplikácie a stav aplikácie, keď sa to stane.

#### <a name="appstartupreason"></a>app.startup.reason

Táto akcia umožňuje zistiť a vyriešiť problémy, ktoré spôsobili zlyhanie Outlooku pri spustení aplikácie.  Táto udalosť zahŕňa informácie o príčinách zlyhania, aby sme mohli problém rýchlo odstrániť.

Zhromažďujú sa tieto polia: 

- **app_background_time** – trvanie aplikácie na pozadí počas poslednej relácie

- **startup_reason_type** – označuje dôvod spúšťania aplikácie a uvádza, či išlo o dôsledok vynúteného ukončenia alebo o iný dôvod. 

- **watch_status_info** – v prípade potreby sleduje nasledujúce informácie. 

  - **is_watch_app_installed** – určuje, či má používateľ nainštalovanú aplikáciu hodiniek

  - **is_watch_paired** – určuje, či je zariadenie so systémom iOS spárované s hodinkami

  - **is_watch_supported_and_active** – označuje, či sú hodinky počas relácie podporované a aktívne

Nasledujúce polia sa zhromažďujú iba pre službu Outlook Mobile pre iOS:

- **clean_exit_reason** – reťazec slov, ktorý označuje, či bol dôvod na zastavenie aplikácie

- **is_agenda_user** – označuje, či používateľ nedávno otvoril agendu, čo znamená, že sa pri spustení zapisuje disk

- **is_watch_supported_and_active** – označuje, či sú hodinky počas relácie podporované a aktívne


#### <a name="applicationcrash"></a>application.crash

Používa sa na monitorovanie kritických zlyhaní aplikácie a pomáha zhromažďovať informácie o tom, prečo aplikácia zlyhávala a ako tomu predchádzať.

Zhromažďujú sa tieto polia: 

- **android.hardware.** – (napr. android.hardware.bluetooth) hodnoty hardvérovej konfigurácie poskytované platformou Android

- **android.software.** – (napr. android.software.device_admin) hodnoty softvérovej konfigurácie poskytované platformou Android

- **android_version** – názov verzie systému Android v zariadení, ako znázorňuje android.os.Build.VERSION#RELEASE

- **application_package_name** – názov balíka aplikácie, ako znázorňuje android.content.Context#getPackageName()

- **application_stack_trace** – sledovanie zásobníka zlyhania

- **application_version_code** – kód verzie aplikácie, ktorý je definovaný v aplikácii Outlook

- **application_version_name** – názov verzie aplikácie, ktorý je definovaný v aplikácii Outlook 

- **com.** (napr. com.google.android.feature.FASTPASS_BUILD, com.amazon.feature.PRELOAD, com.samsung.android.bio.face) Konfiguračné hodnoty špecifické pre výrobcu, ktoré poskytuje platforma Androidu

- **crash_report_sdk** – súčasť SDK bude posielať denníky zlyhaní. Buď hokej, alebo AppCenter

- **crash_type** – crash_type bude mať ako typy java, natívne a menej závažné.

     - Java – či sa zlyhanie zaznamenalo do aplikačnej vrstvy.

     - Natívne – čo sa zlyhanie zaznamenalo do natívnej vrstvy v támci aplikácie. 

     - Menej závažné – zlyhania sa zaznamenávajú na odstraňovanie chýb funkcií. Aplikácia nezlyhá, ale nahrá denníky menej závažných zlyhaní, ktoré pomôžu pri ladení funkcie.

- **device_brand** – značka zariadenia (výrobca alebo operátor), ako znázorňuje android.os.Build#BRAND

- **device_ID** – jedinečné ID zariadenia (IMEI)

- **device_manufacturer** – výrobca zariadenia, ako znázorňuje android.os.Build#MANUFACTURER

- **device_model** – model zariadenia, ako znázorňuje android.os.Build#MODEL

- **device_name** – názov zariadenia, ako znázorňuje android.os.Build#DEVICE

- **device_total_memory** – odhad celkovej veľkosti pamäte zariadenia na základe štatistík systému súborov.

- **glEsVersion** – kľúč verzie systému OpenGL Embedded Systems


#### <a name="crashevent"></a>crash.event

Umožňuje zistiť a vyriešiť situácie kritických zlyhaní aplikácie a pomáha zhromažďovať informácie o tom, prečo aplikácia zlyhávala a ako tomu predchádzať.

Zhromažďujú sa tieto polia: 

- **crashTime** – dátum a čas zlyhania na pomoc so skúmaním

- **crash_time_from_start** – uplynutý čas od spustenia aplikácie po zlyhanie na pomoc so skúmaním

- **exceptionName** – názov výnimky, ktorá spustila zlyhanie, na pomoc so skúmaním

- **exception_reason** – dôvod výnimky, ktorá spustila zlyhanie, na pomoc so skúmaním

- **hasHx** – uvádza, že konto používa našu novú službu synchronizácie, aby sme mohli zistiť problémy spôsobené touto službou

- **incidentIdentifier** – jedinečné ID zostavy zlyhania, aby sme mohli vyhľadať príslušný problém

- **isAppKill** – pomáha pochopiť, či bola aplikácia v zariadení vypnutá alebo zatvorená

- **is_crashloop** – pomáha nám pochopiť, či by zlyhanie mohlo byť slučkou zlyhania.

- **reportKey** – jedinečné ID pre inštaláciu aplikácie na zariadení na preskúmanie problému

- **signal** – signál, ktorý spôsobil zlyhanie, čím získame ďalšie podrobnosti na preskúmanie zlyhania


#### <a name="error"></a>Chyba

Umožňuje pochopiť problémy, s ktorými sa mobilná aplikácia stretáva pri pokuse o načítanie nastavení ochrany osobných údajov zo servera.

Zhromažďujú sa tieto polia:

- **correlationId** – jedinečné ID pripojenia služby, ktoré vyústilo do chyby, čo nám umožňuje diagnostikovať problém

- **errorCode** – identifikuje príslušný kód chyby prijatý zo služby, ktorý možno použiť na diagnostiku problému

- **exceptionType** – typ chyby, ktorá sa vyskytuje v knižnici pri načítavaní nastavenia

- **hlásenie** – identifikuje chybové hlásenie získané zo služby

- **roamingSettingType** – identifikuje umiestnenie, z ktorého sa pokúšame čítať nastavenia

- **settingId** – nastavenie, ktoré sa pokúsilo načítať

#### <a name="officeappdomainunhandledexceptionhandlerfailed"></a>Office.AppDomain.UnhandledExceptionHandlerFailed

Táto udalosť zhromažďuje informácie o všetkých nespracovaných výnimkách pri používaní aplikácie Data Streamer. Tieto údaje sa používajú na monitorovanie stavu aplikácie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Exception** – zásobník volaní pre výnimku

- **Event Name** – názov udalosti je kategória udalosti a označenie udalosti.

#### <a name="officeappleidentitydomainname"></a>Office.Apple.IdentityDomainName

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu nášho systému, ako aj skúmanie príčin zlyhaní niektorých používateľov domén. Zhromažďujeme informácie o doméne, ktorú naši používatelia použijú, keď sa overujú.  Tieto údaje používame na to, aby sme pomohli určiť a vyriešiť problémy, ktoré zdanlivo nemusia mať príliš veľký vplyv na širšej úrovni, ale ktoré môžu mať veľký vplyv na určitú doménu používateľov.

Zhromažďujú sa tieto polia:

- **Data_Domain** – Doména použitá na overenie.

- **Data_IdentityProvider** – Názov poskytovateľa overenia identity. (LiveId alebo ADAL)

- **Data_IdentityProviderEnum** – Kód poskytovateľa overenia identity. (Číslo)

#### <a name="officeapplesystemhealthappexitmacandios"></a>Office.Apple.SystemHealthAppExitMacAndiOS

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu našich aplikácií balíka Office a skúmanie príčin zlyhaní. Zhromažďujeme údaje pri každom ukončení aplikácie, aby sme zistili, či sa aplikácia ukončila bez zlyhania.

Zhromažďujú sa tieto polia:

- **Data_AffectedProcessSessionID** – Identifikátor relácie, v ktorej dôjde k ukončeniu aplikácie.

- **Data_AffectedSessionBuildNumber** – Vedľajšia verzia aplikácie, v ktorej bolo pozorované ukončenie aplikácie.

- **Data_AffectedSessionDuration** – Dĺžka relácie od začiatku do ukončenia.

- **Data_AffectedSessionIDSMatch** – Indikátor stavu telemetrie.

- **Data_AffectedSessionMERPSessionID** – Indikátor stavu telemetrie.

- **Data_AffectedSessionOSLocale** – Miestne nastavenie operačného systému, v rámci ktorého bolo pozorované ukončenie aplikácie.

- **Data_AffectedSessionOSVersion** – Verzia operačného systému, v rámci ktorého bolo pozorované ukončenie aplikácie.

- **Data_AffectedSessionResidentMemoryOnCrash** – Množstvo rezidentnej pamäte, ktorá sa spotrebovala pri výskyte ukončenia aplikácie.

- **Data_AffectedSessionStackHash** – Identifikátor, ktorý bude označovať výskyt konkrétnej chyby.

- **Data_AffectedSessionStartTime** – Čas, v ktorom relácia začala.

- **Data_AffectedSessionUAEType** – Typ pozorovaného ukončenia aplikácie (ak išlo o ukončenie so zlyhaním, tento kód označí typ zistenej chyby).

- **Data_AffectedSessionVersion** – Hlavná verzia aplikácie, v ktorej bolo pozorované ukončenie aplikácie.

- **Data_AffectedSessionVirtualMemoryOnCrash** – Množstvo virtuálnej pamäte, ktorá sa spotrebovala pri výskyte ukončenia aplikácie.

- **Data_ExitWasGraceful** – Či bola aplikácia ukončená bez zlyhania alebo so zlyhaním.

#### <a name="officeextensibilitycomaddinunhandledexception"></a>Office.Extensibility.COMAddinUnhandledException

Udalosť vygenerovaná pri zlyhaní doplnku COM v spotrebiteľskej verzii aplikácií balíka Office. 

Používa sa na výpočet globálneho „prijatia“ služby Aplikácie Microsoft 365 pre veľké organizácie nešpecifického pre podnik pre doplnok, ktorý potom používajú nástroje, ako je napríklad Readiness Toolkit. Podnikoví zákazníci tak môžu overiť, či sú doplnky nasadené v organizáciách kompatibilné s najnovšími verziami Aplikácií Microsoft 365 pre veľké organizácie a podľa toho naplánovať inováciu. 

Zhromažďujú sa tieto polia:

- **ScopeId** – rozsah aktuálneho vlákna

- **Method** – metóda balíka Office, kde došlo k výnimke

- **Interface** – rozhranie balíka Office, kde došlo k výnimke

- **AddinId** – identifikátor triedy doplnku

- **AddinProgId** – nefunkčné

- **AddinFriendlyName** – nefunkčné

- **AddinTimeDateStamp** – časová pečiatka doplnku z metaúdajov knižnice DLL

- **AddinVersion** – nefunkčné

- **AddinFileName** – nefunkčné

- **VSTOAddIn** – či je doplnok VSTO

- **AddinConnectFlag** – správanie pri aktuálnom načítaní

- **LoadAttempts** – počet pokusov o načítanie doplnku

#### <a name="officeextensibilitycomaddinunhandledexceptionenterprise"></a>Office.Extensibility.COMAddinUnhandledExceptionEnterprise

Udalosť vygenerovaná pri zlyhaní doplnku COM v podnikovej verzii aplikácií balíka Office.

Používa sa na výpočet globálneho „prijatia“ služby Aplikácie Microsoft 365 pre veľké organizácie nešpecifického pre podnik pre doplnok, ktorý potom používajú nástroje, ako je napríklad Readiness Toolkit. Podnikoví zákazníci tak môžu overiť, či sú doplnky nasadené v organizáciách kompatibilné s najnovšími verziami Aplikácií Microsoft 365 pre veľké organizácie a podľa toho naplánovať inováciu. 

- **ScopeId** – rozsah aktuálneho vlákna

- **Method** – metóda balíka Office, kde došlo k výnimke

- **Interface** – rozhranie balíka Office, kde došlo k výnimke

- **AddinId** – identifikátor triedy doplnku

- **AddinProgId** – nefunkčné

- **AddinFriendlyName** – nefunkčné

- **AddinTimeDateStamp** – časová pečiatka doplnku z metaúdajov knižnice DLL

- **AddinVersion** – nefunkčné

- **AddinFileName** – nefunkčné

- **VSTOAddIn** – či je doplnok VSTO

- **AddinConnectFlag** – správanie pri aktuálnom načítaní

- **LoadAttempts** – počet pokusov o načítanie doplnku

#### <a name="officeextensibilitysandboxodpactivationheartbeat"></a>Office.Extensibility.Sandbox.ODPActivationHeartbeat

Doplnky balíka Office sa spúšťajú v sandboxe. Táto udalosť zhromažďuje informácie o prezenčných signáloch pri aktiváciách. Pri zlyhaní doplnku táto udalosť zhromažďuje informácie o dôvodoch zlyhania v prípade, že súvisia s naším sandboxom. Používa sa na vyšetrovanie, keď zákazníci eskalujú problémy.
 
Zhromažďujú sa tieto polia:

- **AppID** – ID aplikácie.

- **AppInfo** – údaje týkajúce sa typu doplnku (pracovná tabla alebo režimu bez používateľského rozhrania alebo obsahu atď.) a typu poskytovateľa (omen, SharePoint, systém súborov atď.).

- **AppInstanceId** – ID inštancie aplikácie. 

- **AssetId** – ID položky aplikácie.

- **ErrorCode** – celkový strávený čas.

- **IsAugmentationScenario** – označuje, či je slučka zväčšenia zodpovedná za spustenie ovládacieho prvku OSF (Office Solutions Framework).

- **IsDebug** – signalizuje, či relácia je reláciou ladenia

- **IsPreload** – označuje, či je doplnok predinštalovaný na pozadí na zlepšenie výkonu aktivácie.

- **IsWdagContainer** – označuje, či sa uskutočňuje aktivácia doplnku v kontajneri aplikácie Windows Defender Application Guard.

- **NumberOfAddinsActivated** – počítadlo aktivovaných doplnkov.

- **RemoterType** – špecifikuje typ služby Remoter (dôveryhodná, nedôveryhodná, Win32webView, dôveryhodná funkcia definovaná používateľom atď.), ktorý sa používa na aktiváciu doplnku.

- **StoreType** – pôvod aplikácie.

- **Tag**– Špecifikuje presné miesto zlyhania kódu pomocou jedinečnej priradenej značky.

- **UsesSharedRuntime** – Označuje, či aplikácia používa sharedRuntime alebo nie.


#### <a name="officeextensibilityvbatelemetrybreak"></a>Office.Extensibility.VbaTelemetryBreak

Udalosť vygenerovaná, keď sa v súbore s povolenými makrami vyskytne chyba kompilácie alebo spustenia

Počítačová analýza: používa sa ako čitateľ vo výpočte stavu špecifického pre podnik pre typy makra (napr. makrá vo Worde, makrá v Exceli atď.), ktoré sa používajú na odvodenie počas pilotného procesu, či je doplnok „pripravený na inováciu“ v produkčnom okruhu.

Zhromažďujú sa tieto polia:

- **TagId** – identifikátor značky telemetrie

- **BreakReason** – dôvod prerušenia (spustenie, kompilácia, iná chyba)

- **SolutionType** – typ riešenia (dokument, šablóna, doplnok aplikácie, doplnok COM)

- **Data.ErrorCode** – kód chyby ohlásený nástrojom VBA


#### <a name="officefindtimeappfailedtostart"></a>Office.FindTime.AppFailedToStart

Zhromažďuje sa, ak spustenie aplikácie zlyhá z dôvodu výskytu neočakávanej chyby počas spúšťania. Používa na sledovanie výnimiek a zlyhaní.  Pomáha monitorovať a ladiť stav aplikácie.

Zhromažďujú sa tieto polia: 

- **DateTime** – časová pečiatka pri prihlasovaní udalosti.

- **EventName** – názov udalosti, ktorá sa práve zaznamenáva

#### <a name="officeoutlookdesktophangbucketmetrics"></a>Office.Outlook.Desktop.HangBucketMetrics

Zhromažďuje čas nereagovania pre nereagovania Outlooku – jedinečný identifikátor pre informácie o nereagovaní, uplynutom čase a zásobníku volaní. Údaje sa používajú na rozpoznávanie a identifikovanie zlyhaní aplikácií, aby ich bolo možné opraviť ich v budúcich aktualizáciách.

Zhromažďujú sa tieto polia:

  - **BucketId** – hodnota hash zásobníka volaní

  - **ElapsedTotal** – celkový čas strávený vo volaní

  - **ElapsedHanging** – čas nereagovania strávený vo volaní

#### <a name="officeoutlookdesktophangreportingscopeperfmetrics"></a>Office.Outlook.Desktop.HangReportingScopePerfMetrics

Zhromažďuje čas trvania základných scenárov Outlooku – switchfolder, switchmodule, sendmailoutbox, openitemclassic, sendmailtransport. Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnych problémov s výkonom. Používa sa na zisťovanie a diagnostiku problémov s výkonom a na zlepšenie výkonu pri každej aktualizácii.

Zhromažďujú sa tieto polia:

  - **ElapsedTotal** – celkový čas strávený vo volaní

  - **ScopeId** – názov funkcie s vyhlásením alebo vlastným názvom priradeným prostredníctvom definície rozsahu

#### <a name="officeoutlookdesktopwatsonbuckets"></a>Office.Outlook.Desktop.WatsonBuckets

Toto pravidlo zhromažďuje informácie o zlyhaní z denníkov udalostí, keď Outlook zlyhal v predchádzajúcej relácii.

Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnych nereagovaní. Používajú sa na rozpoznávanie a identifikovanie nereagovaní, aby ich bolo možné opraviť ich v budúcich aktualizáciách.

Zhromažďujú sa tieto polia:

  - **BucketId** – hodnota hash zásobníka volaní

  - **ElapsedTotal** – celkový čas strávený vo volaní

  - **ElapsedHanging** – čas nereagovania strávený vo volaní

#### <a name="officepowerpointsession"></a>Office.PowerPoint.Session

Zhromažďuje použitia funkcie v jednotlivých reláciách PowerPointu. Tieto údaje sa používajú na výpočet pomeru neželaného ukončenia PowerPointu pri používaní funkcie. Pomer neželaného ukončenia PowerPointu je kľúčový signál na zaručenie, že PowerPoint funguje podľa očakávania.

Zhromažďujú sa tieto polia:

  - **Flag** – príznaky relácie

  - **Usage** – použitia funkcie

#### <a name="officepowerpointuaedialog"></a>Office.PowerPoint.UAE.Dialog

Zhromažďuje sa vždy, keď sa PowerPoint neželane ukončí, keď je otvorené dialógové okno navrchu hlavného okna PowerPointu. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu z dôvodu aktívneho dialógového okna, ktoré blokuje hlavné okno PowerPointu. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **DlgCnt** – celkový počet otvorených dialógových okien pri zlyhaní relácie

  - **DlgId** – identifikátor otvoreného dialógového okna

  - **IdType** – typ identifikátora otvoreného dialógového okna

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **SessionId** – identifikátor zlyhanej relácie

  - **TopId** – identifikátor horného dialógového okna

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaedocument"></a>Office.PowerPoint.UAE.Document

Táto udalosť zhromažďuje informácie o tom, ktorá funkcia sa používa v dokumente, keď sa PowerPoint neželane ukončí. Tieto funkcie môžu zahŕňať prezentáciu, otváranie, ukladanie alebo úpravu dokumentu, spolutvorbu alebo vypínanie. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu pri používaní funkcie. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **CoauthFlag** – príznaky používania spolutvorby

  - **CommandFlag** – príznaky úpravy dokumentu

  - **FileIOFlag** – príznaky používania IO súboru

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **Location** – umiestnenie dokumentu

  - **ServerDocId** – identifikátor dokumentu na serveri

  - **SessionId** – identifikátor zlyhanej relácie

  - **UrlHash** – hodnota hash URL adresy dokumentu

  - **Usage** – použitia funkcie

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaeopen"></a>Office.PowerPoint.UAE.Open

Táto udalosť sa zhromažďuje vždy, keď sa PowerPoint neželane ukončí počas otvárania dokumentu. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu počas otvárania dokumentu. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **FileUrlLocation** – URL umiestnenie dokumentu

  - **Flag** – príznaky otvorenia

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **Location** – umiestnenie dokumentu

  - **OpenReason** – dôvod otvorenia

  - **ServerDocId** – identifikátor dokumentu na serveri

  - **SessionId** – identifikátor zlyhanej relácie

  - **UrlHash** – hodnota hash URL adresy dokumentu

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaesession"></a>Office.PowerPoint.UAE.Session

Táto udalosť zhromažďuje informácie o tom, ktorá funkcia sa používala, keď sa relácia PowerPointu neželane ukončila.  Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **Flag** – príznaky relácie

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **PreviousSessionId** – identifikátor zlyhanej relácie

  - **Usage** – použitia funkcie

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaeshutdown"></a>Office.PowerPoint.UAE.Shutdown

Táto udalosť sa zhromažďuje, keď sa PowerPoint neželane ukončí počas vypínania. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu počas vypínania. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **SessionId** – identifikátor zlyhanej relácie

  - **Stage** – fáza vypnutia

  - **Version** – verzia zlyhanej relácie

#### <a name="officepowerpointuaeslideshow"></a>Office.PowerPoint.UAE.SlideShow

Táto udalosť sa zhromažďuje, keď sa PowerPoint neželane ukončí počas vypínania. Tieto informácie sú dôležité na zachytenie neželaných ukončení PowerPointu počas vypínania. Spoločnosť Microsoft používa tieto údaje na diagnostiku problému, aby sa zaručilo, že PowerPoint funguje podľa očakávaní.

Zhromažďujú sa tieto polia:

  - **InitTime** – čas inicializovania zlyhanej relácie

  - **Mode** – režim prezentácie

  - **SessionId** – identifikátor zlyhanej relácie

  - **State** – stav prezentácie

  - **Version** – verzia zlyhanej relácie


#### <a name="officeprogrammabilityaddinscomaddincrash"></a>Office.Programmability.Addins.COMAddInCrash 

Udalosť vygenerovaná pri načítaní doplnku COM. Používa sa na určenie problémov s prijatím a spoľahlivosťou doplnkov balíka Office. 

Zhromažďujú sa tieto polia:

- **AddinConnectFlag** – predstavuje správanie pri načítaní  

- **AddinDescriptionV2** – popis doplnku 

- **AddinFileNameV2** – názov skutočnej knižnice DLL doplnku. Neobsahuje umiestnenie súboru.

- **AddinFriendlyNameV2** – popisný názov doplnku

- **AddinIdV2** – identifikátor triedy doplnku (CLSID)

- **AddinProgIdV2** – identifikátor programu doplnku 

- **AddinProviderV2** – poskytovateľ doplnku 

- **AddinTimeDateStampV2** – časová pečiatka kompilátora

- **AddinVersionV2** – verzia doplnku 

- **Interface** – rozhranie COM doplnku, ktoré viedlo k zlyhaniu 

- **LoadAttempts** – počet pokusov o načítanie pred zlyhaním 

- **Method** – metóda COM doplnku, ktorá viedla k zlyhaniu 


#### <a name="officeprogrammabilitytelemetryaddincrash"></a>Office.Programmability.Telemetry.AddInCrash

Udalosť vygenerovaná pri načítaní doplnku COM. Tieto informácie sú dôležité na určenie, či doplnok spôsobil zlyhanie aplikácie balíka Office. Používajú sa na posúdenie globálnej kompatibility doplnku s aplikáciami balíka Office.

Zhromažďujú sa tieto polia:

  - **CLSID** – identifikátor triedy doplnku

  - **ConnectFlag** – správanie pri aktuálnom načítaní doplnku

  - **FileName** – názov súboru doplnku bez cesty k súboru

  - **FriendlyName** – popisný názov doplnku

  - **Interface** – rozhranie balíka Office, kde došlo k výnimke

  - **LoadAttempts** – počet pokusov o načítanie doplnku

  - **Method** – metóda balíka Office, kde došlo k výnimke

  - **OfficeApplication** – aplikácia balíka Office, v ktorej došlo k výnimke

  - **OfficeVersion** – verzia balíka Office

  - **ProgID** – identifikátor programu doplnku

#### <a name="officeprogrammabilitytelemetrymacrofileopened"></a>Office.Programmability.Telemetry.MacroFileOpened 

Spúšťa sa pri otváraní súboru obsahujúceho makrá (VBA) v zariadení, ktoré bolo zaradené do aplikácií Office ako služby (OAAS) správcom IT a kde boli Aplikácie Microsoft 365 pre veľké organizácie aktivované pomocou podnikovej licencie. Udalosť sa používa na porozumenie stavu súborov obsahujúcich makrá (VBA) v nájomníkovi a porovnáva sa s udalosťou Office.Programmability.Telemetry.VbaTelemetryBreak, ktorá sleduje chyby v súboroch obsahujúcich VBA. 

Nezhromažďujú sa žiadne polia.

#### <a name="officesystemsystemhealthungracefulappexitmacandios"></a>Office.System.SystemHealthUngracefulAppExitMacAndiOS

Udalosť spustenia, ktorá zachytáva neúspešné ukončenia aplikácie na ďalšie skúmanie.

Zhromažďujú sa tieto polia:

- **AffectedProcessAppBuild** – číslo zostavy.

- **AffectedProcessAppBuildRevision** – číslo revízie zostavy.

- **AffectedProcessAppMajorVer** – číslo hlavnej verzie aplikácie.

- **AffectedProcessAppMinorVer** – číslo vedľajšej verzie aplikácie.

- **AffectedProcessAppName** – názov aplikácie.

- **AffectedProcessResidentMemoryOnCrash** – rezidentná pamäť aplikácie, ktorá zlyhala.

- **AffectedProcessUnsymbolicatedChecksum** – ide s hodnotou hash zásobníka pre symbolizáciu.

- **AffectedProcessVirtualMemoryOnCrash** – virtuálna pamäť aplikácie, ktorá zlyhala.

- **AffectedSessionDuration** – trvanie relácie v sekúnd pred zlyhaním.

- **AffectedSessionLongBuildNumber** – dlhé číslo zostavy.

- **CrashedProcessSessionID** – ID relácie procesu v zlyhaní aplikácie.

- **DetectionTime** – dátum a čas zlyhania aplikácie.
    
- **DeviceModel** – model hardvéru.

- **MERPSessionID** – ID relácie funkcie MERP.

- **ReportingOsLocaleTag** – miestne nastavenie operačného systému.

- **ReportingOSVerStr** – verzia operačného systému.

- **SessionBuildNumber** – verzia aplikácie, ktorá zlyhala.

- **SessionIDSMatch** – boolovská hodnota na overenie, či je hlásené ID relácie rovnaké, aké získala funkcia MERP.

- **SessionVersion** – verzia aplikácie, ktorá zlyhala – **StackHash** – hodnota hash sledovania zásobníka aplikácie, ktorá zlyhala.

- **UAEType** – enumerácia, ktorá poskytuje informácie o tom, o aký typ zlyhania išlo.

#### <a name="officethisaddinstartupfailed"></a>Office.ThisAddIn.StartupFailed

Táto udalosť zhromažďuje informácie o výnimke, ktorá sa vyskytne počas spúšťania aplikácie Data Streamer. Tieto údaje sa používajú na monitorovanie stavu aplikácie. Túto udalosť generuje doplnok Microsoft Data Streamer pre Excel.

Zhromažďujú sa tieto polia:

- **Exception** – zásobník volaní pre výnimku

- **Event Name** – názov udalosti je kategória udalosti a označenie udalosti.

#### <a name="onenotesafebootresetcrashcounteronappsuspend-officeonenoteandroidsafebootresetcrashcounteronappsuspend-officeandroidearlytelemetrysafebootresetcrashcounteronappsuspend"></a>OneNote.SafeBootResetCrashCounterOnAppSuspend, Office.OneNote.Android.SafeBootResetCrashCounterOnAppSuspend, Office.Android.EarlyTelemetry.SafeBootResetCrashCounterOnAppSuspend

Kritický signál sa odošle, keď sa nuluje počítadlo zlyhania pri pozastavení aplikácie pred zobrazením dialógového okna bezpečného spustenia. Táto značka sa vyžaduje na sledovanie a diagnostiku stavu aplikácie. Dialógové okno bezpečného spustenia sa zobrazuje, keď aplikácia zlyhá viackrát za sebou. Používateľovi poskytne možnosť resetovať aplikáciu. Táto značka pomáha zistiť, či sa dialógové okno bezpečného spustenia nezobrazilo používateľovi napriek dosiahnutiu kritérií spustenia. 

Zhromažďujú sa tieto polia:

- Žiadne


#### <a name="telemetryerror"></a>telemetry.error

Táto akcia umožňuje diagnostikovať a vyriešiť problémy, ktoré bránia generovaniu a odosielaniu potrebných diagnostických údajov. Tieto udalosti umožňujú zistiť, či chýbajú dôležité údaje, ktoré sú potrebné na identifikovanie problémov so zabezpečením alebo závažných problémov s fungovaním aplikácie.

Zhromažďujú sa tieto polia: 

- **timer_name** – uvádza, kde sa nachádza problém s telemetriou, napríklad v súčasti poštová schránka alebo v kalendári. Pomôže zistiť a vyriešiť problémy s telemetriou z konkrétnej časti aplikácie.

- **type** – uvádza typ chyby časovača, ktorý nám pomôže zistiť, či sa v aplikácii vyskytnú nejaké problémy s odosielaním údajov diagnostickej telemetrie


#### <a name="watchdoganr"></a>watchdog.anr

Potrebné na monitorovanie chýb výkonu aplikácie, aby sa predišlo tomu, že aplikácia prestane reagovať a obrazovka v aplikácii zamrzne (označované ako aplikácia nereaguje).

Zhromažďujú sa tieto polia: 

- **callstack** – zásobník kódu, v ktorom sa vyskytol stav aplikácia nereaguje
 
- **caused_restart** – označuje, či mala aplikácia nútený reštart pre stav aplikácia nereaguje
 
- **duration** – čas, kedy bolo zariadenie zamrznuté
 
- **id** – jedinečné ID stavu aplikácia nereaguje
 
- **interval** – nakonfigurovaná prahová hodnota na spustenie stavu aplikácia nereaguje
 
- **is_application_object_initialized** – označuje, či stav aplikácia nereaguje nastal po úplnej inicializácii aplikácie alebo pred ňou
 
- **last_known_is_in_foreground** – označuje, či bola aplikácia naposledy v popredí alebo na pozadí


### <a name="application-feature-performance-subtype"></a>*Podtyp Výkon funkcie aplikácie*

Dlhý čas odozvy alebo nízky výkon v prípadoch ako spustenie aplikácie alebo otvorenie súboru.

#### <a name="androidframemetrics"></a>android.frame.metrics

Umožňuje zistiť a vyriešiť situácie, keď naše súčasti aplikácie pre Android spôsobujú problémy s výkonom, napríklad v prípade, že nemôžete plynulo posúvať priečinok doručenej pošty.

Zhromažďujú sa tieto polia: 

- **animation_duration** – trvanie vykresľovania animácie v milisekundách

- **command_issue_duration** – trvanie vydania príkazov pre platformu v milisekundách 

- **draw_duration** – trvanie kreslenia používateľského rozhrania v milisekundách 

- **input_handling_duration** – trvanie spracovania vstupu v milisekundách 

- **layout_measure_duration** – trvanie merania rozloženia v milisekundách

- **origin** – meraná súčasť aplikácie, napríklad kalendár alebo pošta

- **sync_duration** – trvanie synchronizácie snímky v milisekundách

- **swap_buffers_duration** – trvanie výmeny medzipamätí v milisekundách

- **total_duration** – celkové trvanie vykresľovania snímky v milisekundách

- **unknown_delay** – oneskorenie spôsobené neznámymi zdrojmi inými ako explicitne sledované trvania

#### <a name="calcomponent"></a>cal.component

Táto udalosť umožňuje zistiť a vyriešiť problémy, ktoré citeľne vplývajú na výkon súčastí používateľského rozhrania kalendára, čo by malo za následok problém s posúvaním kalendára.

Zhromažďujú sa tieto polia: 

- **above_40fps** – počet snímok vykreslených nad 40 fps

- **above_40fps** – počet snímok vykreslených nad 40 fps

- **above_50fps** – počet snímok vykreslených nad 50 fps

- **above_50fps** – počet snímok vykreslených nad 50 fps

- **above_55fps** – počet snímok vykreslených nad 55 fps

- **above_55fps** – počet snímok vykreslených nad 55 fps

- **account_counter** – sleduje počet kont priradených pre každý typ kalendára, napríklad 2 pre kalendár Gmail a to, či toto konto používa našu novú službu synchronizácie

- **app_instance** – Outlook má dva vstupné body pre Duo, jeden je pre kalendár a jeden je pre poštu a oba možno spustiť súbežne v prostredí s viacerými inštanciami. Umožní nám to zistiť, ktorá inštancia vyvolala tento hovor s hlásením (pošta alebo kalendár)

- **component_name** – uvádza názov súčasti kalendára ako napríklad zobrazenie Agenda alebo zobrazenie Deň, aby sme mohli zistiť problémy s výkonom, ktoré majú vplyv na konkrétnu súčasť kalendára

- **display_frame_data** – sleduje čas strávený zobrazením každých 60 snímok, čo slúži na zistenie výskytu problémov s výkonom. 

- **orientation** – uvádza, či bolo zariadenie v režime na výšku alebo na šírku, aby sme mohli zistiť problémy s výkonom, ktoré majú vplyv na konkrétnu orientáciu zariadenia

- **taskId** – TaskId nám poskytne taskId aktuálnej inštancie. Táto možnosť sa bude vyžadovať v prostredí s viacerými inštanciami, ak chce používateľ spúšťať rovnaké inštancie (kalendár, kalendár alebo pošta, pošta) vedľa seba

- **view_duration** – uvádza, ako dlho trvalo vykresliť rôzne súčasti používateľského rozhrania kalendára, aby sme mohli zistiť problémy s výkonom, ktoré sa prejavia pri používaní kalendára

#### <a name="contactaction"></a>contact.action

Táto udalosť sa spustí na rôznych akciách s kontaktmi – prezeranie, aktualizovanie a odstraňovanie kontaktov, ako aj prezeranie zoznamu kontaktov. Používa sa na určenie, či sa vyskytnú nejaké regresie výkonu súvisiace s kontaktmi.

Zhromažďujú sa tieto polia: 

- **accounts_with_filters** – počet kont s filtrami použitými na zoznam kontaktov

- **action** – typ akcie, ktorá sa vykonala, napr. prezeranie kontaktu
 
- **duration_initial_view_load** – trvanie od otvorenia zobrazenia po prvotné načítanie zoznamu kontaktov

- **duration_show_contacts** – trvanie od otvorenia zobrazenia po zobrazenie kontaktov v zozname kontaktov
 
- **total_contacts** – počet kontaktov bez použitia filtrov
 
- **total_filtered_contacts** – počet kontaktov s použitými filtrami

#### <a name="conversationloadtime"></a>conversation.load.time

Táto udalosť umožňuje zistiť a vyriešiť problémy, ktoré citeľne vplývajú na výkon načítavania e-mailových konverzácií, aby sa vaše e-maily načítavali podľa očakávaní.

Zhromažďujú sa tieto polia: 

- **time** – uvádza, ako dlho trvalo dokončenie načítania e-mailovej konverzácie.

#### <a name="conversationreloaded"></a>conversation.reloaded

Táto udalosť nám umožňuje zistiť, ako často opätovne načítavame konverzáciu na základe oznámení služby. Je potrebné sledovať, či sú oznámenia o aktualizáciách nie sú príliš nahlas a netreba ich stíšiť, pretože sú znižujú kvalitu používania.

Zhromažďujú sa tieto polia: 

- **average** – počet opätovných načítaní vydelený veľkosťou 

- **client-request-ID** – identifikátor požiadavky klienta pre žiadosť, ktorá spôsobila chybu

- **date** – dátumová pečiatka žiadosti, ktorá spôsobila chybu

- **duration** – čas otvorenia konverzácie 


#### <a name="coredatamigration"></a>core.data.migration

Umožňuje zistiť a vyriešiť situácie, pri ktorých sa vyskytla chyba pri aktualizácii e-mailových údajov vo vašom zariadení na novšiu verziu.

Zhromažďujú sa tieto polia:

- **db_size_megabytes** – sleduje veľkosť hlavnej databázy údajov zaokrúhlenú na najbližších 25 MB s maximálnou veľkosťou 500 MB

- **db_wal_size_megabytes** – sleduje veľkosť hlavnej databázy údajov (s nezmeneným súborom hlavného ukladacieho priestoru) zaokrúhlenú na najbližší 1 MB s maximálnou veľkosťou 10 MB

- **free_space_megabytes** – sleduje voľné miesto, ktoré je k dispozícii v sektoroch 10, 100, 1000, 10 000 a 100 000. 

- **migration_duration_seconds** – sleduje trvania migrácie zaokrúhlené na niektorý z týchto časových intervalov – 0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120, 130, 140, 150, 160, 170, 180 (180 a viac by malo byť len 180)

#### <a name="coredataperformance"></a>core.data.performance

Umožňuje zistiť a vyriešiť situácie, keď e-mailové údaje uložené vo vašom zariadení spôsobujú problémy s výkonom.

Zhromažďujú sa tieto polia:

- **Caller** – sleduje názov entity, ktorá vyvolala operáciu uloženia

- **db_size_megabytes** – sleduje veľkosť hlavnej databázy údajov zaokrúhlenú na najbližších 25 MB s maximálnou veľkosťou 500 MB

- **duration** – sleduje čas potrebný na dokončenie operácie

- **entity** – sleduje názov entity, ktorá vyvolala operáciu načítania

- **operation** – nespracovaná hodnota operácie uloženia, načítania alebo „rad čítania/zápisu blokovaný“

#### <a name="inboxcomponent"></a>inbox.component

Táto udalosť zhromažďuje dva typy používateľských údajov: stav predplatného na Microsoft 365 a to, či sa používateľovi zobrazujú reklamy. Táto udalosť nám pomáha zistiť a vyriešiť problémy, ktoré citeľne vplývajú na výkon súčastí používateľského rozhrania doručenej pošty používateľa, čo by malo za následok nesprávne načítanie alebo zobrazenie e-mailových správ, avatara a stavu prečítané/neprečítané.

Zhromažďujú sa tieto polia: 

- **above_40fps** – počet snímok vykreslených nad 40 fps

- **above_40fps** – počet snímok vykreslených nad 40 fps

- **above_50fps** – počet snímok vykreslených nad 50 fps

- **above_50fps** – počet snímok vykreslených nad 50 fps

- **above_55fps** – počet snímok vykreslených nad 55 fps

- **above_55fps** – počet snímok vykreslených nad 55 fps

- **account_counter** – počet každého typu konta v zariadení, napríklad konto služieb Office 365 = 1 konto, konto Outlook.com = 1 konto.

- **ad_not_shown_reason** – dôvod, prečo sa nezobrazujú reklamy

- **ad_shown** – označuje, či sa zobrazila reklama (ak sú povolené reklamy)

- **ad_shown_for_premium** – neočakávané zobrazenie reklamy používateľom s prémiovou verziou

- **age** – vek osoby (používa sa na potvrdenie súladu s vekovým obmedzením reklám) *[Toto pole sa odstránilo z aktuálnych zostáv balíka Office, ale stále sa môže zobraziť v starších zostavách.]*

- **app_instance** – Outlook má dva vstupné body pre Duo, jeden je pre kalendár a jeden je pre poštu a oba možno spustiť súbežne v prostredí s viacerými inštanciami. Umožní nám to zistiť, ktorá inštancia vyvolala tento hovor s hlásením (pošta alebo kalendár)

- **component_name** – názov súčasti/zobrazenia, ktoré je aktívne počas filtrovania

- **has_hx** – označuje, či má zariadenie aspoň 1 konto Hx (naša nová služba na synchronizáciu e-mailov)

- **has_subscription** – označuje, či má zariadenie odber reklám

- **is_all_accounts_inbox** – označuje, či je aktuálny priečinok doručenej pošty priečinok „všetky kontá“

- **is_current_account** – označuje, či je aktuálne aktívne konto kontom reklamy

- **load_error_code** – kód chyby pri načítavaní reklám

- **network_error_code** – kód chyby siete pri žiadosti o reklamy

- **orientation** – orientácia obrazovky v čase udalosti (na výšku alebo na šírku)

- **poskytovateľ** – poskytovateľ (Xandr alebo Facebook) aktuálne zobrazenej reklamy

- **sub_error_type** – podrobný typ chyby

- **taskId** – TaskId nám poskytne taskId aktuálnej inštancie. Táto možnosť sa bude vyžadovať v prostredí s viacerými inštanciami, ak chce používateľ spúšťať rovnaké inštancie (kalendár, kalendár alebo pošta, pošta) vedľa seba

- **total_count** – celkový počet snímok zobrazených súčasťou

- **view_duration** – ako dlho mal používateľ zobrazenú súčasť

#### <a name="initialpagelanding"></a>Initial.page.landing 
 
Táto udalosť pomáha sledovať typ skúsenosti, ktorý sa zobrazí používateľom, keď sa ocitnú na stránke aplikácie.  Tieto údaje sa používajú na určenie prenosov používateľov presmerovaných do jednotlivých skúseností v aplikácii. Okrem toho uľahčujú zlúčenie výsledkov experimentovania.
 
Zhromažďujú sa tieto polia: 

- **Page** – Používa sa na sledovanie typu skúsenosti, ktorá sa používateľovi zobrazí ako prvá, keď sa ocitne našej stránke. Možné hodnoty sú „Trial“, „Skip“, „Prebundled”, „Subscription“ atď.

- **storeExperience** – Používa sa na určenie, či používateľ bol oprávnený zobraziť skúsenosť súpravy SDK pre Obchod.

- **stringVariant** – Používa sa na určenie typu reťazcov, ktoré sa používateľovi zobrazia, keď sa ocitne na našej stránke. Majte na pamäti, že na ľubovoľnej stránke, ako je napríklad „Trial“, môže byť používateľ oprávnený zobraziť rôzne reťazce na základe toho, či si nainštaloval staršiu verziu balíka Office, alebo či predtým aktivoval Office. Možné enumerácie tejto vlastnosti sú „LegacyUpsell“, „OfficeOpened“, „Default“, „YesIntent“, „NoIntent“ atď.

- **windowsBuildType** – Používa sa na sledovanie typu WindowsBuildType, na ktorom sa používateľ nachádza. To znamená „RS4", „RS5“, „RS19H1“, „Vibranium“ atď. Keďže naše skúsenosti sú zvyčajne zamerané na rôzne typy WindowsBuildType, táto vlastnosť je veľmi dôležitá pri odlíšení nasadení. 

#### <a name="ipcpbootstrapuser"></a>IpcpBootstrapUser

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcpBootstrapUser.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.AuthCallbackProvided** – označuje, či poskytuje spätné volanie overovania ako vstup volania rozhrania API alebo nie.

- **RMS.ConnectionInfo.ExtranetUrl** – extranetová URL adresa informácií o pripojení.

- **RMS.ConnectionInfo.IntranetUrl** – intranetová URL adresa informácií o pripojení.

- **RMS.ConnectionMode** – režim pripojenia medzi klientom a serverom služby správy prístupových práv: online alebo offline.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.GuestTenant** – ID hosťovského nájomníka pre používateľa.

- **RMS.HomeTenant** – ID domáceho nájomníka pre používateľa.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Identity.ExtranetUrl** – extranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.IntranetUrl** – intranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.Status** – prvé získanie certifikátu Rights Account Certificate zo servera alebo predĺženie certifikátu Rights Account Certificate. 

- **RMS.Identity.Type** – typ používateľského konta, napríklad konto Windows alebo konto Live.

- **RMS.Identity.UserProvided** – označuje, či e-mailová adresa používateľa bola alebo nebola zadaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.IssuerId** – ID servera služby správy prístupových práv, ktorý vydáva certifikát Rights Account Certificate.  

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.RACType** – typ certifikátu Rights Accounts Certificate.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv. 

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **RMS.TemplatesCount** – počet šablón.

- **RMS.TokenProvided** – označuje, či poskytuje token ako vstup volania API alebo nie. 

- **RMS.UserProvided** – označuje, či poskytuje používateľa ako vstup volania API alebo nie. 

- **UserInfo.UserObjectId** – ID objektu používateľa.

#### <a name="ipcpgetkey"></a>IpcpGetKey

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou správy prístupových práv k informáciám (IRM) alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytnú pri uskutočnení volania API IpcpGetKey.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.ApplicationScenarioId** – ID scenára poskytnuté aplikáciou.

- **RMS.AuthCallbackProvided** – označuje, či poskytuje spätné volanie overovania ako vstup volania rozhrania API alebo nie.

- **RMS.ConnectionMode** – režim pripojenia medzi klientom a serverom služby správy prístupových práv: online alebo offline.

- **RMS.ContentId** – ID obsahu dokumentu.

- **RMS.Duration** – celkový čas na dokončenie volania API.

- **RMS.DurationWithoutExternalOps** – celkový čas mínus spotrebované externé operácie, ako je napríklad latencia siete.

- **RMS.ErrorCode** – kód chyby vrátený z volania API, ak sa vyskytla.

- **RMS.EulId** – ID licencie koncového používateľa.

- **RMS.EulProvided** – označuje, či poskytuje licenciu koncového používateľa ako vstup volania API alebo nie.

- **RMS.GuestTenant** – ID hosťovského nájomníka pre používateľa. 

- **RMS.HomeTenant** – ID domáceho nájomníka pre používateľa.

- **RMS.HttpCall** – označuje, či prebieha operácia HTTP.

- **RMS.Identity.ExtranetUrl** – extranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.IntranetUrl** – intranetová URL adresa servera služby správy prístupových práv pre používateľa zhromažďovaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.Identity.Status** – prvé získanie certifikátu Rights Account Certificate zo servera alebo predĺženie certifikátu Rights Account Certificate. 

- **RMS.Identity.Type** – typ používateľského konta, napríklad konto Windows alebo konto Live.

- **RMS.Identity.UserProvided** – označuje, či e-mailová adresa používateľa bola alebo nebola zadaná počas získavania nového certifikátu Rights Account Certificate zo servera.

- **RMS.IssuerId** – ID servera služby správy prístupových práv, ktorý vydáva certifikát Rights Account Certificate. 

- **RMS.KeyHandle** – pamäťová adresa popisovača kľúča.

- **RMS.LicenseFormat** – formát licencie: Xrml alebo Json.

- **RMS.PL.ExtranetUrl** – extranetová URL adresa v publikačnej licencii

- **RMS.PL.IntranetUrl** – intranetová URL adresa v publikačnej licencii

- **RMS.PL.KeyType** – hodnoty „Single“ alebo „Double“ označujú, či PL bolo chránené s ochranou jednoduchým kľúčom alebo ochranou dvojitým kľúčom.

- **RMS.RACType** – typ certifikátu Rights Accounts Certificate.

- **RMS.Result** – úspech alebo zlyhanie volania API.

- **RMS.ScenarioId** – ID scenára definované rozhraním API.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

- **RMS.ServerType** – typ servera služby správy prístupových práv.

- **RMS.StatusCode** – kód stavu vráteného výsledku.

- **RMS.TemplatesCount** – počet šablón.

- **RMS.TokenProvided** – označuje, či poskytuje token ako vstup volania API alebo nie. 

- **RMS.UserProvided** – označuje, či poskytuje používateľa ako vstup volania API alebo nie. 

- **UserInfo.UserObjectId** – ID objektu používateľa.

#### <a name="jsonparseerror"></a>json.parse.error 
 
Táto udalosť označuje, že analyzátor JSON vyhodil chybu.  Budeme môcť vyriešiť problém s reťazcom načítania databázy Registry, ktorý bol odoslaný do analyzátora JSON, aby sa pre používateľov zabezpečila plynulá skúsenosť.
 
Zhromažďujú sa tieto polia: 

- **Error** – Obsahuje chybové hlásenie, že sa vracia objekt chyby.

#### <a name="mailfiltercomponent"></a>mail.filter.component

Táto udalosť umožňuje zistiť a vyriešiť problémy, ktoré citeľne vplývajú na výkon filtrovania pošty, čo by malo za následok nesprávne načítanie alebo zobrazenie filtrov.

Zhromažďujú sa tieto polia: 

- **above_40fps** – počet snímok vykreslených nad 40 fps

- **above_40fps** – počet snímok vykreslených nad 40 fps
 
- **above_50fps** – počet snímok vykreslených nad 50 fps

- **above_50fps** – počet snímok vykreslených nad 50 fps
 
- **above_55fps** – počet snímok vykreslených nad 55 fps

- **above_55fps** – počet snímok vykreslených nad 55 fps
 
- **account_counter** – počet každého typu konta v zariadení, napríklad konto služieb Office 365 = 1 konto, konto Outlook.com = 1 konto.
 
- **ad_not_shown_reason** – dôvod, prečo sa nezobrazujú reklamy
 
- **ad_shown** – označuje, či sa zobrazila reklama (ak sú povolené reklamy)
 
- **age** vek osoby (používa sa na potvrdenie dodržiavania vekových obmedzení reklám)

- **app_instance** – Outlook má dva vstupné body pre Duo, jeden je pre kalendár a jeden je pre poštu a oba možno spustiť súbežne v prostredí s viacerými inštanciami. Umožní nám to zistiť, ktorá inštancia vyvolala tento hovor s hlásením (pošta alebo kalendár)
 
- **component_name** – názov súčasti/zobrazenia, ktoré je aktívne počas filtrovania
 
- **folder_type** – typ filtrovaného priečinka (napríklad Doručená pošta, Kôš, Nesystémový)
 
- **has_hx** – označuje, či má zariadenie aspoň 1 konto Hx (nová služba na synchronizáciu e-mailov)
 
- **has_subscription** – označuje, či má zariadenie odber reklám
 
- **is_all_accounts_inbox** – označuje, či je aktuálny priečinok doručenej pošty priečinok „všetky kontá“
 
- **is_current_account** – označuje, či je aktuálne aktívne konto kontom reklamy
 
- **load_error_code** – kód chyby pri načítavaní reklám
 
- **network_error_code** – kód chyby siete pri žiadosti o reklamy
 
- **orientation** – orientácia obrazovky v čase udalosti (na výšku alebo na šírku)
 
- **sub_error_type** – podrobný typ chyby

- **taskId** – TaskId nám poskytne taskId aktuálnej inštancie. Táto možnosť sa bude vyžadovať v prostredí s viacerými inštanciami, ak chce používateľ spúšťať rovnaké inštancie (kalendár, kalendár alebo pošta, pošta) vedľa seba
 
- **total_count** – celkový počet snímok zobrazených súčasťou
 
- **view_duration** – ako dlho mal používateľ zobrazenú súčasť

#### <a name="messagerenderingintercepted"></a>message.rendering.intercepted

Táto udalosť nám umožňuje sledovať, ako často používatelia zachytávajú proces vykreslenia ešte pred jeho dokončením. Tieto údaje používame na zisťovanie problémov s výkonom.

Zhromažďujú sa tieto polia: 

- **is_cache** – či sa telo správy načítalo z vyrovnávacej pamäte

- **is_on_screen** – či je proces vykreslenia viditeľný pre používateľov (normálne vykresľovanie)

- **is_rendering_complete** – či sa proces vykreslenia dokončil 

- **is_trimmed_body** – či je telo správy orezané 

- **rendering_method** – spôsob vykreslenia správy

- **rendering_time** – trvanie vykreslenia správy, kým používateľ neopustí stranu

#### <a name="messagerenderingperformance"></a>message.rendering.performance

Táto udalosť nám umožňuje monitorovať výkon procesu vykreslenia správy, aby sme mohli analyzovať výkon jednotlivých procesov vykreslenia a rozpoznať problémy s výkonom. 

Zhromažďujú sa tieto polia: 

- **bundle_prepare_time** – čas na prípravu zväzku na vykreslenie

- **full_rendering_time** – čas procesu úplného vykreslenia

- **is_cache** – či sa telo správy načítalo z vyrovnávacej pamäte

- **is_on_screen** – či je proces vykreslenia viditeľný pre používateľov (normálne vykresľovanie)

- **is_trimmed_body** – či je telo správy orezané 

- **load_message_time** – čas na načítanie správy z backendu (môže to byť 0, ak je správa uložená vo vyrovnávacej pamäti)

- **native_preprocess_time** – čas na predbežné spracovanie tela správy na natívnej strane 

- **prepare_body_time** – čas na prípravu tela správy (vrátane správy o načítaní a predbežnom spracovaní)

- **rendering_method** – spôsob vykreslenia správy

- **rendering_time** – čas vykreslenia správy zväzkom  

- **wait_time** – čas na vytvorenie URL adresy správy


#### <a name="officeandroidandroidofficelaunchtolandingpagelatency"></a>Office.Android.AndroidOfficeLaunchToLandingPageLatency

Dôležité pri zachytávaní metriky výkonu aplikácie s ohľadom na čas odozvy aplikácie od spustenia.  Spoločnosť Microsoft používa túto možnosť na zber času potrebného na odozvu aplikácie a tiež na zisťovanie scenárov, ktoré môžu mať vplyv na čas spustenia v aplikáciách Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:
 
- **AnyCrashInteractionDuringBoot** – Boolovská hodnota pre každé zlyhanie, ktoré sa vyskytne počas štartu

- **AppActivationTimeInMs** – čas fázy aplikácie

- **AppSuspendedDuringBoot** – Boolovská hodnota pre pozastavenie aplikácie počas štartu

- **AvailableMemoryInMB** – dostupná pamäť

- **CollectionTime** – čas udalosti

- **DalvikHeapLimitInMB** – informácie o haldách

- **DocumentRecoveryInvoked** – Boolovská hodnota, ktorá označuje, či bol nejaký dokument obnovený

- **ExtractionDone** – čas extrakcie natívnej knižnice

- **FastBootGainTimeInMs** – čas potrebný na dokončenie rýchleho štartu

- **FileActivationAttempted** – Boolovská hodnota, ktorá označuje, či bolo spustenie aplikácie spôsobené aktiváciou súboru

- **HasLogcatLoggingImpactOnBoot** – Boolovská hodnota, ktorá označuje, či logcat ovplyvnil čas štartu

- **IsThisFirstLaunch** – Boolovská hodnota, ktorá označuje, či ide o prvé spustenie aplikácie

- **LatencyTimeInMilliSec** – oneskorenie v milisekundách

- **LibrarySharingTimeInMs** – čas na zdieľanie knižníc

- **LoadMinLibsTimeInMs** – čas načítania minimálnej množiny knižníc

- **MruListingTimeInMs** – čas potrebný na načítanie MRU

- **NativeLibrariesLoadTime** – čas načítania knižnice CPP

- **NumberOfRunningProcesses** – počet spustených procesov

- **NumberOfRunningProcesses** – počet spustených procesov

- **NumberOfRunningServices** – počet spustených služieb

- **OfficeActivityTimeInMs** – čas na inicializáciu OfficeActivity

- **PostAppInitTimeInMs** – čas fázy aplikácie

- **PreAppInitializationTime** – čas inicializácie fázy aplikácie

- **PreAppInitTimeInMs** – čas fázy aplikácie

- **TotalMemoryInMB** – celková pamäť

- **UIRaaSDownloadLanguagePackageBoot** – informácie týkajúce sa stiahnutia jazykového balíka

- **UserDialogInterruptionDuringBoot** – Boolovská hodnota pre každé blokujúce dialógové okno, ktoré sa zobrazí počas štartu


#### <a name="officeappleappleappbootmac"></a>Office.Apple.Apple.AppBoot.Mac

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zhromažďovanie informácií o čase potrebnom na spustenie aplikácie, ako aj niektorých podrobností o type vykonaného spustenia. Táto udalosť nám pomáha monitorovať náš výkon a prinášať vylepšenia výkonu.

Zhromažďujú sa tieto polia:

- **Data_ Data_EvtBootTimerDocStageReady** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_DocumentRecoveryInvoked** – Či bolo pri spustení použité obnovenie dokumentu.

- **Data_EvtBootTimerBootIdle** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_EvtBootTimerFinishLaunchEnd** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_EvtBootTimerLaunchDidFinish** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_EvtBootTimerLaunchStart** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_EvtBootTimerMainStart** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_EvtBootTimerStaticInit** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_EvtDockStageReady** – Čas, ktorý uplynul do dosiahnutia určitého bodu v kóde.

- **Data_IsFileOpenAttempted** – Či sa vyskytol pokus o otvorenie súboru počas spúšťania.

- **Data_IsFirstRunAttempted** – Či spúšťanie aplikácie prešlo prvým spustením.

- **Data_SentToBackground** – Či bola aplikácia odoslaná na pozadie počas spúšťania.

#### <a name="officeapplediskruleresultserializererroronstreamop"></a>Office.Apple.DiskRuleResultSerializerErrorOnStreamOp

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu infraštruktúry telemetrie. Táto udalosť označuje, že sa vyskytla chyba.

Zhromažďujú sa tieto polia:

- **Data_ActualBytesModified** – Počet zmenených bajtov.

- **Data_BytesRequested** – Počet bajtov na spracovanie.

- **Data_IsWriteOp** – Či sa chystáme vykonať operáciu zapisovania.

#### <a name="officeapplemacbootresourceusage"></a>Office.Apple.MacBootResourceUsage

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zhromažďovanie viacerých indikátorov pre zdroje, ktoré spotrebúvajú aplikácie balíka Office počas spúšťania. Táto udalosť nám pomáha monitorovať náš výkon a prinášať vylepšenia výkonu.

Zhromažďujú sa tieto polia:

- **Data_BlockInputOperations** – Počet operácií blokovania vstupu.

- **Data_BlockOutputOperations** – Počet operácií blokovania výstupu.

- **Data_InvoluntaryContextSwitches** – Počet nedobrovoľných kontextových prepínaní.

- **Data_MainThreadCPUTime** – Meranie uplynutého času.

- **Data_MaxResidentSize** – Meranie veľkosti pamäte.

- **Data_MessagesReceived** – Počet prijatých správ.

- **Data_MessagesSent** – Počet odoslaných správ.

- **Data_PageFaults** – Počet opätovných žiadostí na stránke.

- **Data_PageReclaims** – Počet opätovných žiadostí na stránke.

- **Data_ProcessCPUTime** – Meranie uplynutého času.

- **Data_SharedTextMemorySize** – Meranie veľkosti pamäte.

- **Data_SignalsReceived** – Počet prijatých signálov.

- **Data_Swaps** – Počet prepnutí údajov.

- **Data_SystemCPUTime** – Meranie uplynutého času.

- **Data_SystemUpTime** – Meranie uplynutého času.

- **Data_UnsharedDataSize** – Meranie veľkosti údajov.

- **Data_UnsharedStackSize** – Meranie veľkosti zásobníka.

- **Data_UserCPUTime** – Meranie uplynutého času.

- **Data_VoluntaryContextSwitchesNvcsw** – Počet dobrovoľných kontextových prepínaní.

#### <a name="officeapplemauvalidation"></a>Office.Apple.MAU.Validation

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu súčasti Automatická aktualizácia spoločnosti Microsoft, ktorá sa používa na distribúciu a inštaláciu aktualizácií aplikácií. Zhromaždené údaje sa používajú na zisťovanie chýb a skúmanie príčin zlyhaní.

Zhromažďujú sa tieto polia:

- **Data_EventID** – Zhromažďujeme informácie o reťazci predstavujúcom kód chyby.

- **Data_Message** – Zhromažďujeme informácie o reťazci s popisom chyby.

#### <a name="officeapplembuinstrumenthangdetectionspincontrol"></a>Office.Apple.MbuInstrument.Hang.Detection.Spin.Control

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa zapíše do denníka vždy, keď aplikácia prestane reagovať. Táto udalosť nám pomáha monitorovať náš výkon a prinášať vylepšenia výkonu.

Zhromažďujú sa tieto polia:

- **Data_CountSpinControlStart** – Značka, ktorá označuje, že aplikácia prestala reagovať (alebo reaguje pomaly)

#### <a name="officeapplembuinstrumentvmondocumentclose"></a>Office.Apple.MbuInstrument.VMOnDocumentClose

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zhromažďovanie snímok stavu pamäte počas zatvorenia dokumentu. Táto udalosť nám pomáha monitorovať náš výkon a prinášať vylepšenia výkonu.

Zhromažďujú sa tieto polia:

- **Data_CollectionTime** – Časová pečiatka od momentu zhromaždenia údajov.

- **Data_ResidentMemory** – Zistená hodnota rezidentnej pamäte.

- **Data_VirtualMemory** – Zistená hodnota virtuálnej pamäte.

#### <a name="officeapplembuinstrumentvmonshutdown"></a>Office.Apple.MbuInstrument.VMOnShutdown

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zhromažďovanie snímok stavu pamäte počas vypnutia aplikácie. Táto udalosť nám pomáha monitorovať náš výkon a prinášať vylepšenia výkonu.

Zhromažďujú sa tieto polia:

- **Data_CollectionTime** – Časová pečiatka od momentu zhromaždenia údajov.

- **Data_ResidentMemory** – Zistená hodnota rezidentnej pamäte.

- **Data_VirtualMemory** – Zistená hodnota virtuálnej pamäte.

#### <a name="officeapplembuinstrumentvmonstart"></a>Office.Apple.MbuInstrument.VMOnStart

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zhromažďovanie snímok stavu pamäte počas zapnutia aplikácie. Táto udalosť nám pomáha monitorovať náš výkon a prinášať vylepšenia výkonu.

Zhromažďujú sa tieto polia:

- **Data_CollectionTime** – Časová pečiatka od momentu zhromaždenia údajov.

- **Data_ResidentMemory** – Zistená hodnota rezidentnej pamäte.

- **Data_VirtualMemory** – Zistená hodnota virtuálnej pamäte.

#### <a name="officeapplemsoappdelegatebootperf"></a>Office.Apple.MsoAppDelegate.BootPerf

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zhromažďovanie informácií o čase a pamäti, ktoré počas spúšťania spotrebujú aplikácie balíka Office, ako aj niektorých podrobností o type vykonaného spustenia. Táto udalosť nám pomáha monitorovať náš výkon a prinášať vylepšenia výkonu.

Zhromažďujú sa tieto polia:

- **Data_AppLaunchDurationMicroSec** – Trvanie procesu spúšťania.

- **Data_AppLaunchFinishSystemTime** – Časová pečiatka na určitej značke spúšťacieho kódu.

- **Data_AppLaunchStartSystemTime** – Časová pečiatka na určitej značke spúšťacieho kódu.

- **Data_ResidentMemory** – Snímka dostupnej rezidentnej pamäte počas spúšťania.

- **Data_VirtualMemory** – Snímka dostupnej virtuálnej pamäte počas spúšťania.

#### <a name="officeappleungracefulappexithangsinprevioussession"></a>Office.Apple.UngracefulAppExitHangsInPreviousSession

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu našich aplikácií balíka Office, ako aj skúmanie príčin zlyhaní. Zhromažďujeme informácie o tom, koľkokrát aplikácia prestala reagovať ešte pred ukončením aplikácie so zlyhaním.

Zhromažďujú sa tieto polia:

- **Data_HangsDetected** – Informácia o tom, koľkokrát aplikácia prestala reagovať ešte pred zistením ukončenia aplikácie so zlyhaním.

- **Data_LastSessionId** – Identifikátor relácie, v ktorej sa zistilo ukončenie aplikácie so zlyhaním.

- **Data_SessionBuildNumber** – Vedľajšia verzia aplikácie, v ktorej bolo pozorované ukončenie aplikácie so zlyhaním.

- **Data_SessionVersion** – Hlavná verzia aplikácie, v ktorej bolo pozorované ukončenie aplikácie so zlyhaním.

#### <a name="officeapplewhatsnewerrorandwarning"></a>Office.Apple.WhatsNewErrorAndWarning

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na monitorovanie stavu funkcie Čo je nové. Táto udalosť označuje, že sa vyskytla chyba alebo upozornenie počas analýzy obsahu funkcie Čo je nové a ukazuje na potenciálne problémy s tvorbou obsahu.

Zhromažďujú sa tieto polia:

- **Data_ContentKey** – Ukazovateľ na sekciu obsahu, ktorý pravdepodobne spôsobil chybu.

- **Data_ErrorCode** – Zistený kód chyby (ak je k dispozícii).

- **Data_ErrorDescription** – Popis chyby (ak je k dispozícii).

- **Data_EventID** – Zhromažďujeme informácie o reťazci predstavujúcom typ zistenej chyby.

- **Data_IncludesHTMLTag** – Či obsah obsahuje formát Rich HTML.

- **Data_IncludesItemsTag** – Či obsah obsahuje hierarchiu položiek.

- **Data_LengthOfRawData** – Veľkosť obsahu.

- **Data_RequestURL** – URL adresa, z ktorej bol obsah prevzatý.

- **Data_ServerLanguageTag** – Jazyk obsahu.

- **Data_StatusCode** – Stav chyby (ak je k dispozícii).

#### <a name="officeextensibilityrichapimethodinvocation"></a>Office.Extensibility.RichApiMethodInvocation

Keď zákazník použije doplnok balíka Office a zavolá rozhranie Rich API na poskytnutie služby, spustí sa táto udalosť. Používa sa na meranie spoľahlivosti služby, jej výkonu a používania pri vyvolaní metódy rozhrania Rich API.
 
Zhromažďujú sa tieto polia:

- **Api** – úplný názov rozhrania API.

- **DispFlag** – bitový príznak s popisom typu volania metódy (napr.: 0x1 = METHOD, 0x2 = PROPERTYGET, 0x4 = PROPERTYPUT, 0x8 = PROPERTYPUTREF).

- **DispId** – ID odosielania volanej metódu.

- **HResult** – hodnota HResult volania metódy.

- **Latency** – časové oneskorenie volania v mikrosekundách.

- **ReqId** – identifikátor GUID dávkovej žiadosti, ktorej súčasťou je táto metóda.

- **TypeId** – identifikátor GUID rozhrania, v ktorom je táto metóda volaná.

#### <a name="officeiospaywallfailedscreenretrybuttontap"></a>Office.iOS.Paywall.FailedScreen.RetryButtonTap

Táto telemetria používania sa zhromažďuje na zistenie, keď nákup/zriadenie/aktivácia zlyhali a používateľ ťukol na tlačidlo Skúsiť znova.  Používa sa na riešenie scenárov chýb pri nákupe, ktoré vedú k zopakovaniu pokusu, a na zlepšenie spoľahlivosti procesu.

Zhromažďujú sa tieto polia:

- **failureReason** reťazec – označuje, pre aké zlyhanie používateľ opakuje pokus. Napríklad „provisioningFailed“, „purchaseFailed“, „activationFailed“.

- **productid** – reťazec – AppStore ID produktu, pre ktorý používateľ opakuje zlyhanú požiadavku


#### <a name="officemanageabilityserviceapplypolicy"></a>Office.Manageability.Service.ApplyPolicy

Veľmi dôležitá telemetria na sledovanie zlyhania\\úspešnosti použitia nastavení cloudovej politiky na databázu Registry. Pole LastError obsahuje informáciu o tom, prečo a kde zlyhalo použitie politiky v databáze Registry.

Zhromažďujú sa tieto polia:

  - **Data.ApplyLogMsg** – hlásenie výnimky, ak sa vyskytla, počas aplikovania politiky

  - **Data.Cid** – dynamicky generovaný identifikátor korelácie odoslaný do služby, keď sa uskutočnilo volanie služby na načítanie cloudovej politiky. Používa sa na koreláciu, ktoré volanie spôsobilo problém počas aplikovania politík v cloude.

  - **Data.Last Error** – jedna z piatich hodnôt reťazcov (enumerátorov) na zaznamenanie toho, ktorá fáza aplikovania politiky sa vykonávala, keď sa vyskytla výnimka

#### <a name="officeonenoteandroidsyncprovisioningcompleted"></a>Office.OneNote.Android.Sync.ProvisioningCompleted

*[Táto udalosť sa predtým nazývala OneNote.Sync.ProvisioningCompleted.]*

Kritický signál sa používa na zabezpečenie toho, aby sa po prihlásení používateľa do aplikácie OneNote pre Android správne zriadili poznámkové bloky na zaistenie bezproblémového prístupu k nim. Používa sa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby

Zhromažďujú sa tieto polia: 

- **AppSuspendedDuringEvent** – vráti Boolovskú hodnotu, ktorá označuje, či bola aplikácia počas poskytovania pozastavená

- **NetworkConnection** – typ sieťového pripojenia používaného zariadenia.

- **NetworkDataExchange** – zaznamená počet bajtov vymenených počas poskytovania.

- **ServerType** – vráti typ servera, ktorý ponúka službu

- **TimeTakenInMilliSeconds** – vráti čas potrebný na dokončenie poskytovania v milisekundách

#### <a name="officeonenoteandroidsyncprovisioningerror"></a>Office.OneNote.Android.Sync.ProvisioningError

Kritický signál sa používa na zabezpečenie toho, aby sa po prihlásení používateľa do aplikácie OneNote pre Android správne zriadili poznámkové bloky na zaistenie bezproblémového prístupu k nim. Používa sa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby.

Zhromažďujú sa tieto polia:

- **AppSuspendedDuringEvent** – vráti Boolovskú hodnotu, ktorá označuje, či bola aplikácia počas poskytovania pozastavená

- **ErrorCode** – vráti kód chyby zodpovedný za zlyhanie poskytovania 

- **NetworkConnection**: typ sieťového pripojenia používaného zariadenia

- **NetworkDataExchange** – zaznamená počet bajtov vymenených počas poskytovania.

- **ServerType**: vráti typ servera, ktorý ponúka službu

- **TimeTakenInMilliSeconds**: vráti čas potrebný na dokončenie poskytovania v milisekundách


#### <a name="officeonenoteandroidsyncprovisioningstarted"></a>Office.OneNote.Android.Sync.ProvisioningStarted

*[Táto udalosť sa predtým nazývala OneNote.Sync.ProvisioningStarted.]*

Kritický signál sa používa na zabezpečenie toho, aby sa po prihlásení používateľa do aplikácie OneNote pre Android správne zriadili poznámkové bloky na zaistenie bezproblémového prístupu k nim.  Používa sa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby

Zhromažďujú sa tieto polia: 

- **NetworkConnection** – typ sieťového pripojenia používaného zariadenia.

- **ServerType** – vráti typ servera, ktorý ponúka službu

#### <a name="officeonenotesystembootdialogssafebootdialogpending"></a>Office.OneNote.System.BootDialogs.SafeBootDialogPending 

Kritický signál, ktorý sa používa na sledovanie, keď sa rozhodneme používateľovi zobraziť dialógové okno bezpečného spustenia pri ďalšom spustení systému, pretože spúšťanie neustále zlyhávalo. Používa sa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Ak sa používateľom zobrazuje dialógové okno bezpečného spustenia, vyskytla sa kritická chyba spustenia a tieto informácie nám pomôžu zistiť, koľko používateľov má takúto chybu a koľko používateľov spustí aplikáciu znova a zobrazí si dialógové okno bezpečného spustenia a počet tých, ktorí sa nevrátili.

Zhromažďujú sa tieto polia:

 - Žiadne

#### <a name="officeoutlookdesktopbootperfmetrics"></a>Office.Outlook.Desktop.BootPerfMetrics

Táto udalosť zhromažďuje čas potrebný na spustenie Outlooku. Čas spúšťania Outlooku sa aktívne monitoruje na zisťovanie a diagnostiku regresií. Používa sa aj na diagnostikovanie eskalácií zákazníkov, ako aj na postupné zlepšovanie výkonu spúšťania.

Zhromažďujú sa tieto polia:

  - **AddinElapsedTotal** – celkový čas strávený načítavaním doplnkov

  - **CredPromptCount** – počet zobrazených výziev na zadanie poverení

  - **ElapsedTotal** – celkový čas strávený spúšťaním

  - **IsLoggingEnabled** – či je zapisovanie do denníka povolené

  - **ShowChooseProfileDlg** – či sa zobrazilo dialógové okno výberu profilu

  - **ShowFirstRunDlg** – či ide o prvé spustenie Outlooku

  - **ShowIMAPSrchfldWarningDlg** – výstrahy v prípade konta IMAP s ANSI PST

  - **ShowNeedSupportDlg** – dialógové okno podpory spustené zlyhaním pri spustení

  - **ShowSafeModeDlg** – či sa relácia otvorila v núdzovom režime

  - **ShowScanPstDlg** – zobrazuje, či sa pri kontrole opravy ukladacieho priestoru zobrazilo chybové hlásenie


#### <a name="officeoutlookmacbootperf"></a>Office.Outlook.Mac.BootPerf

Táto udalosť zhromažďuje čas potrebný na spustenie Outlooku. Čas spúšťania Outlooku sa aktívne monitoruje na zisťovanie a diagnostiku regresií. Používa sa aj na diagnostikovanie eskalácií zákazníkov, ako aj na postupné zlepšovanie výkonu spúšťania.

Zhromažďujú sa tieto polia:

- **MacOLKBootPerfDuration** – celkový čas strávený spúšťaním.

- **MacOLKBootPerfID** – identifikátor času stráveného spúšťaním.


#### <a name="officeoutlookmacperformanceunresponsive"></a>Office.Outlook.Mac.PerformanceUnresponsive

Používa sa na identifikovanie problémov s vplyvom na používateľov v Outlooku, ktoré sa môžu prejaviť v zníženom výkone. 

Zhromažďujú sa tieto polia:

- **Duration** – čas, ktorý uplynul pri zníženom výkone.

- **EventType** – typ udalosti so zníženým výkonom.


#### <a name="officeperformanceboot"></a>Office.Performance.Boot

Táto udalosť sa zhromažďuje pri spustení aplikácie balíka Office. Obsahuje informácie o tom, či spustenie bolo iniciované otvorením súboru alebo spustením prostredníctvom ponuky Štart, či išlo o prvé spustenie aplikácie, aké množstvo pamäte aplikácia používa a či sa používateľovi zobrazilo nejaké blokujúce používateľské rozhranie. Používa sa na meranie rýchlosti spustenia aplikácií balíka Office a množstva pamäte, ktoré používajú pri štarte, aby sa zaistilo, že je to prijateľné pre používateľa.

Zhromažďujú sa tieto polia:

- **ActivationKind** – zobrazuje, či sa aplikácia spustila spustením z ponuky Štart, otvorením súboru alebo prostredníctvom automatizácie OLE.
  
- **BootToStart** – či používateľ zvolil zobrazenie domovskej obrazovky po spustení aplikácie.

- **ColdBoot** – uvádza, či je aplikácia balíka Office prvýkrát spustená po reštartovaní systému alebo bolo potrebné načítať z disku binárne rozhranie aplikácie.

- **DeviceModel** – model zariadenia.

- **DocLocation** – pri otváraní dokumentu označuje, ktorá služba poskytla dokument (OneDrive, súborový server, SharePoint atď.).

- **DurationUntilMso20Initialization** – trvanie v mikrosekundách od inicializácie procesu balíka Office po načítanie súboru mso20win32client.dll.

- **Embedding** – označuje, či aplikácia bola otvorená na vkladanie OLE.

- **FirstBoot** – zobrazuje, či išlo o prvé spustenie aplikácie.

- **InitializationDuration** – trvanie prvej inicializácie procesu balíka Office v mikrosekundách.

- **InterruptionMessageId** – ID dialógového okna, ak bolo spustenie prerušené dialógovým oknom s výzvou pre používateľa na zadanie údajov.

- **LegacyDuration** – časový úsek trvania spustenia aplikácie meraný pomocou iných počiatočných a koncových bodov než udalosť Activity.Duration.

- **OpenAsNew** – označuje, či sa aplikácia spustila otvorením existujúceho dokumentu ako šablóny pre nový.

- **TotalWorkingSetMB** – množstvo pamäte v megabajtoch v pracovnej sade procesu.

- **VirtualSetMB** – množstvo pamäte v megabajtoch vo virtuálnej sade procesu. (Len macOS/iOS)

- **WorkingSetPeakMB** – najväčšie množstvo pamäte v megabajtoch, ktoré bolo doteraz v pracovnej súprave procesu.


#### <a name="officepowerpointpptandroidrehearseview"></a>Office.PowerPoint.PPT.Android.RehearseView

Táto udalosť označuje, že používateľ ukončil reláciu skúšky. V kombinácii s Office.PowerPoint.PPT.Android.RehearseView.StartSession pôjde o prvý indikátor akéhokoľvek zlyhania alebo chyby, ktorým používateľ čelí.

Zhromažďujú sa tieto polia:

- **ConnectionCreationTime** – čas na vytvorenie bočných pripojení k služby.

- **CountDownAlertTime** – čas, pre ktorý sa zobrazilo upozornenie na odpočítavanie.

- **CountdownInitTime –** – čas medzi dokončením načítania prezentácie a spustením odpočítavania.

- **CritiqueSummary** – Súhrn toho, čo všetci kritici videli, spolu s ich počtami.

- **ExitEventCode** – kód na identifikáciu toho, v ktorom scenári používateľ ukončil skúšobnú reláciu, či išlo o chybový scenár, alebo úspešné ukončenie. 

- **FRETime** – čas od začatia zobrazovania obrazovky FRE, kým ju používateľ nezrušil. 

- **MicrophonePermissionTime** – čas, pre ktorý sa zobrazilo upozornenie na povolenie mikrofónu, kým používateľ nevybral niektorú z možností.

- **ResumeRehearsingCount** – počet kliknutí používateľa na pozastavenie skúšky.

- **RehearsalInitTime** – čas potrebný na inicializáciu skúšky.

- **ResumeRehearsingCount** – počet kliknutí používateľa na pokračovanie v skúške.

- **Sessionid** – Identifikátor relácie reči. Používa sa na ladenie denníkov služby.

- **SlideshowViewLoadTime** – čas potrebný na načítanie prezentácie.


#### <a name="officepowerpointpptandroidrehearseviewrehearsalsummarypage"></a>Office.PowerPoint.PPT.Android.RehearseView.RehearsalSummaryPage 

Udalosť, ktorá sa spustila pri načítavaní stránky súhrnu. Táto akcia nám pomáha pri zachytávaní výkonu stránky súhrnu. Poskytuje nám informácie o tom, koľko času trvá načítanie stránky služby súhrnu skúšky na klientskom počítači. Je potrebná na udržanie výkonu funkcie. 

Zhromažďujú sa tieto polia:

- **PayloadCreationTime** – čas v milisekundách, ktorý bol potrebný na vytvorenie údajovej časti. 

- **PostUrlCallTime** – čas v milisekundách, ktorý bol potrebný na odoslanie volania po URL adrese. 

- **RehearseSessionId** – identifikátor relácie reči. Môžeme ho použiť na ladenie denníkov služby.

- **RequestPayloadSize** – veľkosť údajovej časti požiadavky. 

- **ResourcesLoadTime** – čas v milisekundách, ktorý bol potrebný na načítanie zdrojov (js, css). 

- **SummaryPageErrorReceived** – Boolovská hodnota, ktorá označuje, či bola prijatá stránka súhrnu alebo sa vyskytla chyba.

- **SummaryPageHtmlLoadTime** – čas v milisekundách, ktorý bol potrebný na načítanie html stránky súhrnu. 

- **SummaryPageHtmlLoadTime** – čas v milisekundách, ktorý bol potrebný na prijatie prvej odpovede zo servera. 

- **SummaryPageLoadTime** – trvanie (v ms) načítania stránky súhrnu. Zahŕňa čas vytvárania údajovej časti 

- **ThumbnailsCount** – celkový počet miniatúr, ktoré budú súčasťou stránky súhrnu. 

#### <a name="officepowerpointpptandroidrehearseviewstartsession"></a>Office.PowerPoint.PPT.Android.RehearseView.StartSession

Udalosť sa spustila, keď používateľ klikol na spustenie relácie. Táto udalosť nám pomáha pri zachytávaní počtu používateľov, ktorí používajú nástroj Presenter Coach v zariadení s Androidom. V kombinácii s Office.PowerPoint.PPT.Android.RehearseView nám poskytne informácie o tom, koľko používateľov úspešne dokončilo skúšobnú reláciu a koľko nie. Toto je náš prvý indikátor zlyhania alebo chýb vo funkcii.
 
Zhromažďujú sa tieto polia:

 - Žiadne


#### <a name="officepowerpointpptsharedrehearseviewerrors"></a>Office.PowerPoint.PPT.Shared.RehearseView.Errors

*[Táto udalosť sa predtým nazývala Office.PowerPoint.PPT.Android.RehearseView.Errors]*

Udalosť, ktorá sa spustí v prípade, že sa vyskytne akákoľvek chyba. Táto udalosť nám pomôže zistiť chyby, ktorým používateľ čelil, a udržať výkon funkcie Prezentačný kouč v mobilnom zariadení.

Zhromažďujú sa tieto polia:

- **Session id:string** – ID relácie skúšky

- **RehearsalEventCode** – kód chyby skúšky


#### <a name="officepowerpointrehearsalsessionmetrics"></a>Office.PowerPoint.Rehearsal.SessionMetrics 

Udalosť spustená, keď sa relácia reči zastaví pre nástroj Presenter Coach. Táto udalosť nám pomáha pri zachytávaní určitých metrík pre reláciu nácviku v nástroji Presenter Coach. Pomôže pri udržaní vysokej kvality služby v budúcnosti.

Zhromažďujú sa tieto polia:

- **ActualRehearseBootTimeInMs** – skutočný čas, ktorý bol potrebný na vytvorenie pripojení.

- **AdaptationTextSize** – veľkosť textu, ktorý sa odosiela do služby.

- **AuthDurationInMs** – Čas v milisekundách potrebný na overenie (obnovenie overovacieho tokenu).

- **AuthError** – Popis chyby overenia, ktorá sa vyskytla (ak vôbec).

- **AvgFragmentLatencyInMs** – Priemerný čas sieťových hlasových správ.

- **ConnectDurationInMs** – Čas v milisekundách potrebný na dokončenie pripojenia relácie. 

- **FirstAudioDelayInMs** – Čas v milisekundách potrebný na prijatie prvých zvukových údajov.

- **FRetriedOnOpenConnection** – Boolovská hodnota, ktorá označuje, či pre otvorenie pripojenia došlo k opakovaniu pokusu alebo nie.

- **InitMediaCaptureLayerDurationInMs** – Čas v milisekundách potrebný na inicializáciu vrstvy zachytávania médií/zvuku.

- **LocallyDroppedMessageCount** – Celkový počet lokálne zrušených správ.

- **NumReconnectAttemptsDuringSession** – označuje počet pokusov o opätovné pripojenie k službe reči.

- **NumTriesDuringEachReconnectAttempt** – toto pole označuje počet pokusov vykonaných počas každého pokusu o opätovné pripojenie.

- **OpenFrontDoorConnectionDurationInMs** – Čas v milisekundách potrebný na otvorenie pripojenia k službe FrontDoor.

- **SendAdaptationTextDurationInMs** – Čas v milisekundách potrebný na odoslanie textu prispôsobenia do služby.

- **ServiceDroppedMessageCount** – Celkový počet správ zrušených službou.

- **SessionDurationInMs** – čas trvania celej relácie, odkedy používateľ klikol na spustenie, kým klikol na zastavenie.

- **SessionId** – Identifikátor relácie reči. Môžeme ho použiť na ladenie denníkov služby.

- **SpeechClientResultEventsWithTimestamps** – Pole prijatých chybových kódov spoločne s časovými pečiatkmi, ktoré môže pomôcť pri ladení.

- **SpeechHResultsWithTimestamps** – Pole prijatých chybových kódov spoločne s časovými pečiatkmi, ktoré môže pomôcť pri ladení.

- **StartSpeechCaptureDurationInMs** – Čas v milisekundách potrebný na spustenie zachytávania reťi.

- **StartSpeechServiceDurationInMs** – pole s časom, ktorý bol potrebný na spustenie relácie reči pri každom výskyte opätovného pripojenia vrátane trvania prvého spustenia relácie reči. 

- **TotalMessageCount** – Celkový počet zvukových správ odoslaných do služby.

- **WebSocketConnectDurationInMs** – Čas v milisekundách potrebný na dokončenie pripojenia webového socketu.


#### <a name="officeuxofficeinsidercanshowofficeinsiderslab"></a>Office.UX.OfficeInsider.CanShowOfficeInsiderSlab

Sledovanie aktivity, či sa blok Office Insider môže zobrazovať používateľovi na karte Konto v používateľskom rozhraní Office Backstage.

Zhromažďujú sa tieto polia:

  - **Data_CanShow** – označuje, či sa blok Office Insider môže zobrazovať používateľovi na karte Konto v používateľskom rozhraní Office Backstage.
  
  - **Data_Event** – nepoužíva sa

  - **Data_EventInfo** – nepoužíva sa

  - **Data_Reason** – nepoužíva sa
 

#### <a name="officeuxofficeinsiderregistercurrentinsider"></a>Office.UX.OfficeInsider.RegisterCurrentInsider

Kritický signál na sledovanie úspechu alebo neúspechu registrácie používateľov pomocou zostáv programu Office Insider, ktorí neboli registrovaní ako insideri pre Office. Hlavným scenárom sú aktuálni insideri pre Office, ktorí sa do programu Office Insider pridali ešte pred zavedením registrácie insiderov pre Office.

Zhromažďujú sa tieto polia:

- **Data_RegisterInsider** – stav registrácie v programe Office Insider.

- **Data_RegisterInsiderHr** – výsledný kód registrácie v programe Office Insider.

- **Data_RegistrationStateCurrent** – aktuálny stav registrácie

- **Data_RegistrationStateDesired** – požadovaný stav registrácie


#### <a name="officeuxofficeinsidershowofficeinsiderdlg"></a>Office.UX.OfficeInsider.ShowOfficeInsiderDlg

Kritické sledovanie signálu interakcie používateľa s dialógovým oknom Zapojte sa do programu Office Insider. Používa sa na identifikáciu všetkých problémov s vykonaním zmien iniciovaných používateľmi, ako je napríklad zapojenie sa do programu Office Insider alebo vystúpenie z neho a zmena úrovne programu Office Insider.

Zhromažďujú sa tieto polia:

- **Data_AcceptedContactMeNew** – označuje, či používateľ prijal, že bude kontaktovaný spoločnosťou Microsoft pri zapojení do programu Office Insider.

- **Data_InsiderLevel** – úroveň programu Insider pri otvorení dialógového okna „Zapojte sa do programu Office Insider“.

- **Data_InsiderLevelNew** – úroveň programu Insider pri zatvorení dialógového okna „Zapojte sa do programu Office Insider“.

- **Data_IsInternalUser** – označuje, či je aplikácia spustená s prihlasovacími údajmi podnikového konta Microsoft.

- **Data_IsInternalUserInit** – označuje, či kód dokázal určiť, či je aplikácia spustená s prihlasovacími údajmi podnikového konta Microsoft.

- **Data_OpenNewsletterWebpage** – označuje, či sa spustilo prepojenie prihlásenia na odber bulletinu Office Insider s podmienkou, že sa používateľ zapojil do programu Office Insider, funkcia odberu bulletinu je zapnutá a používateľ nezrušil otvorenie webovej stránky prihlásenia na odber bulletinu Office Insider.
    
- **Data_RegisterInsider** – stav registrácie v programe Office Insider.

- **Data_RegisterInsiderHr** – výsledný kód registrácie v programe Office Insider.

- **Data_RegistrationStateCurrent** – aktuálny stav registrácie

- **Data_RegistrationStateDesired** – požadovaný stav registrácie


#### <a name="officevisiosharedvisiofilerender"></a>Office.Visio.Shared.VisioFileRender

Táto udalosť zachytáva čas vykreslenia súboru. Pomáha nám uchovávať výkon vykresľovania súboru pod kontrolou.

Zhromažďujú sa tieto polia:

  - **Data\_AvgTime: integer** – priemerný čas vykreslenia kresby Visia v relácii

  - **Data\_CompositeSurfEnabled: bool** * má hodnotu true, ak je povolený režim kompozitného vykresľovania

  - **Data\_Count: integer** – koľkokrát Visio vykreslilo kresbu v relácii

  - **Data\_FirstRenderTime: long** – trvanie vykreslenia súboru pri prvom spustení v milisekundách

  - **Data\_MaxTime: integer** – maximálny čas vykreslenia diagramu Visia v relácii


#### <a name="officevisiovisiofileopenreliability"></a>Office.Visio.VisioFileOpenReliability

Táto udalosť zhromažďuje údaje o výkone otvárania súborov pre Visio Dev16. Používa sa na monitorovanie výkonu funkcie otvárania súborov a spája ho s vlastnosťami súboru, ako je napríklad veľkosť súboru, pre Visio Dev16. Vlastnosti súboru nám umožňujú rýchlejšie ladiť problémy a zistiť ich prvotnú príčinu.

Zhromažďujú sa tieto polia:

  - **Data\_CorrelationId: string** – identifikátor korelácie dokumentu

  - **Data\_DocIsEnterpriseProtected: bool** – má hodnotu true, ak je dokument chránený technológiou Windows Information Protection

  - **Data\_DocumentId: string** – identifikátor GUID cesty k súboru

  - **Data\_DurationToCompleteInMilliseconds: double** – čas potrebný na dokončenie funkcie Uložiť ako v milisekundách

  - **Data\_DurationToCompleteInMillisecondsSquared: double** – druhá mocnina poľa DurationToCompleteInMilliseconds

  - **Data\_ErrorCode: integer** – interný kód chyby pre zlyhanie otvárania súboru

  - **Data\_Extension\_Docs: string** – prípona súboru otvoreného diagramu

  - **Data\_FileIOBytesRead: int** – celkový počet bajtov prečítaných počas ukladania

  - **Data\_FileIOBytesReadSquared: int** – druhá mocnina poľa Data\_FileIOBytesRead

  - **Data\_FileIOBytesWritten: int** – celkový počet bajtov zapísaných počas ukladania

  - **Data\_FileIOBytesReadWritten: int** – druhá mocnina poľa Data\_FileIOBytesWritten

  - **Data\_FileName: binary** – binárna hodnota hash názvu súboru

  - **Data\_FileOpenDownloadDurationInMs: long** – trvanie do stiahnutia súboru v milisekundách

  - **Data\_FileOpenEndDurationInMs: long** – trvanie do otvorenia súboru v milisekundách

  - **Data\_FileOpenTimeStamp: time:** – časová pečiatka začatia otvárania súboru

  - **Data\_FilePathHash: binary** – identifikátor GUID cesty k súboru

  - **Data\_FileSize: long** – veľkosť dokumentu v bajtoch

  - **Data\_FileType: string** – prípona súboru otvoreného diagramu

  - **Data\_IsInternalFile: bool** – má hodnotu true, ak ide o interný súbor. Napríklad vzorkovnica

  - **Data\_IsIRM: bool** – má hodnotu true, ak súbor je chránený technológiou IRM

  - **Data\_IsReadOnly: bool** – má hodnotu true, ak súbor je len na čítanie

  - **Data\_IsSuccess: bool** – má hodnotu true, ak otvorenie súboru bolo úspešné

  - **Data\_Location: string** – umiestnenie súboru, napr. Local, SharePoint, OneDrive, WopiConsumer, WopiBusiness, GenericThirdPartyConsumer

  - **Data\_NetworkIOBytesRead: int** – celkový počet sieťových bajtov prečítaných počas ukladania

  - **Data\_NetworkIOBytesReadSquared: int** – druhá mocnina poľa Data\_NetworkIOBytesRead

  - **Data\_NetworkIOBytesWritten: int** – celkový počet sieťových bajtov zapísaných počas ukladania

  - **Data\_NetworkIOBytesWrittenSquared: int** – druhá mocnina poľa NetworkIOBytesWritten

  - **Data\_OpenLocation:integer** – umiestnenie súboru, z ktorého bol otvorený, 0 lokálny, 1 sieť, 2 SharePoint, 3 web

  - **Data\_Size\_Docs: integer** 

  - **Data\_Tag: string** – jedinečný identifikátor na identifikáciu udalosti Uložiť ako

  - **Data\_WasSuccessful:bool** – má hodnotu true, ak otvorenie ako bolo úspešné


#### <a name="onenoteappsafebootdialogactiontaken-officeonenoteandroidsafebootdialogactiontaken-officeandroidearlytelemetrysafebootdialogactiontaken"></a>OneNote.App.SafeBootDialogActionTaken, Office.OneNote.Android.SafeBootDialogActionTaken, Office.Android.EarlyTelemetry.SafeBootDialogActionTaken

Kritický signál, ktorý sa používa na sledovanie odozvy používateľa, keď uvidí dialógové okno bezpečného spustenia. Dialógové okno bezpečného spustenia sa zobrazuje, keď opakovane zlyhá spustenie. Výber bezpečného spustenia používateľov slúži ako povolenie na odstránenie údajov aplikácie a úspešné spustenie. Používa sa na zabezpečenie kritického regresného zisťovania stavu aplikácie OneNote a služby. Používateľ vidí, keď sa vyskytne kritická chyba spustenia. Tieto informácie pomôžu sledovať, či sa dôvod zlyhania podarilo vyriešiť a používateľ môže aplikáciu úspešne spustiť.

Zhromažďujú sa tieto polia: 

- **DIALOG_ACTION** – na ktoré dialógové tlačilo klikol používateľ – kladné alebo záporné.


#### <a name="perfevent"></a>perf.event

Slúži na sledovanie možného nepriaznivého vplyvu na výkon načítavania rôznych častí aplikácie, ak chcete napríklad zabezpečiť, aby sa pri prvom otvorení aplikácie čo najskôr načítal priečinok doručenej pošty.

Zhromažďujú sa tieto polia: 

- **app_start_show_message_list** – označuje, že sa vyskytol problém s výkonom pri spustení aplikácie, čo spôsobilo, že načítanie zoznamu správ v priečinku doručenej pošty trvalo príliš dlho

- **average** – zhromažďuje počet opätovných načítaní v konverzácii vydelený počtom správ v danej konverzácii.  

- **event_type** – uvádza typ udalosti výkonu, ktorá spôsobila problém s výkonom, aby sme mohli zistiť problémy s určitým typom.   

- **extra_params** – vývojár sem môže pridať ďalšie parametre a poskytnúť nám tak ďalšie informácie o tom, čo môže spôsobovať tento problém s výkonom, t. j. kedy sa táto akcia začala a skončila atď. 

-   **has_work_profile** – označuje, či je aplikácia spustená v rámci pracovného profilu Androidu alebo podobnej konfigurácie s cieľom korelovať analýzu výkonu s týmito prostrediami.

- **profiling_summary** – poskytuje informácie o skupine úloh, počte úloh a priemernej dobe pre tieto skupiny na porozumenie potenciálnym regresiám v konkrétnych oblastiach pri načítavaní aplikácie

- **runtime_performance_monitoring_data** – poskytuje údaje o výkone (čas načítania, počet záznamov) pri načítavaní údajov v rôznych častiach aplikácie.
  - **average_cost_time_ns** – priemerný čas spustenia meraný v nanosekundách.
  - **cost_type** – označuje, či táto udalosť slúži na meranie spustenia vrstvy úložiska alebo celkového trvania.
  - **hx_object_type** – poskytuje podrobný programovací typ objektu merania.
  - **is_main_thread** – označuje, či táto udalosť meria len čas spustenia hlavného vlákna.
  - **record_count** – počet záznamov, ktoré vráti základná vrstva úložiska.
  - **scope_name** – poskytuje názov stránky/súčasti používateľského rozhrania, do ktorj patrí táto udalosť.
  - **total_cost_time_ns** – celkový čas spustenia meraný v nanosekundách. 

- **total_time_elapsed** – uvádza čas potrebný na vykonanie udalosti výkonu, aby sme dokázali pochopiť závažnosť problému s výkonom

#### <a name="performancerecord"></a>performance.record

Táto udalosť slúži na zhromažďovanie metriky výkonu aplikácie. Umožňuje zistiť a vyriešiť situácie, pri ktorých bolo využívanie pamäte a procesora aplikáciou kriticky vysoké alebo došlo k iným problémom s výkonom, čo môže spôsobiť spomalenie zariadenia.

Zhromažďujú sa tieto polia: 

- **app_exit_metric** – metrika o počtoch rôznych typov výkonu ukončení aplikácie v popredí a na pozadí, ktorá nám pomôže porozumieť neočakávaným ukončeniam aplikácie s negatívnymi dôvodmi výkonu.

- **average_suspended_memory** – priemerné množstvo pamäte používanej aplikáciou, keď je pozastavená, slúžiace na porovnanie, aby sme dokázali pochopiť nepriaznivý vplyv na výkon.

- **category** – uvádza, či je aplikácia v popredí alebo na pozadí. Medzi možné hodnoty patria v popredí a na pozadí.

- **cpu_usage** – uvádza vyťaženie procesora aplikáciou slúžiace na porovnanie, aby sme dokázali pochopiť nepriaznivý vplyv na výkon

- **cumulative_CPU_time** – celkové využitie procesora aplikáciou s mierou času, slúžiace na porovnanie, aby sme dokázali pochopiť nepriaznivý vplyv na výkon.

- **cumulative_GPU_time** – celkové využitie času GPU aplikáciou, slúžiace na porovnanie, aby sme dokázali pochopiť nepriaznivý vplyv na výdrž batérie.

- **is_watch_app_installed** – uvádza, či používateľ momentálne používa hodinky Apple Watch a či sú nainštalované, aby sme dokázali pochopiť nepriaznivý vplyv hodiniek na výkon

- **is_watch_paired** – uvádza, či používateľ momentálne používa hodinky Apple Watch a či sú spárované so zariadením, aby sme dokázali pochopiť nepriaznivý vplyv hodiniek na výkon

- **is_watch_supported_and_active** – uvádza, či používateľ momentálne používa hodinky Apple Watch a či sú aktívne, aby sme dokázali pochopiť nepriaznivý vplyv hodiniek na výkon

- **memoAry_used_percentage** – uvádza percento pamäte vyťaženej aplikáciou slúžiace na porovnanie, aby sme dokázali pochopiť nepriaznivý vplyv na výkon

- **memory_used** – uvádza vyťaženie pamäte aplikáciou slúžiace na porovnanie, aby sme dokázali pochopiť nepriaznivý vplyv na výkon

- **peak_memory_usage** – najväčšie množstvo pamäte využité aplikáciou slúžiace na porovnanie, aby sme dokázali pochopiť nepriaznivý vplyv na výkon.

- **scroll_hitch_time_ratio** – pomer času stráveného trhaným pohybom počas posúvania v používateľskom rozhraní, aby sme dokázali pochopiť nepriaznivý vplyv používateľského rozhrania na výkon.


### <a name="application-activity-error-subtype"></a>*Podtyp Chyba aktivity aplikácie*

Chyby funkčnosti funkcie alebo používateľského rozhrania.

#### <a name="assertion"></a>assertion

Táto udalosť umožňuje zistiť výskyt kritických chýb aplikácie, ktoré by mohli spôsobiť jej zlyhanie alebo závažné problémy, ako je napríklad zobrazenie prázdnych riadkov v doručenej pošte.

Zhromažďujú sa tieto polia:

- **count** – celkový počet položiek priradených k chybe; napríklad počet kalendárov s chybami

- **has_hx** – uvádza, že konto používa našu novú službu synchronizácie, aby sme mohli zistiť problémy spôsobené touto službou

- **host_name** – názov hostiteľa služby, ktorý sa podieľal na chybe, aby sme mohli zistiť problémy s konkrétnym hostiteľom

- **host_type** – typ hostiteľa, ktorý sa podieľal na chybe, aby sme mohli zistiť problémy s konkrétnym typom hostiteľa

- **message** – vlastná správa s tvrdením, ktorá sa používa na diagnostikovanie problému 

- **origin** – pôvod chyby v kóde, aby sme mohli zistiť problémy s určitou časťou kódu

- **stacktrace** – sledovanie zásobníka, v ktorom sa vyskytlo tvrdenie, aby sme mohli zistiť problémy s určitou časťou kódu

- **type** – typ chyby tvrdenia, ktorá sa vyskytla, napríklad null_folder_name a compose_selected_null_account, aby sme mohli zistiť problémy s určitou časťou kódu

#### <a name="editcontacterror"></a>edit.contact.error

Umožňuje zistiť a vyriešiť situácie, pri ktorých sa pri pokuse o zobrazenie alebo úpravu kontaktov v aplikácii objavili chyby.

Zhromažďujú sa tieto polia: 

- **errorType** – typ chyby, ktorá sa vyskytla, aby sme mohli diagnostikovať problém

- **field** – pole kontaktu, ktoré sa používateľ pokúšal upraviť, aby sme mohli diagnostikovať problém

- **version** – verzia služby karty kontaktu, ktorú používame na diagnostiku problému

#### <a name="errorreport"></a>error.report

Táto udalosť rozpoznať zistiť, či sa vyskytli kritické chyby aplikácie, aby sme mohli zabrániť problémom, ktoré by mohli spôsobiť zlyhanie aplikácie alebo zabránenie čítaniu e-mailov. 

Zhromažďujú sa tieto polia: 

- **client-request-id** – identifikátor požiadavky klienta pre žiadosť, ktorá spôsobila chybu
 
- **date** – dátumová pečiatka žiadosti, ktorá spôsobila chybu

- **error** – typ chyby, napríklad get_mailbox_location_failed
 
- **error_body** – telo chybového hlásenia
 
- **is_x_mailbox_anchor_set** – označuje, či bola v žiadosti nastavená vlastnosť X-AnchorMailbox
 
- **reason** – dôvod chyby, t. j. chybové hlásenie
 
- **request-id** – identifikátor požiadavky servera pre žiadosť, ktorá spôsobila chybu
 
- **source** – zdroj chyby v rámci infraštruktúry OM, zvyčajne je to „BE“ alebo „FE“


#### <a name="officeairspacebackendwin32graphicsdriversofthang"></a>Office.AirSpace.Backend.Win32.GraphicsDriverSoftHang 

Táto udalosť pomáha spoločnosti Microsoft oddeľovať dlhé nereagovania ovládača grafickej karty od krátkych, čo pomáha pri rozhodovaní o tom, ktoré ovládače grafickej karty môžu mať problémy. Ovládač grafickej karty používateľa spôsobil nereagovanie balíka Office, ale vplyv nereagovania ešte nie je známy.

Zhromažďujú sa tieto polia:

  - **Údaje\_InDeviceCall** – metóda zavolaná grafickou kartou, ktorá spôsobila nereagovanie

  - **Data\_Timeout** – ako dlho nereagovanie trvalo

  #### <a name="officeandroidadalsigninuiprompts"></a>Office.Android.ADALSignInUIPrompts

Táto udalosť označuje, že sa používateľovi zobrazila výzva na prihlásenie do školského alebo pracovného konta.  Táto udalosť pomáha porozumieť stavu prihlásenia našich aplikácií a vykonať príslušné akcie, keď si všimneme neočakávané opakované výzvy na prihlásenie. 

Zhromažďujú sa tieto polia:

- **LastLoginDelta** – čas od posledného úspešného prihlásenia.

- **PreviousIdentityCredProviderState** – označuje stav konta.

- **PreviousIdentityState** – označuje stav konta, napríklad uplynutie platnosti relácie. 

- **SignInResultCode** – označuje kód výsledku ukončenia výzvy na prihlásenie.

- **UseCache** – označuje, či sme vynútili výzvu pre používateľa na opätovné zadanie hesla.

- **UserType** – označuje, či ide o existujúce konto alebo nové konto.

#### <a name="officeandroidandroidappdocsfileoperationends"></a>Office.Android.AndroidAppDocsFileOperationEnds

Údaje telemetrie Critical Docs Android Only (AppDocs) pre koncové operácie Súbor Nový/Otvoriť/Uložiť ako. Týmto sa zachytávajú kódy chýb pre zlyhania týchto operácií AppDocsOperations.  Spoločnosť Microsoft používa túto možnosť na identifikovanie zlyhaní v rôznych operáciách súborov a presnej vrstvy, v ktorej došlo k zlyhaniu aplikácií Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **AccessMode** – hodnota enumerácie režimu prístupu pre súbor. Hodnoty – None, ReadOnly, ReadOnlyUpgradable, ReadWrite

- **BlockingUIShown** – Boolovská hodnota, ktorá označuje, či sa zobrazilo blokovacie používateľské rozhranie kdekoľvek v postupe.

- **ContentUriAuthority** – autorita URL adresy obsahu z SAF

- **Correlation** – identifikátor GUID pre ID korelácie v súvislosti s operáciou

- **DocId** – ID dokumentu vygenerované AppDocs

- **DocInstanceId** – DocInstanceId ID inštancie dokumentu vygenerované AppDocs, ktoré je zamerané na inštanciu operácie v dokumente

- **DocIsEnterpriseProtected** – Boolovská hodnota, ktorá označuje, či je dokument chránený.

- **DocUserId** – ID používateľa z vrstvy overenia MS

- **DocUserIdProvider** – enumerácia predstavujúca poskytovateľa ID používateľa, 0 = neznáme, 1 = LiveId; 2 = OrgId, 3 = SSPI, 4 = ADAL

- **DurationInMs** – čas v milisekundách na ukončenie operácie súboru

- **EndReason** – hodnota enumerácie pre dôvod ukončenia.  Hodnoty – None, Success, Failure, Cancel

- **ErrorCode** – kód chyby pre operáciu súboru

- **Extension** – prípona otvoreného súboru.

- **FileSourceLocation** – hodnota enumerácie pre umiestnenie súboru. Možné hodnoty: None, Local, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, UnknownServer

- **FILETIME** – čas udalosti

- **FirstBCSClientError_Info** – informácie o kóde chyby v súvislosti s konverziami súborov

- **HttpStatusCode**-http – kód odozvy HTTP pre žiadosť o webovú službu

- **InitalizationReason** – vstupný bod pre otvorenie súboru

- **K2FileIOHresult** – kód Hresult pre ukončenie operácie otvorenia súboru

- **LastBCSClientError_TagId** – posledná chyba klienta BCS (Binary Conversion Service)

- **OfficeWebServiceApiStatusFlag** – príznak stavu pre žiadosť o webovú službu

- **OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia v skutočnosti ukončila

- **OpFlags** – príznaky parametrov operácií s dokumentom, ktoré používa vrstva AppDocs.

- **OpSeqNum** – číslo, ktoré predstavuje postupnosť volaní súvisiacich s operáciami súborov vo vrstve AppDocs

- **OpType** – enumerácia typu operácie. Hodnoty: "None", "CreateDocument", "OpenDocument", "CopyDocument", "CloseDocument", "SaveDocument", "OpenVersion", "CloseVersion"

- **PreFetchState** – enumerácia stavu prednačítania šablón pre operácie vytvorenia nových súborov.

- **ProviderApp** – názov balíka aplikácie, z ktorej sa súbor otvoril

- **ScopeInstanceId** – ID inštancie rozsahu, ktoré sa používa na pripojenie kontextu údajov k aktivitám

- **Size** – veľkosť súboru

- **State** – hodnota enumerácie pre stav súboru. Hodnoty: None, Creating, Created, CreateFailed, Opening, Opened, OpenFailed, Copying, Copied, CopyFailed, Closing, Closed, CloseFail

- **TemplateName** – binárny názov šablóny v šablóne dokumentu zo služby šablón, napríklad TF10002009.dotx.

- **UriScheme** – schéma URL adresy

#### <a name="officeandroidandroidautherror"></a>Office.Android.AndroidAuthError

Táto udalosť označuje zlyhania základného overenia počas bezobslužného obnovovania tokenu, načítanie prihlasovacej stránky zo služby a podobne.  Táto udalosť pomáha porozumieť stavu prihlásenia našich aplikácií, vykonaným pokusom o prihlásenie, a vykonať príslušné akcie, keď si všimneme neočakávané zlyhania. 

Zhromažďujú sa tieto polia:

- **ADALErrorCode** – označuje kód chyby pri zobrazení výzvy na prihlásenie alebo bezobslužného pokusu o načítanie tokenu pre pracovné konto.

- **ADALRawErrorCode** – označuje kód chyby RAW pri zobrazení výzvy na prihlásenie alebo bezobslužného pokusu o načítanie tokenu pre pracovné konto.

- **ErrorGroup** – označuje typ konta, napríklad osobné konto alebo pracovné konto, alebo lokálne pracovné konto.

- **IDCRLErrorCode** – označuje kód chyby pri zobrazení výzvy na prihlásenie pre osobné konto.

- **IDCRLRawErrorCode** – označuje kód chyby RAW pri zobrazení výzvy na prihlásenie pre osobné konto.

- **LiveOAuthErrorCode** – označuje kód chyby počas bezobslužného pokusu o obnovenie tokenu pre osobné konto.

- **LiveOAuthRawErrorCode** – označuje kód chyby RAW počas bezobslužného pokusu o obnovenie tokenu pre osobné konto.

- **NTLMErrorCode** – označuje kód chyby pri zobrazení výzvy na prihlásenie pre lokálne pracovné konto.

#### <a name="officeandroidandroidfileasyncsavestatus"></a>Office.Android.AndroidFileAsyncSaveStatus

Zachytáva údaje o stave asynchrónnych uložení súborov a rôzne kódy chýb z rôznych súčastí.  Spoločnosť Microsoft používa tieto údaje na analýzu toho, či došlo k strate údajov používateľa v aplikácii počas ukladania súborov v aplikáciách Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **FileExtension** – prípona súboru

- **FileIOSaveHResult** – hodnota HResult operácie uloženia súboru

- **FileIOSaveIsCopy** – Boolovská hodnota, ktorá označuje, či sa v rámci operácie ukladá kópia.

- **FileSize** – veľkosť súboru

- **FileSourceLocation** – enumerácia pre umiestnenie zdroja súboru. Hodnoty: None, Local, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, UnknownServer

#### <a name="officeandroidandroidfileopenreliability"></a>Office.Android.AndroidFileOpenReliability

Zachytáva údaje o stave otvorenia súboru a rôzne kódy chýb na identifikovanie toho, aké zlyhania otvorenia súboru sú očakávané a neočakávané a ktorá časť kódu ich nahlasuje.  Spoločnosť Microsoft používa tieto údaje na analýzu príčin zlyhaní otvorení súborov a výpočet kritickej metriky, napríklad miery úspešnosti otvorení súborov v aplikáciách Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **AccessMode** – enumerácia režimu prístupu

- **AppDocsFileOpenErrorCode** – kód chyby AppDocs v prípade zlyhania otvorenia súboru

- **ContentUriAuthority** – autorita URL adresy obsahu z SAF

- **DownloadCsiError** – hlásenie chyby pri sťahovaní z CSI

- **FileExtension** – prípona súboru

- **FileOpenEndErrorCode** – kód chyby v prípade zlyhania otvorenia súboru

- **FileOpenStatus** – enumerácia stavu otvorenia súboru

- **FileSize** – veľkosť súboru

- **FileSourceLocation** – enumerácia umiestnenia súboru

- **FirstBCSClientError_Info** – posledná chyba klienta BCS (Binary Conversion Service)

- **IfWordFileOpencanceled** – či bolo otvorenie súboru vo Worde zrušené používateľom

- **InitializationReason** – enumerácia pre vstupný bod otvorenia súboru

- **IsAutoSaveDisabled** – či je automatické ukladanie vypnuté počas otvorenia súboru

- **IsFileEmpty** – Boolovská hodnota, ktorá označuje, či je súbor prázdny

- **K2FileIOHresult** – hodnota Hresult pre ukončenie operácie súboru

- **OpenCsiError** – hlásenie chyby otvorenia súboru vo vrstve CSI

- **OpEndEventId** – značka, kde sa operácia v skutočnosti ukončila

- **PPTHresult** – hodnota Hresult v PPT

- **PPTIsExpectedError** – klasifikácia chyby PPT pre očakávané/neočakávané zlyhanie otvorenia súboru 

- **PPTTag** – značka chyby v PPT

- **ProviderApp** – názov balíka aplikácie, z ktorej sa súbor otvoril

- **ProviderFileSize** – veľkosť súboru zachytená pri otváraní súboru prostredníctvom aktivácie súboru

- **State** – enumerácia stavu otvorenia súboru

- **UriScheme** – schéma URL adresy

- **WordErrortag** – značka chyby vo Worde

- **WordFileCorruptionReason** – dôvod poškodenia, ktorý môže spôsobiť zlyhanie otvorenia wordového súboru

- **WordFileOpenErrorCode** – špecifický kód chyby otvorenia súboru vo Worde.

- **WordFileTypeFromDod** – typ súboru určený Wordom na základe skutočného formátu súboru

- **WordFileTypeFromExtension** – typ súboru určený Wordom na základe prípony súboru

#### <a name="officeandroidandroidfilesavestatus"></a>Office.Android.AndroidFileSaveStatus

Dôležité na zachytávanie údajov o stave uložení súborov a rôznych kódov chýb z rôznych súčastí.  Spoločnosť Microsoft používa tieto údaje na analýzu toho, či došlo k strate údajov používateľa v aplikácii počas ukladania súborov v aplikáciách Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **AccessMode** – Hodnoty** – None, ReadOnly, ReadOnlyUpgradable, ReadWrite.

- **AppDocsEndReason** – enumerácia pre dôvod ukončenia uloženia súboru AppDocs EndReason.  Hodnoty: None, Success, Failure, Cancel.

- **AppDocsErrorCode** – posledný kódu chyby pri zlyhaní ukladania súboru

- **AppDocsTriggeringSaveDetails** – pole, ktoré označuje, či AppDocs spúšťa uloženie

- **DocInstanceId** – DocInstanceId ID inštancie dokumentu vygenerované AppDocs, ktoré je zamerané na inštanciu operácie v dokumente

- **ExcelFileSaveResult** – špecifický kód HResult v Exceli

- **FileExtension** – prípona súboru.

- **FileIOSaveErrorCode** – kód chyby vo FileIO

- **FileIOSaveHResult** – kód HResult vo FileIO

- **FileIOSaveIsCopy** – Boolovská hodnota, ktorá označuje, či ide o operáciu kópie.

- **FileSize** – veľkosť súboru

- **FileSourceLocation** – enumerácia umiestnenia súboru.  Hodnoty: None, Local, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, UnknownServer

- **OpFlags** – príznaky operácie uloženia

- **PPTFileSaveFailHresult** – kód HResult v PPT pri zlyhaní uloženia

- **PPTFileSaveFailTag** – značka v PPT pri zlyhaní uloženia

- **State** – enumerácia stavu otvorenia súboru. 

- **Hodnoty** – None, Creating, Created, CreateFailed, Opening, Opened, OpenFailed, Copying, Copied, CopyFailed, Closing, Closed, CloseFail

- **WordFileCopyErrorTrackbackTag** – značka odkazu pri zlyhaní vo fáze CopyDocument vo Worde

- **WordFileSaveCancelReason** – značka odkazu pri zrušeniach vo Worde

- **WordFileSaveEid** – špecifický kód chyby pre Word

- **WordFileSaveErrorTrackbackTag** – značka odkazu pri zlyhaniach uloženia

- **WordFileSaveOpResult** – enumerácia pre stav výsledku 0 v prípade úspechu, 1 v prípade zlyhania, 2 v prípade zrušenia

- **WordFileSaveSuccess** – enumerácia pre špecifické podrobnosti vo Worde pri úspešnej operácii uloženia súborov.

#### <a name="officeandroidandroidofficeactivationlatency"></a>Office.Android.AndroidOfficeActivationLatency

Dôležité údaje na zhromažďovanie komplexného času otvorenia súborov pre všetky otvorenia súborov v aplikáciách Windows, Excel a PowerPoint.  Spoločnosť Microsoft používa túto možnosť na zistenie metriky pre výkon našich aplikácií pri otváraní súborov

Zhromažďujú sa tieto polia:

- **AppBootingOccured** – Boolovská hodnota na kontrolu, či je štart aplikácie dokončený

- **ApplicationBootTime** – čas potrebný počas konkrétnej fázy štartu aplikácie

- **AppSuspendedDuringBoot** – Boolovská hodnota, ktorou sa kontroluje, či bola aplikácia pozastavená počas štartu

- **BlockingUIShownDuringFileOpen** – Boolovská hodnota, ktorá označuje, či sa počas operácie otvorenia súboru zobrazilo nejaké blokovacie dialógové okno

- **CachedInfoAvailable** – Boolovská hodnota, ak hľadáte informácie vo vyrovnávacej pamäti špecifické pre operáciu otvorenia súboru

- **DocumentRecoveryInvoked** – Boolovská hodnota, ktorá označuje, či nejaký dokument čakal na obnovenie

- **EndToEndActivationTime** – čas potrebný na vykreslenie súboru pre súbory otvorené mimo aplikácie

- **EndToEndFileOpenTime** – čas potrebný na vykreslenie súboru pre súbory otvorené v rámci aplikácie

- **FileOpenPhaseDurationInMs** – čas operácie otvorenia súboru spotrebovaný v konkrétnej fáze

- **FileSourceLocation** – hodnota enumerácie pre umiestnenie súboru, napríklad None, Local, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, UnknownServer

- **InitalizationReason** – vstupný bod pre otvorenie súboru

- **InitialBootPhaseTime** – čas potrebný počas konkrétnej fázy štartu aplikácie

- **IsThisFirstLaunch** – Boolovská hodnota, ktorá označuje, či je toto prvé spustenie aplikácie

- **MinimumLibraryLoadPhaseTime** – čas potrebný počas konkrétnej fázy štartu aplikácie

- **MinimumLibraryLoadPhaseTime** – čas potrebný počas konkrétnej fázy štartu aplikácie

- **MinimumLibraryLoadPhaseTime** – čas potrebný počas konkrétnej fázy štartu aplikácie

- **PostAppInitTimeInMs** – čas potrebný počas konkrétnej fázy štartu aplikácie

- **PPTRenderPhase** – čas, ktorý sa vzťahuje na konkrétnu fázu vo vykresľovaní v PPT

- **PreAppInitTimeInMs** – čas potrebný počas konkrétnej fázy štartu aplikácie

- **ProviderApp** – názov balíka aplikácie, z ktorej sa súbor otvoril

- **TelemetryReason** – hodnota enumerácie, ktorá je podobná ako InitialisationReason, ale podrobnejšia ohľadom vstupného bodu otvorenia súboru.

- **UserDialogInterruptionDuringBoot** – Boolovská hodnota, ktorá označuje, či sa počas štartu zobrazilo nejaké blokujúce dialógové okno

- **XLRenderPhase** – čas, ktorý sa vzťahuje na konkrétnu fázu vo vykresľovaní v Exceli

#### <a name="officeandroidappdocsfileoperationends"></a>Office.Android.AppDocsFileOperationEnds

Údaje telemetrie Critical Docs Android Only (AppDocs) pre koncové operácie Súbor Nový/Otvoriť/Uložiť ako. Týmto sa zachytávajú kódy chýb pre zlyhania týchto operácií AppDocsOperations.  Spoločnosť Microsoft používa túto možnosť na identifikovanie zlyhaní v rôznych operáciách súborov a presnej vrstvy, v ktorej došlo k zlyhaniu aplikácií Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **AccessMode** – hodnota enumerácie režimu prístupu pre súbor.  Hodnoty: None, ReadOnly, ReadOnlyUpgradable, ReadWrite

- **BlockingUIShown** – Boolovská hodnota, ktorá označuje, či sa zobrazilo blokovacie používateľské rozhranie kdekoľvek v postupe.

- **ContentUriAuthority** – autorita URL adresy obsahu z SAF

- **Correlation** – identifikátor GUID pre ID korelácie v súvislosti s operáciou

- **DocId** – ID dokumentu vygenerované AppDocs

- **DocInstanceId** – DocInstanceId ID inštancie dokumentu vygenerované AppDocs, ktoré je zamerané na inštanciu operácie v dokumente

- **DocIsEnterpriseProtected** – Boolovská hodnota, ktorá označuje, či je dokument chránený.

- **DocUserId** – ID používateľa z vrstvy overenia MS

- **DocUserIdProvider** – enumerácia predstavujúca poskytovateľa ID používateľa, 0 = neznáme, 1 = LiveId; 2 = OrgId, 3 = SSPI, 4 = ADAL

- **DurationInMs** – čas v milisekundách na ukončenie operácie súboru

- **EndReason** – hodnota enumerácie pre dôvod ukončenia.  Hodnoty: None, Success, Failure, Cancel

- **ErrorCode** – kód chyby pre operáciu súboru

- **Extension** – prvé štyri znaky prípony otvoreného súboru.

- **FileSourceLocation** – hodnota enumerácie pre umiestnenie súboru. Možné hodnoty: None, Local, UncOrMappedNetworkDrive, SkyDrive, App, SharePoint, UnknownServer

- **FILETIME** – čas udalosti

- **FirstBCSClientError_Info** – informácie o kóde chyby v súvislosti s konverziami súborov

- **HttpStatusCode**-http – kód odozvy HTTP pre žiadosť o webovú službu

- **InitalizationReason** – vstupný bod pre otvorenie súboru

- **K2FileIOHresult** – kód Hresult pre ukončenie operácie otvorenia súboru

- **LastBCSClientError_TagId** – posledná chyba klienta BCS (Binary Conversion Service)

- **OfficeWebServiceApiStatusFlag** – príznak stavu pre žiadosť o webovú službu

- **OpEndEventId** – značka, ktorá predstavuje miesto, kde sa operácia v skutočnosti ukončila

- **OpFlags** – príznaky parametrov operácií s dokumentom, ktoré používa vrstva AppDocs.

- **OpSeqNum** – číslo, ktoré predstavuje postupnosť volaní súvisiacich s operáciami súborov vo vrstve AppDocs

- **OpType** – enumerácia typu operácie. Hodnoty: "None", "CreateDocument", "OpenDocument", "CopyDocument", "CloseDocument", "SaveDocument", "OpenVersion", "CloseVersion"

- **PreFetchState** – enumerácia stavu prednačítania šablón pre operácie vytvorenia nových súborov.

- **ProviderApp** – názov balíka aplikácie, z ktorej sa súbor otvoril

- **ScopeInstanceId** – ID inštancie rozsahu, ktoré sa používa na pripojenie kontextu údajov k aktivitám

- **Size** – veľkosť súboru

- **State** – hodnota enumerácie pre stav súboru. Hodnoty: None, Creating, Created, CreateFailed, Opening, Opened, OpenFailed, Copying, Copied, CopyFailed, Closing, Closed, CloseFail

- **TemplateName** – binárny názov šablóny v šablóne dokumentu zo služby šablón, napríklad TF10002009.dotx.

- **UriScheme** – schéma URL adresy

#### <a name="officeandroidauthaceerrors"></a>Office.Android.AuthACEErrors

Táto udalosť používa konto Microsoft (MSA) na určenie toho, ktorý používateľ sa pokúša prihlásiť do aplikácie, a počas toho ktorá telemetria sa spúšťa ako súčasť neúspešného pokusu.  

Táto udalosť pomáha pri analýze rozdelenia chýb prihlásenia MSA, čo pomáha pochopiť dôvody neúspešného ukončenia procesu prihlasovania MSA.

Zhromažďujú sa tieto polia:

- **ExceptionsName** – označuje triedy výnimiek, ktoré sa týkajú značiek výnimiek, ktoré sa vyskytujú počas procesu prihlasovania do konta Microsoft.

- **ExceptionsTag** – označuje, ktoré výnimky v procese prítomné v únii sa vyskytnú pre proces prihlásenia MSA.

- **IDCRLACEErrorCode** – poskytuje kód chyby, ktorá sa vyskytuje počas procesu prihlásenia MSA. Rôzne kódy chýb sú uvedené v: %SRCROOT%\identity\coreapi\public\IdentityData.h

- **IDCRLAuthenticationStatusErrorCode** – označuje kódy chýb pre neplatný stav výsledku overovania z konta Microsoft (MSA).

- **IDCRLUserInteractionMissingError** – označuje, či proces prihlasovania do konta Microsoft (MSA) vyvolaný s príznakom showUI ako false spôsobuje zhodu.


#### <a name="officeandroidbcserrors"></a>Office.Android.BCS.Errors

Telemetria chýb binárnej konverzie pri operáciách tlače a zdieľania vo formáte PDF.  Spoločnosť Microsoft používa túto možnosť na identifikáciu bodov zlyhania počas konverzií BCS v aplikáciách Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **DocumentFileSize** – veľkosť súboru.

- **FileExtension** – prvé štyri znaky prípony súboru.

- **IsFileDirty** – Boolovská hodnota, ktorá označuje, či sa v súbore nenachádzali neuložené zmeny.

- **Location** – enumerácia umiestnenia súboru.  Hodnoty: OneDrive, SharePoint, Dropbox, Others

- **PDFConversionError** – značka, kde sa vyskytne chyba pri konverzii PDF

- **PdfConversionErrorCode** – kód chyby konverzie PDF

- **PdfConversionHRStatus** – kód stavu konverzie PDF

- **PdfConversionResult** – enumerácia výsledku konverzie PDF.  Hodnoty: „Success“, „Failed“, „Cancelled“

- **PdfFileSize** – veľkosť PDF súboru

#### <a name="officeandroidclientsideiap"></a>Office.Android.ClientSideIAP

Telemetria kritických chýb v prípade zlyhania databázy pri prehľadávaní súborov a pridávaní miest.  Spoločnosť Microsoft používa túto možnosť na identifikovanie problémov s poškodením databázy v aplikáciách, ktoré môžu brániť používateľovi v pridávaní miest alebo prehľadávaní cez aplikáciu v rámci aplikácií Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **ClientTransactionId** – identifikátor GUID, ktorý sa odovzdá do DSC na účely konkrétnej žiadosti o uplatnenie nároku.

- **CollectionTime** – čas dokončenia kúpy predplatného

- **CountryCode** – kód krajiny klienta, ktorý sa odošle do DSC na účely žiadosti klienta o uplatnenie nároku

- **GoPremiumEntryPoint** – vstupný bod spustenia nákupu 

- **IsActivateExistingSubscription** – Boolovská hodnota, ktorá označuje, či sa našlo existujúce predplatné, ktoré bolo aktivované.

- **IsErrorRetriable** – Boolovská hodnota, ktorá označuje, či je možné zopakovať pokus o uplatnenie nároku

- **IsPreviousPurchase** – Boolovská hodnota, ktorá označuje, či došlo k aktivácii pri predchádzajúcom zakúpení predplatného

- **IsProvisioningTriggeredByRetry** – Boolovská hodnota, ktorá označuje, či došlo k opakovanému pokusu

- **LanguageCode** – kód jazyka klienta, ktorý sa odošle do DSC na účely žiadosti klienta o uplatnenie nároku

- **ProductIdentifier** – názov jednotky SKU, ktorú sa klient pokúša zakúpiť

- **ProvisioningHttpStatusCode** – kód stavu poskytovania HTTP

- **ProvisioningStatusCode** – kód stavu poskytovania

- **PurchaseOrderId** – identifikátor nákupnej objednávky z obchodu Google/Samsung

- **RedemptionTaskHR** – kód HResult úlohy uplatnenia nároku na predplatné

- **SubscriptionProvisioningSucceeded** – Boolovská hodnota pre úspešný výsledok poskytovania predplatného

- **SubscriptionPurchaseHR** – kód HResult úlohy zakúpenia predplatného

- **SubscriptionType** – enumerácia typu predplatného alebo jednotiek SKU.

- **TCID** – kliknutie na ikonu, ktorým sa spustí proces predplatného

#### <a name="officeandroiddbfailurecause"></a>Office.Android.DBFailureCause

Telemetria kritických chýb v prípade zlyhania databázy pri prehľadávaní súborov a pridávaní miest.  Spoločnosť Microsoft používa túto možnosť na identifikovanie problémov s poškodením databázy v aplikáciách, ktoré môžu brániť používateľovi v pridávaní miest alebo prehľadávaní cez aplikáciu v rámci aplikácií Word, Excel alebo PowerPoint.

Zhromažďujú sa tieto polia:

- **ErrorAt** – hodnota značky: informácie o mieste, kde sa vyskytlo zlyhanie

- **ExceptionErrorMessage** – podrobné chybové hlásenie

#### <a name="officeandroidearlytelemetryexpansionfileserrors"></a>Office.Android.EarlyTelemetry.ExpansionFilesErrors

Rozširujúce súbory súpravy Android Package Kit (APK) pre mobilnú aplikáciu Office sú doplnkové zdrojové súbory, ktoré môžu vývojári aplikácií pre Android publikovať spolu so svojou aplikáciou. Aby bol náš mechanizmus sťahovania rozširujúcich súborov spoľahlivejší, zaznamenávame príčiny chýb, ktoré sa vyskytujú pri sťahovaní rozširujúcich súborov alebo pri čítaní stiahnutých rozširujúcich súborov.

Zhromažďujú sa tieto polia:

- **Data_ClassName** – text zastupujúci názov súboru zdrojového kódu, v ktorom došlo k chybe.

- **Data_ErrorMessage** – text zastupujúci operáciu, ktorá zlyhala.

- **Data_ExceptionMessage** – voliteľné textové pole, ktoré predstavuje príčinu výnimky.

- **Data_ExceptionType** – voliteľné textové pole, ktoré predstavuje názov vygenerovaný zo zdrojového kódu.

- **Data_MethodName** – text zastupujúci názov metódy v zdrojovom kóde, v ktorom došlo k chybe.

#### <a name="officeandroidearlytelemetryextractionerror"></a>Office.Android.EarlyTelemetry.ExtractionError

Na zmenšenie veľkosti aplikácií balíka Office pre Android používame komprimáciu zdrojov v konečnom balíku. V čase spustenia najskôr extrahujeme tieto zdroje pred ich použitím. Niekedy sa vyskytnú neočakávané chyby pri vykonávaní extrakcie, čo vedie k zlyhaniam aplikácie. 

Prostredníctvom tejto udalosti sa zhromažďujú niektoré diagnostické informácie týkajúce sa extrakcie, ako sú napríklad názov extrahovaného zdroja, cesta extrakcie, voľné miesto na disku atď. Tieto údaje sa zhromažďujú len v prípade, že sa vyskytnú chyby pri extrakcii.

Tieto údaje používame na pochopenie príčiny zlyhaní extrakcie a zlepšenie funkčnosti našich aplikácií.

Zhromažďujú sa tieto polia:

- **Data_ArchiveName** – názov extrahovaného zdroja.

- **Data_ArchivePath** – cesta, v ktorej je zdroj dočasne uložený vo vyrovnávacej pamäti.

- **Data_ArchiveSizeKB** – veľkosť extrahovaného zdroja.
 
- **Data_ClassName** – názov súboru v zdrojovom kóde, kde došlo k chybe.

- **Data_ErrorDetail** – text s popisom ďalších podrobností o príčine chyby, ako je napríklad kód chyby atď.

- **Data_ErrorMessage** – text s popisom typu chyby, ktorá sa vyskytla pri extrakcii.

- **Data_ExtractionDestinationPath** – cesta, kam sa zdroj uloží po extrakcii.

- **Data_FreeDiskSpaceMB** – množstvo voľného miesta dostupného v zariadení v megabajtoch. 

- **Data_ItemToExtract** – názov extrahovaného zdroja.

- **Data_MethodName** – názov metódy v zdrojovom kóde, kde došlo k chybe.


#### <a name="officeandroidearlytelemetryregistryerrors"></a>Office.Android.EarlyTelemetry.RegistryErrors

Táto udalosť zachytáva všetky chyby, ktoré sa vyskytli počas prístupu do databázy Registry pre Android. Údaje tejto udalosti nám pomáhajú pochopiť chyby používateľov a zlepšiť fungovanie funkcie databázy Registry.

Zhromažďujú sa tieto polia:

- **App** – Proces aplikácie, ktorý odosiela udalosť.

- **AppVersionLong** – Verzia aplikácie.

- **Data_StackTrace** – Stopa zásobníka chyby.

#### <a name="officeandroidearlytelemetrysharedlibraryloadersearchandloadlibraryerror"></a>Office.Android.EarlyTelemetry.SharedLibraryLoadersearchAndloadLibraryError 

Túto udalosť zaznamenáme v prípade, že sa pri načítavaní zdieľaných knižníc vyskytnú chyby. Chyby pri načítavaní knižníc sa môžu vyskytnúť z dvoch dôvodov: 1) Nainštalovaná aplikácia nie je kompatibilná so zariadením. 2) Knižnica, ktorú sa pokúšame načítať, môže byť poškodená z dôvodu chýb v jej extrahovaní pre nedostatok miesta na disku alebo v pamäti.

Zhromažďujú sa tieto polia:

- **Data_ExceptionMessage** – hlásenie výnimky zobrazené rozhraním Android API System.loadlibrary

- **Data_FreeSpaceInMB** – dostupné voľné miesto v zariadení

- **Data_nickName** – názov knižnice, ktorá sa nedá načítať.

#### <a name="officeandroidintuneintunejavacopyfailedattempts"></a>Office.Android.Intune.IntuneJavaCopyFailedAttempts

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri ukladaní lokálnej kópie chránených cloudových dokumentov služby Intune.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- **Data_FileCreationFailedErrorCode** – kód chyby priradený k procesu

#### <a name="officeandroidintuneintunejavaexceptionadaltokenformam"></a>Office.Android.Intune.IntuneJavaExceptionADALTokenForMAM

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri získavaní tokenu ADAL pre zdroje služby Intune.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- **Data_ErrorCode** – kód chyby priradený k procesu

#### <a name="officeandroidintuneintunejavaexceptionapppolicy"></a>Office.Android.Intune.IntuneJavaExceptionAppPolicy

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s načítaním politík identity pre aktuálny proces.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:
 
- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionapppolicyforcontext"></a>Office.Android.Intune.IntuneJavaExceptionAppPolicyForContext

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s načítaním politík identity pre aktuálnu aktivitu.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:
 
- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionauthenticationcallback"></a>Office.Android.Intune.IntuneJavaExceptionAuthenticationCallback

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s registráciou na spätné volanie overovania spravovaných kont.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptiongetaccountstatesync"></a>Office.Android.Intune.IntuneJavaExceptionGetAccountStateSync

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti so spravovaným kontom.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:
 
- Žiadne

#### <a name="officeandroidintuneintunejavaexceptiongetissavetolocationallowed"></a>Office.Android.Intune.IntuneJavaExceptionGetIsSaveToLocationAllowed

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri načítavaní politiky v súvislosti s ukladaním do lokálneho umiestnenia.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptiongetpolicyforidentity"></a>Office.Android.Intune.IntuneJavaExceptionGetPolicyForIdentity

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s načítaním politík identity.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptiongetprotectioninfofromdescriptor"></a>Office.Android.Intune.IntuneJavaExceptionGetProtectionInfoFromDescriptor

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s informáciami o ochrane.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:
  
- Žiadne

#### <a name="officeandroidintuneintunejavaexceptiongetprotectioninfofrompath"></a>Office.Android.Intune.IntuneJavaExceptionGetProtectionInfoFromPath

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s informáciami o ochrane.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptiongetuipolicyidentity"></a>Office.Android.Intune.IntuneJavaExceptionGetUIPolicyIdentity

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s načítaním politík používateľského rozhrania pre spravované konto.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionisidentitymanaged"></a>Office.Android.Intune.IntuneJavaExceptionIsIdentityManaged

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s identifikovaním, či je konto spravované.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta.

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionnullenrollmentmanager"></a>Office.Android.Intune.IntuneJavaExceptionNullEnrollmentManager

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s registráciou súčastí na spätné volanie.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionprotect"></a>Office.Android.Intune.IntuneJavaExceptionProtect

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s ochranou spravovaného dokumentu.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta.

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionprotectfromdescriptorifrequired"></a>Office.Android.Intune.IntuneJavaExceptionProtectFromDescriptorIfRequired

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s ochranou spravovaného dokumentu.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionregisteraccountsync"></a>Office.Android.Intune.IntuneJavaExceptionRegisterAccountSync

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s registráciou spravovania konta cez Intune.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionsetuipolicyidentitysync"></a>Office.Android.Intune.IntuneJavaExceptionSetUIPolicyIdentitySync

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s nastavením politík pre spravované konto.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionunregisteraccountsync"></a>Office.Android.Intune.IntuneJavaExceptionUnregisterAccountSync

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti so scenármi vzdialeného vymazania pre spravovanie cez Intune.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidintuneintunejavaexceptionupdatetoken"></a>Office.Android.Intune.IntuneJavaExceptionUpdateToken

Telemetria kritických chýb na sledovanie zlyhaní pre jednotlivé rozhrania API služby Intune. Táto telemetria sa zapisuje do denníka v prípade chýb pri volaní rozhraní API služby Intune v súvislosti s tokenom overenia aktualizácie pre spravované konto.  Spoločnosť Microsoft používa tieto údaje na identifikovanie chýb počas nasadenia a po nasadení služby Intune v rámci aplikácie, po prihlásení do aplikácie pomocou pracovného konta

Zhromažďujú sa tieto polia:

- Žiadne

#### <a name="officeandroidlicenseactivationfailure"></a>Office.Android.LicenseActivationFailure

Telemetria kritických chýb na sledovanie zlyhaní pri aktivácii licencií pre kontá Office 365 v aplikáciách Word, Excel alebo PowerPoint.  Spoločnosť Microsoft používa túto možnosť na analýzu zlyhaní aktivácie zakúpenej licencie na Office 365.

Zhromažďujú sa tieto polia:

- **EntryPoint** – enumerácia vstupného bodu spustenia procesu aktivácie licencie

- **HResult** – kód chyby pri zlyhaní

- **IsGallatin** – Boolovská hodnota na kontrolu, či ide o konto Gallatin

- **MessageCode** – enumerácia označujúca bod zlyhania aktivácie

- **PreviousEntryPoint** – enumerácia vstupného bodu spustenia procesu aktivácie licencie

- **StateAfterActivation** – enumerácia označujúca stav licencie aplikácie pred spustením procesu aktivácie

- **StateBeforeActivation** – enumerácia označujúca stav licencie aplikácie pred spustením procesu aktivácie

- **UserAccountType** – enumerácia označujúca, či ide o osobné konto alebo podnikové konto.

#### <a name="officeandroidmsasigninuiprompts"></a>Office.Android.MSASignInUIPrompts

Táto udalosť označuje, že sa používateľovi zobrazila výzva na prihlásenie do osobného konta.  Táto udalosť pomáha porozumieť stavu prihlásenia našich aplikácií a vykonať príslušné akcie, keď si všimneme neočakávané opakované výzvy na prihlásenie. 

Zhromažďujú sa tieto polia:

- **ExternalCacheRefreshError** – kód chyby pokusu o obnovenie tokenu pred zobrazením výzvy na prihlásenie.

- **LastLoginDelta** – čas od posledného úspešného prihlásenia.

- **MSAserverUAID** – ID korelácie s údajmi telemetrie služby.

- **PreviousIdentityState** – označuje stav konta, napríklad uplynutie platnosti relácie. 

- **SignInResultCode** – označuje kód výsledku ukončenia výzvy na prihlásenie.

- **UseCache** – označuje, či sme vynútili výzvu pre používateľa na opätovné zadanie hesla.

- **UserType** – označuje, či ide o existujúce konto alebo nové konto.

- **WasIdentitySignedOut** – označuje, či sa konto nachádzalo v stave odhlásenia.


#### <a name="officeapplelicensingmacdractivationfailures"></a>Office.Apple.Licensing.Mac.DRActivationFailures

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na zaznamenanie zlyhaní aktivácie Digital River (udalosť zaznamená kľúč a produkt, ktorý bol použitý na aktiváciu, a prijatý kód chyby).  Táto udalosť sa používa na zisťovanie a pomoc pri riešení problémov s aktiváciou (problémy s Digital River).

Zhromažďujú sa tieto polia:

- **Data_DigitalRiverID** – ID produktu Digital River, ktoré mapuje na jednotku SKU tohto produktu balíka Office.

- **Data_Error** – Reťazec, ktorý predstavuje kód chyby aktivácie.

- **Data_ProductKey** – Kód Product Key, u ktorého prebehol pokus o aktiváciu.

- **Data_ProductKeyHash** – Zakódovaný aktivovaný kód Product Key.

#### <a name="officeapplelicensingmacgetmachinestatuserrors"></a>Office.Apple.Licensing.Mac.GetMachineStatusErrors

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť zhromažďuje vrátený kód chyby, pričom sa pravidelne kontroluje platnosť licencie na predplatné. Kód chyby môže znamenať nedostupnosť servera, ale aj uplynutie platnosti licencie, obmedzenie počtu prístrojov, neplatné ID hardvéru atď.  Táto udalosť sa používa na monitorovanie stavu licenčnej služby balíka Office, ale aj na skúmanie problémov týkajúcich sa správy prístzrojov a predplatného.

Zhromažďujú sa tieto polia:

- **Data_Error** – Zhromažďujeme informácie o reťazci predstavujúcom kód chyby.

#### <a name="officeextensibilitysandboxodperrornotification"></a>Office.Extensibility.Sandbox.ODPErrorNotification

Sleduje rôzne upozornenia na chyby získané zo sandboxu. Používa sa na zisťovanie scenárov chýb v sandboxe a zvyšovanie produktivity používateľa pomocou opravy.
 
Zhromažďujú sa tieto polia:

- **AppID** – ID aplikácie.

- **AppUrl** – vyčistená URL adresa aplikácie. 

- **Result** -výsledný kód chyby.

#### <a name="officefirstrunapplemaconiolkfirstrunstarted"></a>Office.FirstRun.Apple.MacONIOLKFirstRunStarted

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť nám umožňuje vedieť, že používateľ zadal prvé spustenie. Túto udalosť používame na to, aby sme zistili, či sa prvé spustenie (FRE) začalo úspešne.

Zhromažďujú sa tieto polia:

- **Data_FirstRunCollectionTime** – Časová pečiatka registrujúca čas, v ktorom sa postup začal.

#### <a name="officegraphicsarcexceptions"></a>Office.Graphics.ARCExceptions 

Tieto informácie o nahlásení výnimky sú dôležité na posúdenie celkového stavu zásobníka grafiky, ako aj na identifikáciu častí kódu, v ktorých sa zlyhania vyskytujú s vysokou frekvenciou, aby sa stanovili priority skúmania. Tieto informácie o nahlásení výnimky sú dôležité na posúdenie celkového stavu zásobníka grafiky, ako aj na identifikáciu častí kódu, v ktorých sa zlyhania vyskytujú s vysokou frekvenciou. Pomáhajú inžinierovi určiť, ktoré zlyhania vykresľovania ovplyvňujú väčšinu používateľov, čo nám umožní stanoviť priority nášho skúmania s cieľom vyriešenia problémov, ktoré budú mať najväčší úžitok pre používateľov.

Zhromažďujú sa tieto polia:

  - **Data\_HResult** – chybový kód vrátený zo zlyhania

  - **Data\_TagCount** – počet všetkých zlyhaní, ktoré sa vyskytli

  - **Data\_TagID** – identifikátor zlyhania, ktoré sa vyskytlo

#### <a name="officeoutlookdesktopcalendaracceptcalsharenavigatetosharedfoldererror"></a>Office.Outlook.Desktop.Calendar.AcceptCalShareNavigateToSharedFolder.Error

Táto udalosť zhromažďuje informácie, keď dôjde k zlyhaniu pri navigácii do zdieľaného kalendára. Tieto údaje sa používajú na monitorovanie stavu rozhrania API zdieľania kalendára a interakcie Outlooku so zdieľanými kalendármi.

Zhromažďujú sa tieto polia:

  - **FailedCaseHResult** – chybový kód vrátený zo zlyhania

#### <a name="officeoutlookdesktopedpedpopenstorefailure"></a>Office.Outlook.Desktop.EDP.EDPOpenStoreFailure

Úspešné alebo neúspešné otvorenie e-mailového ukladacieho priestoru chráneného technológiou Enterprise Data Protection na základe výsledku volania rozhrania API systému Windows na získanie kľúča na dešifrovanie ukladacieho priestoru. Táto udalosť sa používa na diagnostikovanie jedného z najčastejších problémov s technológiou Enterprise Data Protection, ktorý môže zabrániť spusteniu Outlooku. Primárnou príčinou zlyhania je interakcia Outlooku s rozhraním API systému Windows, ktoré sa používa na dešifrovanie kľúča ukladacieho priestoru.

Zhromažďujú sa tieto polia:

  - **HVA Activity** **-** s vlastnými údajovými poliami

  - **IsFlightOn** – označuje, či EDPDecryption Flight je povolené

#### <a name="officeoutlookdesktopndbcorruptionresult"></a>Office.Outlook.Desktop.NdbCorruptionResult

Udalosti Office.Outlook.Desktop.NdbCorruptionResult a Office.Outlook.Desktop.NDBCorruptStore.Warning sa zhromažďujú, keď zistíme poškodenie súboru súborov PST/OST používateľa. Keď zistíme poškodenie, spoločnosť Microsoft zhromažďuje formát databázy, miesto zistenia a malé množstvo kontextu o poškodení. Poškodenie súborov OST/PST zabraňuje používateľom v prístupe k e-mailom. Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnej aktivity. Našou snahou je skúmať a diagnostikovať problémy na obmedzenie straty údajov zákazníkov.

Zhromažďujú sa tieto polia:

  - **0** – názov procesu, ktorý nahlásil poškodenie

  - **1** – boolovská hodnota, ktorá označuje, či si používateľ vybral nový súbor alebo nie

  - **2** – počet ďalších procesov, ktoré majú otvorenú databázu

#### <a name="officeoutlookdesktopndbcorruptstorewarning"></a>Office.Outlook.Desktop.NDBCorruptStore.Warning

Udalosti Office.Outlook.Desktop.NdbCorruptionResult a Office.Outlook.Desktop.NDBCorruptStore.Warning sa zhromažďujú, keď zistíme poškodenie súboru súborov PST/OST používateľa. Keď zistíme poškodenie, spoločnosť Microsoft zhromažďuje formát databázy, miesto zistenia a malé množstvo kontextu o poškodení. Poškodenie súborov OST/PST zabraňuje používateľom v prístupe k e-mailom. Tieto údaje sa aktívne monitorujú na zisťovanie abnormálnej aktivity. Našou snahou je skúmať a diagnostikovať problémy na obmedzenie straty údajov zákazníkov.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – čas zhromaždenia

  - **Context** – kontext poškodeného ukladacieho priestoru, kde sa zistilo poškodenie

  - **CreatedWithVersion** – (voliteľné) pole s verziou ukladacieho priestoru

  - **Details** – podrobnosti o zlyhaní

  - **NdbType** – typ ukladacieho priestoru, môže byť 0 = NdbUndefined; 1 = NdbSmall; 2 = NdbLarge; 3 = NdbTardis

  - **ProcessName** – názov procesu spôsobujúceho poškodenie ukladacieho priestoru

  - **PstVersion** – verzia súboru MSPST32.DLL

  - **Version** – verzia formátu súboru ukladacieho priestoru

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptforwardactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ForwardActions.Rule.O16

Táto udalosť zhromažďuje úspech a neúspech akcie Preposlať, Preposlať ako prílohu a Preposlať vo formáte iCalendar pre odpovede na jednoduché, opakované a výnimočné schôdze v zobrazení Outlooku Pošta, Kalendár a Inšpektor. Miera zlyhania akcií Preposlať, Preposlať ako prílohu a Preposlať vo formáte iCalendar sa aktívne monitoruje na zisťovanie anomálií. Abnormálna štatistika označuje zlyhanie schopnosti Outlooku vykonávať základné operácie kalendára. Tieto údaje sa používajú aj na diagnostiku ďalších problémov súvisiacich s kalendárom, ktoré sa môžu zistiť.

Zhromažďujú sa tieto polia:

  - **CountExceptionForward** – počet preposlaných výnimiek schôdzí.

  - **CountExceptionForwardAsiCal** – počet preposlaných výnimiek schôdzí ako iCal.

  - **CountExceptionForwardInSplit** – počet preposlaných výnimiek schôdzí z ponuky Rozdeliť na páse s nástrojmi.

  - **CountExceptionForwardWithAttach** – počet preposlaných výnimiek schôdzí ako príloha.

  - **CountExceptionForward** – počet preposlaných opakovaných schôdzí.

  - **CountExceptionForwardAsiCal** – počet preposlaných opakovaných schôdzí ako iCal.

  - **CountRecurringForwardInSplit** – počet preposlaných opakovaných schôdzí z ponuky Rozdeliť na páse s nástrojmi.

  - **CountExceptionForwardWithAttach** – počet preposlaných opakovaných schôdzí ako príloha.

  - **CountSingleForward** – počet preposlaných jednotlivých schôdzí.

  - **CountSingleForwardAsiCal** – počet preposlaných jednotlivých schôdzí ako iCal.

  - **CountSingleForwardInSplit** – počet preposlaných jednotlivých schôdzí z ponuky Rozdeliť na páse s nástrojmi.

  - **CountSingleForwardWithAttach** – počet preposlaných jednotlivých schôdzí ako príloha.

  - **HResult** – kód chyby.

  - **OlkViewName** – označuje zobrazenie Pošta, Kalendár alebo Inšpektor.

#### <a name="officeoutlookdesktopoutlookcalendarusageerrmeetrcptreplyactionsruleo16"></a>Office.Outlook.Desktop.OutlookCalendarUsageErr.MeetRcpt.ReplyActions.Rule.O16

Táto udalosť zhromažďuje úspech a neúspech akcie Odpovedať, Odpovedať všetkým, Odpovedať okamžitou správou a Odpovedať všetkým okamžitou správou pre odpovede na jednoduché, opakované a výnimočné schôdze v zobrazení Outlooku Pošta, Kalendár a Inšpektor. Miera zlyhania akcií Odpovedať, Odpovedať všetkým, Odpovedať okamžitou správou a Odpovedať všetkým okamžitou správou sa aktívne monitoruje na zisťovanie anomálií. Abnormálna štatistika označuje zlyhanie schopnosti Outlooku vykonávať základné operácie kalendára. Tieto údaje sa používajú aj na diagnostiku ďalších problémov súvisiacich s kalendárom, ktoré sa môžu zistiť.

Zhromažďujú sa tieto polia:

  - **CountExceptionReply** – počet odpovedí na výnimky schôdzí.

  - **CountExceptionReplyAll** – počet odpovedí všetkým na výnimky schôdzí.

  - **CountExceptionReplyAllWithIM** – počet odpovedí všetkým okamžitou správou na výnimky schôdzí.

  - **CountExceptionReplyWithIM** – počet odpovedí okamžitou správou na výnimky schôdzí.

  - **CountRecurringReply** – počet odpovedí na opakované schôdze.

  - **CountRecurringReplyAll** – počet odpovedí všetkým na opakované schôdze.

  - **CountRecurringReplyAllWithIM** – počet odpovedí všetkým okamžitou správou na opakované schôdze.

  - **CountRecurringReplyWithIM** – počet odpovedí okamžitou správou na opakované schôdze.

  - **CountSingleReply** – počet odpovedí na jednotlivé schôdze.

  - **CountSingleReplyAll** – počet odpovedí všetkým na jednotlivé schôdze.

  - **CountSingleReplyAllWithIM** – počet odpovedí všetkým okamžitou správou na jednotlivé schôdze.

  - **CountSingleReplyWithIM** – počet odpovedí okamžitou správou na jednotlivé schôdze.

  - **HResult** – kód chyby.

  - **OlkViewName** – označuje zobrazenie Pošta, Kalendár alebo Inšpektor.

#### <a name="officeoutlookdesktopoutlookprivsdlgsingleuserloadfail"></a>Office.Outlook.Desktop.OutlookPrivsDlgSingleUser.LoadFail

Toto pravidlo zhromažďuje chyby zdieľania kalendára pri pridávaní nového používateľa (typu EX alebo SMTP) z adresára. Tieto údaje sa používajú na diagnostikovanie a riešenie problémov zistených v dialógovom okne Zdieľanie kalendára

Zhromažďujú sa tieto polia:

  - **CountAccountWizardEnd** – koľkokrát sa dialógové okno staršieho sprievodcu ukončilo

  - **CountCreatePIMAccount** – koľkokrát používateľ vytvoril profil PIM

#### <a name="officeoutlookmacmacolkasserts"></a>Office.Outlook.Mac.MacOLKAsserts

Používa sa na identifikovanie problémov s vplyvom na používateľov v Outlooku, ktoré sa môžu prejaviť ako zlyhania alebo znížená funkčnosť. 

Zhromažďujú sa tieto polia:

- **Category** – typ vyhodnotenia.

- **CollectionTime** – čas zhromaždenia vyhodnotenia.


#### <a name="officeoutlookmacmacolkerrors"></a>Office.Outlook.Mac.MacOLKErrors

Používa sa na identifikovanie problémov s vplyvom na používateľov v Outlooku, ktoré sa môžu prejaviť ako zlyhania alebo znížená funkčnosť. 

Zhromažďujú sa tieto polia:

- **Category** – typ chyby.

- **CollectionTime** – čas zhromaždenia chyby.

- **ThreadId** – identifikátor vlákna.


#### <a name="officesystemsystemhealthasserts"></a>Office.System.SystemHealthAsserts

Chyby, ktoré táto udalosť identifikuje, nám pomáhajú porozumieť tomu, kedy sa zhoršuje zákaznícka skúsenosť. Mnohé z týchto vyhodnotení ShipAssert vedú k zlyhaniam a vďaka týmto informáciám je možné mnohé z nich vyriešiť. Zhromažďuje vyhodnotenia ShipAssert z produktu, čo nám pomáha identifikovať chyby.

Zhromažďujú sa tieto polia:

 - **Count** – počet jednotlivých nahlásených vyhodnotení.

  - **EndTime** – čas, v ktorom sa vyskytlo posledné nahlásené vyhodnotenie

  - **ErrorGroup** – Skupinový identifikátor každého vyhodnotenia

  - **FirstTimeStamp** – čas prvého výskytu vyhodnotenia

  - **Trackback** – jedinečný identifikátor konkrétneho vyhodnotenia

#### <a name="officesystemsystemhealtherrorsetwshim"></a>Office.System.SystemHealthErrorsEtwShim

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **Count** – počet jednotlivých chýb

  - **FirstTimeStamp** – čas prvého výskytu chyby

#### <a name="officesystemsystemhealtherrorsulsandasserts"></a>Office.System.SystemHealthErrorsUlsAndAsserts

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **Count** – počet jednotlivých chýb

  - **FirstTimeStamp** – čas prvého výskytu chyby

#### <a name="officesystemsystemhealtherrorsulsworkaround"></a>Office.System.SystemHealthErrorsUlsWorkaround

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **Count** – počet jednotlivých chýb

#### <a name="officesystemsystemhealtherrorswithouttag"></a>Office.System.SystemHealthErrorsWithoutTag

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

Count – počet jednotlivých chýb

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **ErrorCode** – identifikátor chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **ErrorId** – identifikátor chyby

  - **FirstTimeStamp** – čas prvého výskytu chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

#### <a name="officesystemsystemhealtherrorswithtag"></a>Office.System.SystemHealthErrorsWithTag

Táto udalosť sa používa na identifikovanie problémov ovplyvňujúcich zákazníkov v rámci spustenej aplikácie, ktorá sa môžu prejaviť ako zlyhania alebo zhoršená funkčnosť. Zaznamenáva chyby, ktoré sa vyskytujú počas spustenia procesu.

Zhromažďujú sa tieto polia:

  - **Count** – počet jednotlivých chýb

  - **EndTime** – čas výskytu poslednej nahlásenej chyby

  - **ErrorCode** – identifikátor chyby

  - **ErrorGroup** – Skupinový identifikátor každej chyby

  - **ErrorId** – identifikátor chyby

  - **FirstTimeStamp** – čas prvého výskytu chyby

  - **Trackback** – jedinečný identifikátor konkrétnej chyby

#### <a name="renewidentityfailure"></a>RenewIdentityFailure

Zhromažďuje sa, keď sa používateľ pokúsi otvoriť dokument chránený technológiou IRM alebo použiť ochrany technológiou IRM. Obsahuje informácie potrebné na správne preskúmanie a diagnostiku problémov, ktoré sa vyskytujú, keď sa nepodarí obnoviť používateľské certifikáty.

Zhromažďujú sa tieto polia:

- **AppInfo.ClientHierarchy** – hierarchia klienta, ktorá označuje, či sa aplikácia spúšťa v produkčnom prostredí alebo vo vývojárskom prostredí.

- **AppInfo.Name** – názov aplikácie.

- **AppInfo.Version** – verzia aplikácie.

- **Failure.Category** – kategória zlyhania „nespracovaná chyba“

- **Failure.Detail** – podrobné informácie o zlyhaní

- **Failure.Id** – ID zlyhania

- **Failure.Signature** – podpis zlyhania, ktorý je rovnaký ako názov udalosti

- **iKey** – ID servera služby zapisovania do denníka.

- **RMS.HRESULT** – výsledok obnovenia používateľského certifikátu

- **RMS.ScenarioId** – ID scenára definované klientom služby správy prístupových práv.

- **RMS.SDKVersion** – verzia klienta služby správy prístupových práv.

#### <a name="saveerror"></a>save.error

Umožňuje zistiť a vyriešiť situácie, pri ktorých sa vyskytla chyba pri pokuse o uloženie súboru.  Sleduje chyby spôsobené zlyhaniami uloženia súboru vrátane popisného chybového hlásenia, ktoré nám pomôžu pri riešení problému.

Zhromažďujú sa tieto polia: 

- **error** – typ chyby, ktorá sa vyskytla, aby sme mohli zistiť a vyriešiť problémy s konkrétnym typom chyby

- **file_type** – typ súboru, ktorý sa používateľ pokúsil uložiť (napríklad .doc)

- **origin** – označuje umiestnenie pôvodu pokusu o uloženie súboru (napríklad z e-mailu), aby sme mohli zistiť problémy s ukladaním súboru z určitého umiestnenia v aplikácii

- **token_type** – typ tokenu slúžiaci na overenie konta s cieľom uloženia súboru, aby sme mohli zistiť problémy s overovaním týkajúce sa ukladania súboru

#### <a name="wkwebviewerror"></a>wkwebview.error

Táto udalosť nám umožňuje zistiť, či sa vyskytli chyby webového zobrazenia pri písaní alebo čítaní e-mailu, aby sme mohli zabrániť problémom, ktoré by mohli spôsobiť, že aplikácia nemôže vytvoriť alebo čítať e-mail. 

Zhromažďujú sa tieto polia: 

- **description** – popis chyby

- **error_code** – kódy chyby pre WKError

- **function_name** – názov funkcie JavaScript, keď sa vyskytne chyba

- **js_exception_column_number** – číslo stĺpca, v ktorom sa vyskytla výnimka JavaScript 

- **js_exception_line_number** – číslo riadka, v ktorom sa vyskytla výnimka JavaScript

- **js_exception_message** – hlásenie výnimky pri výskyte výnimky JavaScript

- **js_exception_source_url** – URL adresa zdroja, kde sa vyskytla výnimka JavaScript  

- **scenario** – miesto výskytu chyby. Ide o enumeráciu. Možné hodnoty sú old_renderer, react_renderer a composing.

#### <a name="wkwebviewterminate"></a>wkwebview.terminate

Táto udalosť nám umožňuje rozpoznať, keď systém ukončí webové zobrazenie. Tieto údaje nám umožňujú monitorovať chyby, ktoré sa používateľovi vyskytli pri vytváraní alebo čítaní e-mailu. 

Zhromažďujú sa tieto polia: 

- **is_foreground** – či k tejto udalosti došlo, keď bola aplikácia v popredí.

- **scenario** – miesto výskytu chyby, pri vykresľovaní alebo písaní.


## <a name="device-connectivity-and-configuration-data-events"></a>Udalosti údajov v kategórii Pripojiteľnosť a konfigurácia zariadenia

Toto sú podtypy údajov v tejto kategórii:

- [Pripojiteľnosť a konfigurácia zariadenia](#device-connectivity-and-configuration-subtype)


### <a name="device-connectivity-and-configuration-subtype"></a>*Podtyp Pripojiteľnosť a konfigurácia zariadenia*

Stav sieťového pripojenia a nastavenia zariadenia, napríklad pamäte.

#### <a name="applicationdidreceivememorywarning"></a>application.did.receive.memory.warning

Táto udalosť sa odošle, keď zariadenie Apple oznámi, že aplikácia nemá dostatok pamäte. Uvádza, že sme ako súčasť správy pamäte zaviedli do zariadenia problém.

Zhromažďujú sa tieto polia: 

- **current_memory_used** – uvádza množstvo pamäte, ktorú aplikácia využívala v čase, keď sa vyskytol jej nedostatok.

- **current_memory_used_percentage** – uvádza percentuálny podiel pamäte z celkovej veľkosti pamäte, ktorú aplikácia využívala a ktorá bola dostupná v čase, kde sa vyskytol jej nedostatok.

- **currentVC** – uvádza zobrazenie, ktoré sa v súčasnosti zobrazuje, kde sa vyskytol nedostatok pamäte.

- **has_hx** – uvádza, že konto používa našu novú službu synchronizácie, aby sme mohli zistiť problémy spôsobené touto službou

- **is_watch_app_installed** – uvádza, či používateľ momentálne používa hodinky Apple Watch a či sú nainštalované, aby sme dokázali pochopiť nepriaznivý vplyv hodiniek na výkon

- **is_watch_paired** – uvádza, či používateľ momentálne používa hodinky Apple Watch a či sú spárované so zariadením, aby sme dokázali pochopiť nepriaznivý vplyv hodiniek na výkon

- **is_watch_supported_and_active** – uvádza, či používateľ momentálne používa hodinky Apple Watch a či sú aktívne, aby sme dokázali pochopiť nepriaznivý vplyv hodiniek na výkon

- **rn_initialized** – uvádza, či bola funkcia React Native inicializovaná v čase, kde sa vyskytol nedostatok pamäte.

- **running_time** – uvádza čas behu aplikácie v čase, kde sa vyskytol nedostatok pamäte.

#### <a name="conversationmemoryleak"></a>conversation.memory.leak

Umožňuje zistiť situácie, pri ktorých naše zobrazenie e-mailových konverzácií spotrebováva v zariadení väčšie množstvo pamäte, ako sa očakávalo.

Zhromažďujú sa tieto polia:

- Nezhromažďujú sa žiadne polia ani pridané údaje. Zhromažďujú sa len denníky v prípade pretekania pamäte súvisiaceho s vláknom konverzácie.

#### <a name="coredatacorruption"></a>core.data.corruption

Umožňuje zistiť situácie, pri ktorých sa nedarí zobraziť e-maily alebo kalendár, pretože miesto uloženia e-mailov v zariadení bolo poškodené.

Zhromažďujú sa tieto polia:

- **errorSource** – označuje, či sa jedná o akciu uložiť alebo vytvoriť

- **sqlError** – číselný kód chyby, ktorý je uvedený na https://www.sqlite.org/c3ref/c_abort.html

#### <a name="coredatacorruptionuserreset"></a>core.data.corruption.user.reset

Umožňuje zistiť situácie, pri ktorých ste v aplikácii odstránili alebo vynulovali svoje konto a bolo to spôsobené poškodením e-mailových údajov uložených v zariadení.

Zhromažďujú sa tieto polia:

- **errorSource** – určuje, kde sa vyskytlo poškodenie bez ohľadu na to, či to bolo pri ukladaní alebo vytváraní

#### <a name="coredatadiagnostics"></a>core.data.diagnostics 

Umožňuje zistiť a vyriešiť situácie, pri ktorých náš e-mailový ukladací priestor spotrebováva príliš veľa ukladacieho priestoru v zariadení.

Zhromažďujú sa tieto polia:

- **db_size_megabytes** – sleduje veľkosť hlavnej databázy údajov zaokrúhlenú na najbližších 25 MB s maximálnou veľkosťou 500 MB

#### <a name="generalpropertieslog"></a>general.properties.log

Táto udalosť zhromažďuje informácie, ktoré umožňujú kategorizovať a klasifikovať problémy v aplikácii Outlook súvisiace s nastavením zjednodušenia ovládania a zariadenia.  Táto kategorizácia je potrebná na stanovenie priority vplyvu problémov na zákazníkov.

Zhromažďujú sa tieto polia len pre iOS:

- **bold_text** – uvádza, či má zariadenie zapnuté tučné písmo, aby sme mohli zistiť problémy s tučným písmom

- **closed_captioning** – uvádza, či používateľ v zariadení zapol skryté titulky, aby sme mohli zistiť problémy so skrytými titulkami

- **darker_system_colors** – uvádza, či používateľ v zariadení zapol tmavnutie systémových farieb, aby sme mohli zistiť problémy s týmto nastavením

- **gray_scale** – uvádza, či používateľ v zariadení zapol odtiene sivej, aby sme mohli zistiť problémy s týmto nastavením

- **guided_access** – uvádza, či používateľ v zariadení zapol riadený prístup, aby sme mohli zistiť problémy s týmto nastavením

- **invert_colors** – uvádza, či používateľ v zariadení zapol nastavenie inverzie farieb, aby sme mohli zistiť problémy s týmto nastavením

- **mono_audio** – uvádza, či používateľ v zariadení zapol nastavenie pre monofonický zvuk, aby sme mohli zistiť problémy s týmto nastavením

- **reduce_motion** – uvádza, či používateľ v zariadení zapol nastavenie zníženia pohybu, aby sme mohli zistiť problémy s týmto nastavením

- **reduce_transparency** – uvádza, či používateľ v zariadení zapol nastavenie na zníženie priehľadnosti, aby sme mohli zistiť problémy s týmto nastavením

- **speak_screen** – uvádza, či používateľ v zariadení zapol nastavenie pre monofonický zvuk, aby sme mohli zistiť problémy s týmto nastavením

- **speak_selection** – uvádza, či používateľ v zariadení zapol nastavenie Výber reči, aby sme mohli zistiť problémy s týmto nastavením

- **switch_control** – uvádza, či používateľ v zariadení zapol nastavenie Prepnúť ovládanie, aby sme mohli zistiť problémy s týmto nastavením

- **voice_over** – uvádza, či používateľ v zariadení zapol nastavenie funkcie VoiceOver, aby sme mohli zistiť problémy s týmto nastavením

Zhromažďujú sa tieto polia len pre Android:

- **braille** – uvádza, či používateľ v zariadení zapol nastavenie inverzie farieb, aby sme mohli zistiť problémy s týmto nastavením

- **caption** – uvádza, či používateľ v zariadení zapol skryté titulky, aby sme mohli zistiť problémy so skrytými titulkami

- **color_inversion** – uvádza, či používateľ v zariadení zapol nastavenie inverzie farieb, aby sme mohli zistiť problémy s týmto nastavením

- **high_contrast** – uvádza, či používateľ v zariadení zapol nastavenie vysokého kontrastu, aby sme mohli zistiť problémy s týmto nastavením

- **large_text** – uvádza, či má zariadenie zapnuté nastavenie veľkého písma, aby sme mohli zistiť problémy s týmto nastavením

- **oem_preinstall** – uvádza, či bola naša aplikácia v zariadení predinštalovaná (platí len pre zariadenia Samsung)

- **supported_abis** – uvádza, aký druh binárnych rozhraní aplikácie (ABI) podporuje platforma zariadenia, aby sme mohli zistiť problémy s týmto nastavením

- **switch_access** – uvádza, či používateľ v zariadení zapol nastavenie Prepnúť prístup, aby sme mohli zistiť problémy s týmto nastavením

- **talkback** – uvádza, či používateľ v zariadení zapol nastavenie pre službu TalkBack, aby sme mohli zistiť problémy s týmto nastavením

- **theme_color** – vlastná (používateľom vybratá) farba motívu aktuálne používaného aplikáciou

- **webview_kernel_version**: verzia jadra platformy Chromium webového zobrazenia v zariadení, aby sme mohli zistiť problémy s kompatibilitou týkajúce sa verzie webového zobrazenia.

- **webview_package_name**: názov balíka webového zobrazenia v zariadení, aby sme mohli zistiť problémy s kompatibilitou týkajúce sa verzie webového zobrazenia.

- **webview_package_version**: vewrzia balíka webového zobrazenia v zariadení, aby sme mohli zistiť problémy s kompatibilitou týkajúce sa verzie webového zobrazenia.

#### <a name="lowstoragewarning"></a>low.storage.warning

Indikuje, kedy je v zariadení málo pamäte a slúži na monitorovanie toho, či naša aplikácia náhle nezaberá väčšinu ukladacieho priestoru zariadenia z dôvodu vysokého využitia pamäte

Zhromažďujú sa tieto polia: 

- **free_bytes** – množstvo voľného ukladacieho priestoru, ktorý je v zariadení k dispozícii

#### <a name="officeairspaceairspacelocalblocklistdriverupdated"></a>Office.AirSpace.AirSpaceLocalBlocklistDriverUpdated

Používateľ aktualizoval ovládač grafickej karty, ktorý predtým spôsoboval zlyhania balíka Office, a teda sa už nepoužíval na vykresľovanie. Táto udalosť informuje spoločnosť Microsoft o tom, že používatelia, ktorí predtým neboli v optimálnom stave vykresľovania, sa opäť nachádzajú v odporúčanom stave vykresľovania.

Zhromažďujú sa tieto polia:

  - **Data\_BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek.

  - **Data\_DeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek.

  - **Data\_UpdatedDriverVersion** – verzia aktualizovaného ovládača

#### <a name="officeairspaceairspacelocalblocklistinfo"></a>Office.AirSpace.AirSpaceLocalBlocklistInfo

Podrobné informácie o ovládači grafickej karty používateľa, ktorý spôsobil viacnásobné nedávne zlyhania aplikácií balíka Office. Balík Office nebude používať túto grafickú kartu v tejto relácii balíka Office (bude namiesto toho používať softvérové vykresľovanie), kým sa ovládač neaktualizuje. Táto udalosť informuje spoločnosť Microsoft o ovládačoch grafickej karty, ktoré spôsobujú problémy v balíku Office, aby sa mohli identifikovať trendy a aby bolo možné analyzovať vplyv takýchto ovládačov na používateľa. Informuje spoločnosť Microsoft o tom, koľko používateľov sa nachádza v tomto podoptimálnom stave.

Zhromažďujú sa tieto polia:

  - **Data\_AllAppsBlocked** – či sú všetky aplikácie balíka Office na zozname blokovaných položiek

  - **Data\_BlockedDeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek

  - **Data\_BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek

  - **Data\_CrashHistory** – reťazec, ktorý predstavuje históriu ovládača grafickej karty, ktorá spôsobovala zlyhania, na analýzu

  - **Data\_SecsBetweenCrashes** – ako často sa vyskytujú zlyhania ovládača karty

#### <a name="officeairspaceairspacewincompisenabled"></a>Office.AirSpace.AirSpaceWinCompIsEnabled

Táto udalosť zhromažďuje informácie o tom, či sa používa najnovšia platforma vykresľovania na nižšej úrovni založená na Windows Composition.

Keďže najnovšia platforma vykresľovania na nižšej úrovni sa vyvinula a začína sa vydávať zákazníkom, táto udalosť umožňuje spoločnosti Microsoftu zistiť, koľko používateľov má jednotlivé verzie, aby sa zabezpečilo, že platforma bude bez chýb.

Zhromažďujú sa tieto polia:

  - **Data\_WinCompEnabled** –či sa používa riešenie založené na Windows Composition

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorblocklistapp"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorBlocklistApp

Zistilo sa, že grafická karta používateľa spôsobuje dlhé alebo nezvratné nereagovania. Balík Office nebude používať túto grafickú kartu v tejto relácii balíka Office (bude namiesto toho používať softvérové vykresľovanie), kým sa ovládač neaktualizuje. Táto udalosť informuje spoločnosť Microsoft o ovládačoch grafickej karty, ktoré spôsobujú problémy v balíku Office, aby sa mohli identifikovať trendy a aby bolo možné analyzovať vplyv takýchto ovládačov na používateľa. Takisto pomáha pri informovaní o tom, koľko používateľov sa nachádza v tomto podoptimálnom stave.

Zhromažďujú sa tieto polia:

  - **Data\_AppName** – v ktorej aplikácii došlo k nereagovaniam ovládača grafickej karty

#### <a name="officeairspacebackendwin32graphicsdriverhangdetectorregistrywrite"></a>Office.AirSpace.Backend.Win32.GraphicsDriverHangDetectorRegistryWrite

Office zistil, že ovládač grafickej karty používateľa spôsobil nereagovanie, ktoré by sa malo analyzovať pri ďalšom spustení aplikácie balíka Office. Táto udalosť sa používa na určenie, či by bolo pre používateľa vhodnejšie používať iný ovládač alebo adaptér grafickej karty. Pri výskyte vzorov môže spoločnosť Microsoft vykonávať úpravy, aby čo balík Office fungoval čo najplynulejšie.

Zhromažďujú sa tieto polia:

  - **Data\_HangDetected** – či sa zistilo nereagovanie

  - **Data\_InDeviceCall** – v ktorom volaní vykresľovania grafickej karty sa Office nachádzal, keď došlo k nereagovaniu

  - **Data\_Timeout** – ako dlho nereagovanie trvalo, ak sa zariadenie z neho zotavilo

  - **Data\_UnrecoverableCommand** – či sa z nereagovania v tomto príkaze vykresľovania grafickej karty zariadenie zvyčajne zotaví.

#### <a name="officeairspacebackendwin32localblocklistactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistActivity

Podrobné informácie o ovládači grafickej karty používateľa, ktorý spôsobil viacnásobné nedávne zlyhania aplikácií balíka Office. Balík Office nebude používať túto grafickú kartu v tejto relácii balíka Office (bude namiesto toho používať softvérové vykresľovanie), kým sa ovládač neaktualizuje. Táto udalosť informuje spoločnosť Microsoft o ovládačoch grafickej karty, ktoré spôsobujú problémy v balíku Office, aby sa mohli identifikovať trendy a aby bolo možné analyzovať vplyv takýchto ovládačov na používateľa. Informuje spoločnosť Microsoft o tom, koľko používateľov sa nachádza v tomto podoptimálnom stave.

Zhromažďujú sa tieto polia:

  - **Data.AllAppsBlocked** – či sú všetky aplikácie balíka Office na zozname blokovaných položiek

  - **Data.BlockedDeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek

  - **Data.BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek

  - **Data.CrashHistory System.String** – reťazec, ktorý predstavuje históriu ovládača grafickej karty, ktorá spôsobovala zlyhania, na analýzu

  - **Data.SecsBetweenCrashes** – ako často sa vyskytujú zlyhania ovládača karty

#### <a name="officeairspacebackendwin32localblocklistdriverupdatedactivity"></a>Office.AirSpace.Backend.Win32.LocalBlocklistDriverUpdatedActivity

Používateľ aktualizoval ovládač grafickej karty, ktorý predtým spôsoboval zlyhania balíka Office, a teda sa už nepoužíval na vykresľovanie. Táto udalosť informuje spoločnosť Microsoft o tom, že používatelia, ktorí predtým neboli v optimálnom stave vykresľovania, sa opäť nachádzajú v odporúčanom stave vykresľovania.

Zhromažďujú sa tieto polia:

  - **Data\_BlockedDeviceId** – identifikátor zariadenia grafickej karty, ktoré bolo zaradené na zoznam blokovaných položiek

  - **Data\_BlockedDriverVersion** – verzia ovládača, ktorá bola zaradená na zoznam blokovaných položiek

  - **Data\_UpdatedDriverVersion** – verzia aktualizovaného ovládača

#### <a name="officegraphicsspritememcorrupt"></a>Office.Graphics.SpriteMemCorrupt

Táto udalosť nahlasuje chyby zistené v telemetrii účtovania pamäte sprajtov. Je to dôležité na posúdenie stavu telemetrie používania grafickej pamäte. Tieto informácie sú potrebné na overenie správnosti našej telemetrie SpriteMem.

Zhromažďujú sa tieto polia:

  - **Data\_CurrentSpriteMem** – celkové množstvo pamäte, ktoré je aktívne vyhradené na to, aby obsahovalo sprajty (obrázky), ktoré tvoria obsah obrazovky.

  - **Data\_Function** – názov funkcie, ktorá sa pokúša uvoľniť pamäť sprajtov.

  - **Data\_SpriteMemToRemove** – množstvo pamäte, ktoré sa má odstrániť z priradenia pre sprajty.

#### <a name="officepowerpointpptsharednointernetconnectivity"></a>Office.PowerPoint.PPT.Shared.NoInternetConnectivity

Táto udalosť sa zhromažďuje vždy, keď PowerPoint zistí, že internetové pripojenie nie je k dispozícii. Spoločnosť Microsoft používa tieto údaje na získanie diagnostických informácií o internetovom pripojení používateľa, aby mohla porozumieť tomu, ako to ovplyvňuje pripojenie k službám Office.

Zhromažďujú sa tieto polia:

- **Data\_IsNexusDetected:bool** – zobrazuje, či je k dispozícii internetové pripojenie pri volaní služby Nexus (hodnota true) alebo pri volaní rozhrania API všeobecnej webovej služby (hodnota false)

#### <a name="officeserviceabilitymanagerofficesvcmgrprofile"></a>Office.ServiceabilityManager.OfficeSvcMgrProfile

Táto udalosť sa spúšťa pri spustení služby Office Serviceability Manager a je rozhodujúca pre poskytovanie presných prehľadov v súvislosti so stavom nasadenia a zlyhaniami aplikácií a doplnkov v rámci nájomníka zákazníka, a to tak, že nám umožňuje generovať prehľady pre správcov IT, aby mohli bezpečne zavádzať aktualizácie pre podnikové počítače.  

Zhromažďujú sa tieto polia:

- **DeviceIdJoinToken** – používa sa na spojenie údajov telemetrie celkového stavu a stavu nasadenia s inými funkčnými údajmi, ktoré sa zhromažďujú prostredníctvom kanála služieb.

- **TenantAssociationKeyStamped** – boolovský príznak, ktorý sa používa na určenie počtu spravovaných zariadení v ekosystéme balíka Office.
