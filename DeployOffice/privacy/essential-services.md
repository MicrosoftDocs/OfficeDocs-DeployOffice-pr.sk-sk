---
title: Nevyhnutné služby pre Office
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
description: V tomto článku získajú správcovia balíka Office informácie o nevyhnutných službách v balíku Office, ako sú napríklad Klikni a spusti a licenčná služba, a nájdu tu zoznam udalostí a údajových polí pre tieto nevyhnutné služby.
hideEdit: true
ms.openlocfilehash: 25f594865089d35cb46ebfcc9b97d6b048f6298d
ms.sourcegitcommit: ad2bb6e42b2432a2cb9370594cd50f3a14f2fbe3
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/13/2019
ms.locfileid: "38310695"
---
# <a name="essential-services-for-office"></a>Nevyhnutné služby pre Office

> [!IMPORTANT]
> Informácie v tomto článku sa týkajú verzie 1904 alebo novšej verzie nasledujúceho klientskeho softvéru balíka Office nainštalovaného v počítači s Windowsom:
> - Office 365 ProPlus a Office 365 Business
> - Office 365 Personal, Office 365 Home alebo iné verzie balíka Office, ktoré sú súčasťou predplatného služieb Office 365.
> - Project a Visio, ktoré sú súčasťou niektorých plánov predplatného, ako sú napríklad Project Online Professional alebo Visio Online Plan 2.
>
> Informácie platia aj pre verziu 16.28 alebo novšie verzie týchto aplikácií balíka Office pre Mac: Excel, Outlook, OneNote, PowerPoint a Word.

Office pozostáva z klientskych softvérových aplikácií a pripojených funkcií, ktoré sú navrhnuté tak, aby umožňovali efektívnejšiu tvorbu, komunikáciu a spoluprácu. Hoci môžete ovládať mnohé pripojené funkcie, ktoré sú k dispozícii vám alebo vašim používateľom, ak ste správcom vo svojej organizácii, niekoľko služieb je nevyhnutných pre fungovanie balíka Office, a preto sa nedajú vypnúť. Príkladom je licenčná služba, ktorá potvrdzuje, že máte správnu licenciu na používanie služieb balíka Office. Požadované údaje týchto služieb sa zhromažďujú a odosielajú spoločnosti Microsoft bez ohľadu na ďalšie nastavenia týkajúce sa ochrany osobných údajov, ktoré ste nakonfigurovali. Tieto údaje môžete zobraziť pomocou zobrazovača diagnostických údajov.

Ďalšie informácie sa nachádzajú v nasledujúcich témach:

- [Požadované údaje služieb pre Office](required-service-data.md)
- [Používanie nástroja Diagnostic Data Viewer s balíkom Office](https://support.office.com/article/cf761ce9-d805-4c60-a339-4e07f3182855)
- [Pripojené funkcie v Office](connected-experiences.md)

Ak ste správcom v organizácii, možno vás budú zaujímať aj nasledovné témy:

- [Prehľad ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus](overview-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office 365 ProPlus s nastaveniami politiky](manage-privacy-controls.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre Mac pomocou predvolieb](mac-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office v zariadeniach so systémom iOS pomocou predvolieb](ios-privacy-preferences.md)
- [Spravovanie ovládacích prvkov na ochranu osobných údajov pre Office pre zariadenia s Androidom s nastaveniami politiky](android-privacy-controls.md)

## <a name="list-of-essential-services-for-office"></a>Zoznam nevyhnutných služieb pre Office 

Nasledujúca tabuľka obsahuje zoznam nevyhnutných služieb pre Office a ich popis.

| **Služba**  | **Popis**  |
| ------ | ---- |
| [Overovanie](#authentication-events) | Overovanie je služba v rámci viacerých platforiem, ktorá potvrdzuje identitu používateľa pre Office. Vyžaduje sa na to, aby ste sa mohli prihlásiť do balíka Office, aktivovať licenciu na Office a pristupovať k súborom uloženým v cloude a zároveň poskytuje konzistentné používanie v rámci rôznych relácií balíka Office a zariadení.    |
| [Klikni a spusti](#click-to-run-events) | Klikni a spusti je technológia inštalácie, ktorá sa používa na inštaláciu a aktualizáciu balíka Office vo Windowse. Kontroluje dostupnosť nových verzií balíka Office a ak je k dispozícii nová verzia, stiahne a nainštaluje ju.Služba Klikni a spusti rozpoznáva potrebu, sťahuje a inštaluje aktualizácie balíka Office vrátane aktualizácií zabezpečenia.     |
| [Rozšírená konfiguračná služba (ECS)](#enhanced-configuration-service-ecs-events) | Služba ECS umožňuje spoločnosti Microsoft meniť konfiguráciu inštalácií balíka Office bez nutnosti opätovného nasadenia balíka Office. Používa sa na riadenie postupného nasadzovania funkcií alebo aktualizácií, pričom vplyv nasadenia sa monitoruje zo zhromaždených diagnostických údajov. Používa sa aj na zmiernenie problémov funkcie alebo aktualizácie so zabezpečením a výkonom. Okrem toho služba ECS podporuje zmeny konfigurácie týkajúce sa diagnostických údajov na pomoc pri zabezpečovaní zhromažďovania príslušných udalostí. |
| [Licenčná služba](#licensing-events)     | Licenčná služba je cloudová služba, ktorá podporuje aktiváciu balíka Office pre nové inštalácie a uchováva licenciu v zariadeniach po aktivovaní balíka Office. Registruje každé zariadenie používateľa a aktivuje Office, kontroluje stav predplatného na Office a spravuje kódy Product key.    |
|[Microsoft AutoUpdate (MAU)](#microsoft-autoupdate-mau-events)|Microsoft AutoUpdate (MAU) je technológia, ktorá sa používa na aktualizáciu aplikácií od spoločnosti Microsoft vytvorených pre MacOS, ako je napríklad Office. Služba MAU rozpoznáva potrebu, sťahuje a inštaluje aktualizácie aplikácií vrátane aktualizácií zabezpečenia.|
|[OneNote sync](#onenote-sync-events)|OneNote pre Mac podporuje iba poznámkové bloky uložené na internete vo OneDrive alebo v SharePointe Online. OneNote pre Mac neustále synchronizuje všetky poznámky používateľa s OneDrivom alebo SharePointom Online. Vďaka tomu môžu používatelia svoje poznámkové bloky otvárať, zobrazovať a upravovať vo všetkých svojich zariadeniach a budú stále aktuálne.
 [Services Configuration](#services-configuration-events)  | Služba Services Configuration umožňuje vykonávať aktualizácie nastavení konfigurácie balíka Office na povolenie alebo zakázanie klientskych funkcií. Zavolá sa vždy, keď sa spustí aplikácia balíka Office a poskytuje podrobné informácie o iných konfiguráciách a službách balíka Office. Služba Services Configuration tiež riadi, ktoré služby sú určené ako nevyhnutné služby.  |
| [Telemetria](#telemetry-events)  | Služba telemetrie slúži na zhromažďovanie diagnostických údajov z aplikácií balíka Office. Umožňuje zhromažďovať diagnostické údaje vytvorené balíkom Office, a to požadované aj voliteľné diagnostické údaje. Je zodpovedná aj za zhromažďovanie diagnostických údajov služieb v rámci požadovaných údajov služieb pre Office.  |

## <a name="events-and-data-fields-for-essential-services-for-office"></a>Udalosti a údajové polia pre nevyhnutné služby pre Office

V ďalších častiach sú uvedené tieto informácie:

- Zoznam udalostí pre každú nevyhnutnú službu
- Popis každej udalosti
- Zoznam údajových polí v každej udalosti
- Popis každého údajového poľa

Tieto udalosti môžete zobraziť pomocou zobrazovača diagnostických údajov.



## <a name="authentication-events"></a>Udalosti služby overovania

Tieto udalosti diagnostických údajov sa zhromažďujú, keď sa Office pokúša získať token overenia, či už bez zobrazenia výzvy alebo prostredníctvom zobrazenia výzvy.

### <a name="officeidentityfbapromptwin32"></a>Office.Identity.FbaPromptWin32

Zhromažďuje sa, keď sa v balíku Office používateľovi zobrazí výzva na prihlásenie typu Forms-Based-Auth.

Spolu so získaním skrytého tokenu výzvy na overenie umožňujú určiť, či sa používateľ nachádza v stave nefunkčného overenia, čo pre používateľa znamená, že je buď stave offline klienta, alebo v horšom prípade môže nefunkčné overenie znemožniť získanie licencie a mať tak za následok, že klient bude úplne nepoužiteľný.

Výzvy na prihlásenie typu Forms-Based-Auth (FBA) sa používajú pre niektoré lokálne scenáre overovania a zvyčajne sa chceme uistiť, že sa to nedeje, pretože všetky by mali používať prihlásenie typu Modern-Auth z dôvodov chýb zabezpečenia súvisiacich s prihlásením typu FBA.

**Zhromažďujú sa tieto polia:**

  - **AuthScheme** – používaná schéma overovania

  - **DocumentUrlHash** – vyžadovanie šifrovanej URL adresy

  - **EndTag** – značka, v ktorej je formulár FBA skončený

  - **Flags** – zastarané

  - **FlowTag** – značka, v ktorej je formulár FBA začatý

  - **LastError** – vrátený kód chyby

  - **PromptEndTime** – čas skončenia výzvy

  - **PromptStartTime** – čas začatia výzvy

  - **Result** – či bolo overenie úspešné

  - **SessionEndTime** – čas skončenia relácie udalosti

  - **Timeout** – čas uplynutia časového limitu výzvy

### <a name="officeidentitysignoutevent"></a>Office.Identity.SignOutEvent

Zhromažďuje sa, keď sa používateľ odhlási z balíka Office.

Vďaka informácii, že používateľ je odhlásený, je možné klasifikovať ďalšie udalosti, ako sú napríklad výzvy, ako očakávané, aby bolo tieto udalosti možné správne vypočítať v metrike spoľahlivosti/pripravenosti na odoslanie a predchádzať upozorneniam alebo návratu zostáv na predchádzajúcu verziu z dôvodu nesprávneho predpokladu, že používateľovi sa zobrazujú neočakávané výzvy na prihlásenie.

Zhromažďujú sa tieto polia:

  - **FlowEndTime** – čas skončenia akcie odhlásenia

  - **FlowStartTime** – čas začatia akcie odhlásenia

  - **IdentityErrorState** – akýkoľvek stav chyby identity počas odhlásenia

  - **IdentityHashedUniqueId** – šifrovaný identifikátor identity, ktorá sa odhlasuje

  - **IdentityProviderType** – poskytovateľ identity odhlasovanej identity

  - **IdentityUniqueId** – identifikátor identity, ktorá sa odhlasuje

  - **SessionEndTime** – čas skončenia relácie udalosti

  - **SignOutUserAction** – označuje, že používateľ inicioval akciu odhlásenia

### <a name="officeidentitysspipromptwin32"></a>Office.Identity.SspiPromptWin32

Zhromažďuje sa, keď sa v balíku Office používateľovi zobrazí výzva na prihlásenie typu Windows SSPI. Spolu so získaním skrytého tokenu výzvy na overenie umožňujú určiť, či sa používateľ nachádza v stave nefunkčného overenia, čo pre používateľa znamená, že je stave offline klienta. Nefunkčné overenie môže znemožniť získanie licencie a mať tak za následok, že klient bude úplne nepoužiteľný.

Výzvy typu Windows SSPI slúžia na overovanie so službou Exchange (na synchronizáciu pošty), keď prostriedok služby Exchange používateľa nebol nastavený na viacfaktorové overovanie.

Tieto udalosti, ako aj udalosti priestoru názvov Office.MATS, sa používajú na tieto účely:

1\) Identifikácia, či klienti dokážu úspešne získať overovací token alebo či prešli do stavu nefunkčného overenia.

2\) Vyhodnotenie, či zmeny, ku ktorým došlo v klientovi alebo v službách, mali za následok kritické regresie pri postupe alebo spoľahlivosti overovania používateľa

3\) Keď sa vyskytnú zlyhania, tieto signály vysielajú dôležité kódy zlyhania z príslušnej súčasti (kód klienta balíka Office, knižnice overovania alebo služby oprávnenia), ktoré je možné použiť na určenie priority, diagnostikovanie a zmierňovanie

4\) Tieto signály slúžia ako vstupy pre rôzne monitory pripravenosti na odoslanie a monitory stavu, ktoré odosielajú upozornenia, vďaka ktorým naši inžinieri môžu rýchlo reagovať a skrátiť čas na zmiernenie kritických chýb blokujúcich používateľa

Zhromažďujú sa tieto polia:

  - **AllowSavedCreds** – či sú nové poverenia trvalé

  - **AuthScheme** – používaná schéma overovania

  - **CredsSaved** – či sú nové poverenia uložené

  - **DocumentUrlHash** – vyžadovanie šifrovanej URL adresy

  - **EndTag** – značka, v ktorej sa výzva skončila

  - **NewIdentity**\_ErrorState – či je nová identita platná

  - **NewIdentity\_HashedUniqueId** – šifrovaný identifikátor novej identity po skončení výzvy

  - **NewIdentity\_ProviderType** – poskytovateľ novej identity po skončení výzvy

  - **NewIdentity\_UniqueID** – identifikátor novej identity po skončení výzvy

  - **OutStatus** – či je výstup výzvy platný

  - **PromptEndTime** – čas skončenia výzvy

  - **PromptFailedTag** – značka, ktorá signalizuje zlyhanie výzvy SSPI

  - **PromptFlow** – značka, ktorá vyvolala výzvu SSPI

  - **PromptStartTime** – čas začatia výzvy

  - **Proxy** – či sa používa server proxy

  - **ServerHash** – šifrovaná adresa servera

  - **SessionEndTime** – čas skončenia relácie udalosti

  - **Timeout** – čas uplynutia časového limitu výzvy

  - **UiMessage** – hlásenie používateľského rozhrania vo výzve

  - **UserNameHash** – šifrované meno používateľa

### <a name="officeidentitywin32prompt"></a>Office.Identity.Win32Prompt

Zhromažďuje sa, keď sa v balíku Office používateľovi zobrazí výzva na prihlásenie s viacfaktorovým overovaním. Spolu so získaním skrytého tokenu výzvy na overenie umožňujú určiť, či sa používateľ nachádza v stave nefunkčného overenia, čo pre používateľa znamená, že je stave offline klienta. Nefunkčné overenie môže znemožniť získanie licencie a mať tak za následok, že klient bude úplne nepoužiteľný.

Tieto udalosti, ako aj udalosti priestoru názvov Office.MATS, sa používajú na tieto účely:

1\) Identifikácia, či klienti dokážu úspešne získať overovací token alebo či prešli do stavu nefunkčného overenia.

2\) Vyhodnotenie, či zmeny, ku ktorým došlo v klientovi alebo v službách, mali za následok kritické regresie pri postupe alebo spoľahlivosti overovania používateľa

3\) Keď sa vyskytnú zlyhania, tieto signály vysielajú dôležité kódy zlyhania z príslušnej súčasti (kód klienta balíka Office, knižnice overovania alebo služby oprávnenia), ktoré je možné použiť na určenie priority, diagnostikovanie a zmierňovanie

4\) Tieto signály slúžia ako vstupy pre rôzne monitory pripravenosti na odoslanie a monitory stavu, ktoré odosielajú upozornenia, vďaka ktorým naši inžinieri môžu rýchlo reagovať a skrátiť čas na zmiernenie kritických chýb blokujúcich používateľa

Zhromažďujú sa tieto polia:

  - **AdalWAMUsed** – značka, ktorá označuje výsledok, ak sa používa ADAL-atop-WAM

  - **CallTag** – značka, ktorá označuje volajúceho používateľského rozhrania prihlásenia

  - **Context** – kontext prihlásenia pre výzvu

  - **EndTagIdentityProviderRequested** – značka, v ktorej sa vyžaduje poskytovateľ identity

  - **HrdShownTag** – značka, v ktorej sa zobrazuje dialógové okno prihlásenia HRD

  - **IdentityProviderResulted** – typ poskytovateľa identity, ktorý sa požaduje

  - **IdPFlowTag** – značka, ktorá označuje výsledok požiadavky na identitu

  - **LastLoginDelta** – čas od posledného úspešného prihlásenia

  - **NewIdentity\_ErrorState** – či je identita platná po výzve

  - **NewIdentity\_ProviderType** – typ poskytovateľa novej identity po výzve

  - **NewIdentity\_UniqueID** – identifikátor novej identity po výzve

  - **PromptCorrelation** – identifikátor korelácie výzvy na diagnostické účely

  - **PromptEndTime** – čas skončenia výzvy

  - **PromptStartTime** – čas začatia výzvy

  - **SessionEndTime** – čas skončenia relácie udalosti

  - **ShowUIResult** – kód výsledku vrátený z používateľského rozhrania výzvy

  - **StartTag** – značka, v ktorej sa začala výzva Win32

  - **Timeout** – čas uplynutia časového limitu výzvy

  - **WasIdentitySignedOut** – či je používateľ odhlásený

### <a name="officematsactionofficewin32-officematsactionofficewinrt"></a>Office.MATS.actionofficewin32, Office.MATS.actionofficewinrt

Nasledujúci popis sa vzťahuje na udalosti platformy Win32 aj WinRT (názov závisí od platformy.)

Microsoft Auth Telemetry System (MATS) sa zhromažďuje, keď sa Office pokúša získať token overenia, či už bez zobrazenia výzvy alebo prostredníctvom zobrazenia výzvy. Keď pokusy o získanie zlyhajú, zahrnú sa aj informácie o chybe. Tieto udalosti pomáhajú našim používateľom vyhnúť sa prechodu do stavu nefunkčného overenia:

1\) Identifikáciou, či klienti dokážu úspešne získať overovací token alebo či prešli do stavu nefunkčného overenia.

2\) Vyhodnotením, či zmeny, ku ktorým došlo v klientovi alebo v službách, mali za následok kritické regresie pri postupe alebo spoľahlivosti overovania používateľa

3\) Keď sa vyskytnú zlyhania, tieto signály vysielajú dôležité kódy zlyhania z príslušnej súčasti (kód klienta balíka Office, knižnice overovania alebo služby oprávnenia), ktoré je možné použiť na určenie priority, diagnostikovanie a zmierňovanie

4\) Tieto signály slúžia ako vstupy pre rôzne monitory pripravenosti na odoslanie a monitory stavu, ktoré odosielajú upozornenia, vďaka ktorým naši inžinieri môžu rýchlo reagovať a skrátiť čas na zmiernenie kritických chýb

Zhromažďujú sa tieto polia:

  - **Actiontype** – ktorá knižnica overovania sa používa

  - **Appaudience** – či je zostava aplikácie na interné alebo externé používanie

  - **Appforcedprompt** – či aplikácia prepísala vyrovnávaciu pamäť a vynútila zobrazenie výzvy

  - **Appname** – názov aplikácie, ktorá vykonáva overovanie

  - **Appver** – verzia aplikácie, ktorá vykonáva overovanie

  - **Askedforcreds** – či sa v aplikácii zobrazila výzva pre používateľa na zadanie poverení pre túto akciu

  - **Authoutcome** – či bol pokus o overenie úspešný, zlyhal alebo bol zrušený

  - **Blockingprompt** – či sa v aplikácii zobrazila výzva vyžadujúca interakciu používateľa

  - **Correlationid** – identifikátor GUID, ktorý sa použil na spojenie s údajmi služby

  - **Count** – počet udalostí v prípadoch agregácie

  - **Data\_accounttype** – spotrebiteľské konto alebo konto organizácie

  - **Devicenetworkstate** – či bol používateľ online

  - **Deviceprofiletelemetryid** – anonymný identifikátor zariadenia, ktorý sa používa na meranie výkonu zariadenia

  - **Duration** – dĺžka trvania overovania

  - **Endtime** – čas skončenia udalosti overovania

  - **Error** – kód chyby, ak overovanie zlyhalo

  - **Errordescription** – stručný popis chyby

  - **Errorsource** – či chyba pochádzala zo služby, knižnice overovania alebo aplikácie

  - **Identityservice** – či bola vyvolaná služba Microsoft Service Account (MSA) alebo Azure Active Directory (AAD)

  - **Interactiveauthcontainer** – aký typ výzvy sa zobrazil

  - **Issilent** – či sa výzva zobrazila

  - **Microsoft**\_**ADAL**\_**adal**\_**version** – verzia knižnice Azure Active Directory Authentication Library (ADAL)

  - **Microsoft\_ADAL\_api\_error\_code** – kód chyby vyslaný knižnicou overovania pre tento pokus o overenie

  - **Microsoft\_ADAL\_api\_id** – rozhranie API vyvolané pre tento pokus o overenie

  - **Microsoft\_ADAL\_authority** – URL adresa autority služby Azure Active Directory zodpovednej za overovanie používateľa

  - **Microsoft\_ADAL\_authority\_type** – spotrebiteľské/Microsoft Service Agreement (MSA) alebo organizačné/Azure Active Directory (AAD); v súčasnosti vždy AAD

  - **Microsoft\_ADAL\_authority\_validation\_status** – signalizuje, či sa overovanie dokončilo na strane služby

  - **Microsoft\_ADAL\_broker\_app** – signalizuje, či knižnica ADAL použila sprostredkovateľa na overenie

  - **Microsoft\_ADAL\_broker\_app\_used** – uvádza názov sprostredkovateľa (napr. Windows Account Management)

  - **Microsoft\_ADAL\_broker\_version** – uvádza verziu sprostredkovateľa, ak sa použil

  - **Microsoft\_ADAL\_cache\_event\_count** – počet udalostí vyrovnávacej pamäte, ktoré knižnica ADAL vykonala počas načítavania tokenu

  - **Microsoft\_ADAL\_cache\_event\_count\_max** – ak je tento signál agregovaný, max. počet udalostí vyrovnávacej pamäte ktorejkoľvek z agregovaných udalostí.

  - **Microsoft\_ADAL\_cache\_event\_count\_min** – ak je tento signál agregovaný, min. počet udalostí vyrovnávacej pamäte ktorejkoľvek z agregovaných udalostí.

  - **Microsoft\_ADAL\_cache\_event\_count\_sum** – ak je tento signál agregovaný, súčet udalostí vyrovnávacej pamäte všetkých agregovaných udalostí.

  - **Microsoft\_ADAL\_cache\_read\_count** – koľkokrát rozhranie API čítalo z vyrovnávacej pamäte disku. Je prítomné, ak došlo k aspoň jednému čítaniu.

  - **Microsoft\_ADAL\_cache\_read\_error\_count** – koľkokrát zlyhalo čítanie z vyrovnávacej pamäte disku. Je prítomné, ak došlo k aspoň jednému zlyhaniu.

  - **Microsoft\_ADAL\_cache\_read\_last\_error** – kód chyby knižnice ADAL. Je prítomné, ak došlo k aspoň jednému zlyhaniu čítania.

  - **Microsoft\_ADAL\_cache\_read\_last\_system\_error** – kód systémovej chyby. Je prítomné, ak došlo k aspoň jednému zlyhaniu čítania.

  - **Microsoft\_ADAL\_cache\_write\_count** – koľkokrát rozhranie API zapísalo do vyrovnávacej pamäte disku. Je prítomné, ak došlo k aspoň jednému zapisovaniu.

  - **Microsoft\_ADAL\_cache\_write\_error\_count** – koľkokrát zlyhalo zapisovanie do vyrovnávacej pamäte disku. Je prítomné, ak došlo k aspoň jednému zlyhaniu.

  - **Microsoft\_ADAL\_cache\_write\_last\_error** – kód chyby knižnice ADAL. Je prítomné, ak došlo k aspoň jednému zlyhaniu zapisovania.

  - **Microsoft\_ADAL\_cache\_write\_last\_system\_error** – kód systémovej chyby. Je prítomné, ak došlo k aspoň jednému zlyhaniu zapisovania.

  - **Microsoft\_ADAL\_client\_id** – hashovaný identifikátor aplikácie služby AAD

  - **Microsoft\_ADAL\_extended\_expires\_on\_setting** – pravda/nepravda, uvádza, či token má predĺženú životnosť.

  - **Microsoft\_ADAL\_http\_event\_count** – počet HTTP volaní uskutočnených knižnicou ADAL.

  - **Microsoft\_ADAL\_http\_event\_count\_max** – ak je tento signál agregovaný, max. počet HTTP volaní uskutočnených knižnicou ADAL ktorejkoľvek agregovanej udalosti.

  - **Microsoft\_ADAL\_http\_event\_count\_min** – ak je tento signál agregovaný, min. počet HTTP volaní uskutočnených knižnicou ADAL ktorejkoľvek agregovanej udalosti.

  - **Microsoft\_ADAL\_http\_event\_count\_sum** – ak je tento signál agregovaný, súčet HTTP volaní uskutočnených knižnicou ADAL všetkých agregovaných udalostí.

  - **Microsoft\_ADAL\_is\_silent\_ui** – pravda/nepravda, uvádza, či knižnica ADAL zobrazila používateľské rozhranie (výzvu).

  - **Microsoft\_ADAL\_is\_successful** – pravda/nepravda, uvádza, či rozhranie API knižnice ADAL bolo úspešné.

  - **Microsoft\_ADAL\_logging\_pii\_enabled** – pravda/nepravda, uvádza, či je povolený režim úplného zapisovania do denníka knižnice ADAL. Tieto údaje sa zapisujú do denníka len lokálne, neodosielajú sa v telemetrii.

  - **Microsoft\_ADAL\_oauth\_error\_code** – kód chyby protokolu OAuth vrátený službou.

  - **Microsoft\_ADAL\_prompt\_behavior** – prihlasovací alebo žiaden HTTP parameter odovzdaný do služby na určenie, či je možné zobraziť používateľské rozhranie.

  - **Microsoft\_ADAL\_request\_id** – transakčný identifikátor GUID pre požiadavky vyslaný knižnicou do služby.

  - **Microsoft\_ADAL\_response\_code** – kód odpovede HTTP zo služby.

  - **Microsoft\_ADAL\_response\_time** – ako dlho trvalo, kým sa služba vrátila ku knižnici ADAL.

  - **Microsoft\_ADAL\_response\_time\_max** – ak je signál agregovaný, max. čas, kým sa knižnica ADAL vrátila zo svojho rozhrania API, spomedzi ktorejkoľvek z agregovaných udalostí.

  - **Microsoft\_ADAL\_response\_time\_min** – ak je signál agregovaný, min. čas, kým služba odpovedala knižnici ADAL, spomedzi ktorejkoľvek z agregovaných udalostí.

  - **Microsoft\_ADAL\_response\_time\_sum** – ak je signál agregovaný, súčet časov, kým sa knižnica ADAL vrátila zo svojho rozhrania API, spomedzi všetkých agregovaných udalostí.

  - **Microsoft\_ADAL\_rt\_age** – vek tokenu obnovenia

  - **Microsoft\_ADAL\_server\_error\_code** – kód chyby vrátený serverom

  - **Microsoft\_ADAL\_server\_sub\_error\_code** – čiastočný kód chyby vrátený serverom na pomoc pri jednoznačnom určení dôvodu zlyhania požiadavky.

  - **Microsoft\_ADAL\_spe\_ring** – pravda/nepravda, uvádza, či používať používal vnútorný okruh Secure Production Enterprise (len zamestnanci spoločnosti Microsoft).

  - **Microsoft\_ADAL\_start\_time** – čas uskutočnenia volania rozhrania API knižnice ADAL

  - **Microsoft\_ADAL\_stop\_time** – čas vrátenia volania rozhrania API knižnice ADAL

  - **Microsoft\_ADAL\_telemetry\_pii\_enabled** – pravda/nepravda, uvádza, či je povolený režim úplnej telemetrie knižnice ADAL. Názov je nevhodný, keďže sa nevysiela žiadne PII/EUII.

  - **Microsoft\_ADAL\_tenant\_id** – identifikátor GUID identifikujúci nájomníka, ku ktorému patrí overený používateľ.

  - **Microsoft\_ADAL\_token\_acquisition\_from\_context** – opisuje správanie knižnice ADAL na základe tokenov v kontexte overovania.

  - **Microsoft\_ADAL\_token\_type** – token obnovenia (RT) alebo token obnovenia s viacerými zdrojmi (MRRT).

  - **Microsoft\_ADAL\_ui\_event\_count** – počet výziev zobrazených používateľovi. Môžu byť skryté.

  - **Microsoft\_ADAL\_user\_cancel** – pravda/nepravda, či bolo okno používateľského rozhrania zrušené.

  - **Microsoft\_ADAL\_x\_ms\_request\_id** – identifikátor dodatočnej požiadavky poskytnutý službe v hlavičke HTTP knižnicou ADAL.

  - **Platform** – Win32/WinRT/Android/iOS/Mac

  - **Scenarioid** – identifikátor GUID. Viacero udalostí môže patriť do jedného scenára, napríklad scenár môže pridať nové konto, no v rámci daného scenára sa vyskytuje viacero výziev. Tento identifikátor umožňuje výskyt korelácie.

  - **Sessionid** – identifikátor GUID identifikujúci reláciu spustenia

  - **Skdver** – verzia súpravy SDK klienta MATS použitá na vytvorenie týchto údajov

  - **Starttime** – čas zavolania rozhrania Start\*Action MATS API

  - **Tenantid** – identifikátor GUID identifikujúci nájomníka, ku ktorému patrí overený používateľ (v prípadoch bez knižnice ADAL).

  - **Uploadid** – jedinečný identifikátor GUID pre túto udalosť použitý na de-duping

  - **Wamapi** – identifikuje, ktoré rozhranie WAM API sa volá

  - **Wamtelemetrybatch** – v súčasnosti sa nepoužíva. V budúcnosti bude umožňovať súčasti WAM odosielať doplňujúce informácie o udalosti overovania.

## <a name="click-to-run-events"></a>Udalosti služby Klikni a spusti

### <a name="officeclicktorunbootstrapper"></a>Office.ClickToRun.Bootstrapper 

Údaje o inštalácii a inventári balíka Office zhromažďované, keď používateľ spustí súbor setup.exe balíka Office na úpravu nainštalovaných produktov balíka Office. Používa sa na meranie úspechu alebo neúspechu úplnej inštalácie balíka Office spustenej používateľom vrátane predbežných nevyhnutných kontrol.

Zhromažďujú sa tieto polia:

  - **Data\_BootStrapperStateFailure\_ErrorCode** – kód chyby zlyhania

  - **Data\_BootStrapperStateFailure\_ErrorSource** – funkcia, v ktorej došlo k zlyhaniu

  - **Data\_BootStrapperStateFailure\_FailingState** – časť, v ktorej došlo k zlyhaniu v bootstrapper

  - **Data\_BootStrapperStateFailure\_OExceptionType** – typ výnimky zlyhania

  - **Data\_Culture** – jazyková verzia, s ktorou sa spúšťa súbor exe, t. j. en-us

  - **Data\_HashedOLSToken** – sha-256 hash tokenu, ktoré nám služba OLS poskytuje

  - **Data\_Platform** – inštalácia typu x64 alebo x86

  - **Data\_PrereqFailure\_Type** – predbežné zlyhanie, ktoré sa vyskytlo, napr. operačný súbor nie je podporovaný

  - **Data\_ProductReleaseId** – produkt, ktorý inštalujeme, t. j. Office 365 ProPlus

### <a name="officeclicktoruncorruptioncheck"></a>Office.ClickToRun.CorruptionCheck

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti spustil kontrolu poškodenia na zaistenie správnosti binárnych súborov balíka Office. Používa sa na meranie poškodenia binárnych súborov balíka Office a na určenie, ktoré binárne súbory sú poškodené.

Zhromažďujú sa tieto polia:

  - **Data\_Active** – aktuálny manifest streamu, ktorý sa kontroluje na disku

  - **Data\_ActivePackages** – ktoré balíky manifest obsahuje

  - **Data\_ActiveVersion** – verzia manifestu

  - **Data\_AddFileCount** – koľko súborov sa pridáva

  - **Data\_AddFileFiles** – vzorka súborov, ktoré sa pridávajú

  - **Data\_CompressionLevel** – ako sú súbory komprimované

  - **Data\_CorruptionCheckLevel** – ako podrobne sa kontroluje poškodenie, fázy

  - **Data\_CorruptSizeCount** – koľko súborov má poškodenú veľkosť

  - **Data\_CorruptSizeFiles** – vzorka súborov, ktoré majú poškodenú veľkosť

  - **Data\_CorruptVersonCount** – koľko súborov má poškodenú veľkosť

  - **Data\_CorruptVersionFiles** – vzorka súborov, ktoré majú poškodenú verziu

  - **Data\_FileBadDigestCount** – koľko súborov sa nepodarilo otvoriť

  - **Data\_FileBadDigestFiles** – vzorka súborov, ktoré sa nepodarilo otvoriť

  - **Data\_FileNotSignedCount** – koľko súborov nie je podpísaných

  - **Data\_FileNotSignedFiles** – vzorka súborov, ktoré nie sú podpísané

  - **Data\_FileNotTrustedCount** – koľko súborov nie je dôveryhodných

  - **Data\_FileNotTrustedFiles** – vzorka súborov, ktoré nie sú dôveryhodné

  - **Data\_IncompleteFileCount** – koľko súborov je pravdepodobne neúplných

  - **Data\_IncompleteFileFiles** – vzorka súborov, ktoré sú neúplné

  - **Data\_KeepFileCount** – s koľkými súbormi sa nič nerobí

  - **Data\_KeepFileFiles** – vzorka súborov, ktoré sa ponechávajú

  - **Data\_KeepIncompleteFileCount** – koľko súborov sa nemení, aj keď sú neúplné

  - **Data\_KeepIncompleteFileFiles** – vzorka súborov, ktoré sa ponechávajú, hoci sú neúplné

  - **Data\_MismatchSizeCount** – koľko súborov má veľkosť nezodpovedajúcu manifestu

  - **Data\_MismatchSizeFiles** – vzorka súborov, ktoré majú nezodpovedajúcu veľkosť

  - **Data\_MismatchVersionCount** – koľko súborov má verziu nezodpovedajúcu manifestu

  - **Data\_MismatchVersionFiles** – vzorka súborov, ktoré majú nezodpovedajúce verzie

  - **Data\_MissingFileCount** – koľko súborov pravdepodobne chýba

  - **Data\_MissingFileFiles** – vzorka súborov, ktoré chýbajú

  - **Data\_NotToBeStreamedFileCount** – koľko súborov sa nestreamuje

  - **Data\_RemoveFileCount** – koľko súborov sa odstraňuje

  - **Data\_RemoveFileFiles** – vzorka súborov, ktoré sa odstraňujú

  - **Data\_StreamUnitsMismatchCount** – koľko súborov má jednotky nezodpovedajúce manifestu

  - **Data\_StreamUnitsMismatchFiles** – vzorka súborov, ktoré majú stream s nezodpovedajúcimi jednotkami

  - **Data\_TimeElapsed** – dĺžka trvania kontroly poškodenia

  - **Data\_UpdateFileCount** – koľko súborov sa aktualizuje

  - **Data\_UpdateFileFiles** – vzorka súborov, ktoré sa aktualizujú

  - **Data\_Working** – nový manifest, ktorý sa kontroluje

  - **Data\_WorkingVersion** – verzia nového manifestu

### <a name="officeclicktorunmachinemetadata"></a>Office.ClickToRun.MachineMetadata

Údaje o inštalácii a inventári balíka Office, ktoré poskytujú potrebné metaúdaje pre inštaláciu a inventár a ktoré sa používajú na určenie presnej inštalačnej základne.

Zhromažďujú sa tieto polia:

  - **Data\_C2RClientVer** – verzia súboru OfficeClickToRun.exe v zariadení

  - **Data\_OfficeBitness** – bitová verzia nainštalovaného balíka Office, x86 alebo x64

  - **Data\_OfficeVersion** – nainštalovaná verzia balíka Office

  - **Data\_Sku** – nainštalovaná jednotka SKU, t. j. Office 365 ProPlus.en-us

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM Data\_SusClientID – identifikátor aktualizácie balíka Office v zariadení

### <a name="officeclicktorunodt"></a>Office.ClickToRun.ODT

Údaje o inštalácii a inventári balíka Office zhromažďované, keď správca IT spustí súbor setup.exe služby Klikni a spusti nástroja na nasadenie balíka Office na úpravu nainštalovaných produktov balíka Office jeho používateľov. Používa sa na meranie úspechu alebo neúspechu úplnej inštalácie balíka Office spustenej správcom IT vrátane predbežných nevyhnutných kontrol.

Zhromažďujú sa tieto polia:

  - **Data\_BootStrapperStateFailure\_ErrorCode** – kód chyby zlyhania

  - **Data\_BootStrapperStateFailure\_ErrorSource** – funkcia, v ktorej došlo k zlyhaniu

  - **Data\_BootStrapperStateFailure\_FailingState** – časť, v ktorej došlo k zlyhaniu v bootstrapper

  - **Data\_BootStrapperStateFailure\_OExceptionType** – typ výnimky zlyhania

  - **Data\_ConfigurationHost** – hostiteľ, od ktorého pochádza súbor configuration.xml

  - **Data\_ConfigurationId** – identifikátor získaný zo súboru configuration.xml

  - **Data\_ConfigurationSource** – zdroj súboru configuration.xml

  - **Data\_Culture** – jazyková verzia, s ktorou sa spúšťa súbor exe, t. j. en-us

  - **Data\_HashedOLSToken** – sha-256 hash tokenu, ktoré nám služba OLS poskytuje

  - **Data\_MigrateArchRequest** – či sa používateľ migruje z x86 na x64 alebo naopak

  - **Data\_MigrateArchRequestValid** – či je požiadavka na migráciu platná

  - **Data\_Platform** – inštalácia typu x64 alebo x86

  - **Data\_PlatformMigratedFrom** – počiatočná platforma, t. j. x86

  - **Data\_PlatformMigratedTo** – výsledná platforma, t j. x64

  - **Data\_PrereqFailure\_Type** – predbežné zlyhanie, ktoré sa vyskytlo

  - **Data\_ProductReleaseId** – produkt, ktorý inštalujeme, t. j. Office 365 ProPlus

### <a name="officeclicktorunrepomanlogger"></a>Office.ClickToRun.RepomanLogger

Hlási stav nového kanála aktualizácií Klikni a spusti („Repoman“) a či boli aktualizácie balíka Office úspešne stiahnuté a použité.

Zhromažďujú sa tieto polia:

  - **ApplySucceeded** – hodnota true označuje, že kanál úspešne použil aktualizáciu balíka Office. V opačnom prípade má hodnotu false.
  
  - **DownloadSucceeded** – hodnota true označuje, že kanál úspešne stiahol aktualizáciu balíka Office. V opačnom prípade má hodnotu false.

  - **ErrorCode** – kód poslednej chyby, ku ktorej došlo v kanáli Klikni a spusti (Repoman).

  - **ErrorDetails** – ďalšie informácie o chybe, ku ktorej došlo v kanáli Klikni a spusti (Repoman).
 
  - **ErrorMessage** – hlásenie poslednej chyby, ku ktorej došlo v kanáli Klikni a spusti (Repoman).

  - **OpenStreamSessionSucceeded** – hodnota true označuje, že kanál úspešne vytvoril reláciu na streamovanie aktualizácie balíka Office. V opačnom prípade má hodnotu false.

  - **RepomanErrorMessage** – chybové hlásenie prijaté z knižnice repoman.dll.
 

### <a name="officeclicktorunscenarioinstalltaskconfigure"></a>Office.ClickToRun.Scenario.InstallTaskConfigure

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office umiestňuje novostiahnuté súbory. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove** – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID** – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskconfigurelight"></a>Office.ClickToRun.Scenario.InstallTaskConfigurelight

Údaje o inštalácii a inventári balíka Office zhromažďované, keď sa inštalátor balíka Office rozhoduje, ktoré súbory treba stiahnuť. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID** – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskfinalintegrate"></a>Office.ClickToRun.Scenario.InstallTaskFinalintegrate

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office inštaluje licencie a nastavenia databázy Registry. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskfonts"></a>Office.ClickToRun.Scenario.InstallTaskFonts

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office inštaluje písma. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID** – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskinitupdates"></a>Office.ClickToRun.Scenario.InstallTaskInitupdates

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office vytvára nastavenia na správne fungovanie aktualizácií. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID** – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskintegrateinstall"></a>Office.ClickToRun.Scenario.InstallTaskIntegrateinstall

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office vytvára položky databázy Registry pre aplikácie balíka Office používané na meranie úspechu/neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltasklastrun"></a>Office.ClickToRun.Scenario.InstallTaskLastrun

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office dokončuje inštaláciu, pripína skratky a vytvára konečné nastavenia databázy Registry. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID** – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskmigrate"></a>Office.ClickToRun.Scenario.InstallTaskMigrate

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office migruje nastavenia zo starších verzií balíka Office. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskpublishrsod"></a>Office.ClickToRun.Scenario.InstallTaskPublishrsod

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office publikuje virtuálnu databázu Registry pre vrstvu virtualizácie AppV. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskremoveinstallation"></a>Office.ClickToRun.Scenario.InstallTaskRemoveinstallation

Údaje o inštalácii a inventári balíka Office zhromažďované, keď odinštalátor balíka Office odstraňuje časti balíka Office zo zariadenia. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion**  – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskstream"></a>Office.ClickToRun.Scenario.InstallTaskStream

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office sťahuje nové súbory pre balík Office. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion**  – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioinstalltaskuninstallcentennial"></a>Office.ClickToRun.Scenario.InstallTaskUninstallcentennial

Údaje o inštalácii a inventári balíka Office zhromažďované, keď inštalátor balíka Office odinštalováva predchádzajúcu verziu balíka Office nainštalovanú zo Storu. Používa sa na meranie úspechu alebo neúspechu inštalácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenariorepairtaskfinalintegrate"></a>Office.ClickToRun.Scenario.RepairTaskFinalintegrate

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient opravy balíka Office opätovne publikuje súbory .msi a rozšírenia balíka Office. Používa sa na meranie úspechu alebo neúspechu opravy balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion**  – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenariorepairtaskfullrepair"></a>Office.ClickToRun.Scenario.RepairTaskFullrepair

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient opravy balíka sťahuje najnovšiu verziu klienta služby Klikni a spusti na prípravu počítača na odinštalovanie alebo preinštalovanie. Používa sa na meranie úspechu alebo neúspechu opravy balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenariorepairtaskintegraterepair"></a>Office.ClickToRun.Scenario.RepairTaskIntegraterepair

Údaje o inštalácii a inventári balíka Office zhromažďované, keď sa klient opravy balíka Office pokúša opraviť niektoré známe problémové položky databázy Registry. Používa sa na meranie úspechu alebo neúspechu opravy balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenariorepairtaskremoveinstallation"></a>Office.ClickToRun.Scenario.RepairTaskRemoveinstallation

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient opravy balíka Office odstraňuje balík Office zo zariadenia na na prípravu počítača na preinštalovanie alebo opravu. Používa sa na meranie úspechu alebo neúspechu opravy balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioupdatetaskintegrateupdate"></a>Office.ClickToRun.Scenario.UpdateTaskIntegrateupdate 

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti aktualizuje licencie v prípade potreby. Používa sa na meranie úspechu alebo neúspechu aktualizácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioupdatetaskpublishrsod"></a>Office.ClickToRun.Scenario.UpdateTaskPublishrsod

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti aktualizuje nastavenia databázy Registry pre nové binárne súbory. Používa sa na meranie úspechu alebo neúspechu aktualizácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioupdatetaskupdateapply"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateapply

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti ukončí spustené aplikácie v prípade potreby a inštaluje nové stiahnuté súbory. Používa sa na meranie úspechu alebo neúspechu aktualizácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_AvailableVersion** – aká verzia balíka Office je dostupná na aktualizáciu

  - **Data\_CompletedWithoutActionInfo** – dôvod nedokončenia scenára, t. j. aplikácie boli otvorené

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_CorruptionChecksOnly** – či sa len kontroluje poškodenie a nevykonáva aktualizácia

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_HardlinkingException** výnimka, ktorá sa vyskytla pri pokuse o vytvorenie pevných pripojení

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_PackageOperationSuccessful** – pravda, ak sa úspešne dokončila úloha v balíku pre Office

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

  - **Data\_WorkstationLockState** – pravda, ak je počítač pravdepodobne zamknutý

### <a name="officeclicktorunscenarioupdatetaskupdateclientdownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdateclientdownload

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti sťahuje novšiu verziu samého seba. Používa sa na meranie úspechu alebo neúspechu aktualizácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedetection"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedetection

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti kontroluje, či je k dispozícii nová aktualizácia. Používa sa na meranie úspechu alebo neúspechu aktualizácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion** – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_AvailableVersion** – aká verzia balíka Office je dostupná na aktualizáciu

  - **Data\_ComAction** – Int zastupujúci akciu com, ktorá sa vykonáva

  - **Data\_CompletedWithoutActionInfo** – dôvod nedokončenia scenára, t. j. aplikácie boli otvorené

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_PackageUpdateAvailable** – pravda, ak je k dispozícii nové verzia Office

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioupdatetaskupdatedownload"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatedownload

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti sťahuje novú aktualizáciu. Používa sa na meranie úspechu alebo neúspechu aktualizácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion**  – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_AvailableVersion** – aká verzia balíka Office je dostupná na aktualizáciu

  - **Data\_CompletedWithoutActionInfo** – dôvod nedokončenia scenára, t. j. aplikácie boli otvorené

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_CorruptionChecksOnly** – či sa len kontroluje poškodenie a nevykonáva aktualizácia

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_FoundCorruptFiles** – pravda, ak sa našli poškodené súbory

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_PackageOperationSuccessful** – pravda, ak sa úspešne dokončila úloha v balíku pre Office

  - **Data\_PipelineExitCode** – výstupný kód vráteného kanála súboru

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID** – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktorunscenarioupdatetaskupdatefinalize"></a>Office.ClickToRun.Scenario.UpdateTaskUpdatefinalize

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti čistí po aktualizácii a obnovuje predtým otvorené aplikácie. Používa sa na meranie úspechu alebo neúspechu aktualizácie balíka Office.

Zhromažďujú sa tieto polia:

  - **Data\_15\_SourceType** – kde sa nachádza zdroj balíka Office 15, t. j. CDN alebo Local 

  - **Data\_15\_UpdatesEnabled** – či sú aktualizácie balíka Office 15 povolené 

  - **Data\_15\_UpdateVersion**  – na akú verziu balíka Office 15 sa aktualizuje 

  - **Data\_15\_Version** – verzia balíka Office 15 

  - **Data\_16\_SourceType** – kde sa nachádza zdroj balíka Office 16, t. j. CDN alebo Local 

  - **Data\_16\_UpdatesEnabled** – či sú aktualizácie balíka Office 16 povolené 

  - **Data\_16\_UpdateVersion** – na akú verziu balíka Office 16 sa aktualizuje 

  - **Data\_16\_Version** – verzia balíka Office 16 

  - **Data\_AddingFixedProducts** – pridávané produkty 

  - **Data\_AddingProducts** – produkty s požiadavkou na pridanie 

  - **Data\_CompletionState** – či sa úloha dokončila

  - **Data\_ErrorCode** – kód chyby zlyhania 

  - **Data\_ErrorDetails** – dodatočné podrobnosti o chybe 

  - **Data\_ErrorMessage** – chybové hlásenie o problémoch 

  - **Data\_ErrorSource** – miesto výskytu chyby 

  - **Data\_ExceptionType** – výnimka zlyhania 

  - **Data\_IsErrorCodeIgnorable** – či kód chyby zlyhania možno ignorovať 

  - **Data\_IsErrorCodeIgnorableForScenarioHealth** – či kód chyby možno ignorovať 

  - **Data\_NewestPackageVersion** – najnovšia verzia balíka Office v zariadení 

  - **Data\_OldestPackageVersion** – najstaršia verzia balíka Office v zariadení 

  - **Data\_ProductsToAdd** – pridávané produkty balíka Office 

  - **Data\_ProductsToRemove**  – odstraňované produkty balíka Office 

  - **Data\_RemovingFixedProducts** – odstraňované produkty 

  - **Data\_RemovingProducts** – produkty na odstránenie 

  - **Data\_ScenarioInstanceID** – jedinečný identifikátor GUID pre spustený scenár 

  - **Data\_ScenarioName** – ktorý scenár je spustený, t. j. inštalácia 

  - **Data\_ScenarioSubType** – typ spusteného scenára, t. j. odinštalovanie, preinštalovanie 

  - **Data\_SourceType** – zdroj, t. j CDN 

  - **Data\_SqmMachineID**  – jedinečný identifikátor zariadenia, ktorý používa Windows SQM 

  - **Data\_SusClientID**  – identifikátor aktualizácie balíka Office v zariadení 

  - **Data\_TaskState** – stav úlohy, napr. spustená alebo zrušená 

  - **Data\_TotalClientCabSize** – veľkosť kabinetu klienta 

  - **Data\_TriggeringUI** – čo spustilo používateľské rozhranie 

  - **Data\_UpdatesEnabled** – či sú aktualizácie balíka Office povolené 

  - **Data\_Version** – verzia balíka Office 

### <a name="officeclicktoruntransport"></a>Office.ClickToRun.Transport

Táto udalosť nahlasuje akcie sťahovania súborov s cieľom určiť úspešnosť operácie, typ vykonaného sťahovania a diagnostické informácie.


- **BytesFromGroupPeers** – počet bajtov z partnerských zariadení v skupine, iba na sťahovanie pomocou optimalizácie doručovania

- **BytesFromHttp** – počet bajtov z protokolu http, iba na sťahovanie pomocou optimalizácie doručovania

- **BytesFromInternetPeers** – počet bajtov z partnerských zariadení na internete, iba na sťahovanie pomocou optimalizácie doručovania 

- **BytesFromLanPeers** – počet bajtov z partnerských zariadení v sieti LAN, iba na sťahovanie pomocou optimalizácie doručovania 

- **CancelledJobs** – počet zrušených žiadostí v relácii

- **Connected** – či je pripojené k zdroju

- **ErrorCode** – kód poslednej chyby

- **ErrorDetails** – podrobnosti poslednej chyby

- **ErrorMessage** – hlásenie poslednej chyby 

- **ErrorSource** – zdroj poslednej chyby (napr. pripojenie, načítanie súboru alebo načítanie rozsahu)

- **FailedJobs** – počet zlyhaných žiadostí v relácii

- **FileSize** – veľkosť zdroja

- **SourcePathNoFilePath** – zdrojová cesta k zdroju, len zdroj http sa hlási, cesta k lokálnemu súboru alebo cesta UNC sa filtruje

- **SucceededJobs** – počet úspešných žiadostí v relácii

- **TotalJobs** – celkový počet žiadostí v relácii

- **TotalRequestedBytes** – celkový počet bajtov v relácii

- **TotalTransferTime** – celkový čas prenosu v relácii

- **TransferredBytes** – celkový počet prenesených bajtov v relácii

- **TransportType** – druh prenosu (napr. optimalizácia doručovania v pamäti, http, služba inteligentného prenosu na pozadí)



### <a name="officeclicktoruntransportexperimentaltransportpipelinecreatetransport"></a>Office.ClickToRun.Transport.ExperimentalTransport.PipelineCreateTransport

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti vytvára transportný stream na stiahnutie súborov balíka Office. Používa sa na určenie stavu rôznych technológií prenosu (napr. HTTP, BITS, DO), čo je dôležité na správne stiahnutie balíka Office na inštaláciu a aktualizácie.

Zhromažďujú sa tieto polia:

  - **Data\_IsForeGroundStreaming** – či sa streamuje v popredí alebo na pozadí

  - **Data\_IsInstallMode** – 1, ak inštalujú a sťahujú súbory, 0, ak nie

  - **Data\_SourceProtocol –** či sa sťahuje zo siete údajov obsahu (CDN), zariadeni, v ktorom sa inštaluje (local) alebo zo zdroja v lokálnej sieti

  - **Data\_Status** – Úspech alebo zlyhanie 

### <a name="officeclicktorunupdatestatus"></a>Office.ClickToRun.UpdateStatus

Údaje o inštalácii a inventári balíka Office zhromažďované, keď klient služby Klikni a spusti dokončuje stav inštalácie.

Zhromažďujú sa tieto polia:

  - **Data\_build** – aktuálne nainštalovaná verzia balíka Office

  - **Data\_channel** –, kanál, v ktorom sa používateľ nachádza

  - **Data\_errorCode** – celé číslo určujúce typ chyby, ktorá sa vyskytla, ak sa vyskytla

  - **Data\_errorMessage** – reťazec s popisom chyby, ktorá sa vyskytla, ak sa vyskytla

  - **Data\_status** – krátky stav, čo sa stalo počas aktualizácie, ako napríklad úspešné alebo stiahnuté

  - **Data\_targetBuild** – verzia balíka Office, na ktorú sa aktualizuje


### <a name="officeclicktorununiversalbootstrapperapplication"></a>Office.ClickToRun.UniversalBootstrapper.Application

Táto udalosť nahlasuje výsledok pokusu o end-to-end inštaláciu

 - **ErrorCode** – celočíselná hodnota s nespracovanou výnimkou

 - **ErrorDetails** – reťazec, ktorý popisuje umiestnenie, v ktorom sa vyskytla nespracovaná výnimka (funkcia, súbor, číslo riadka, ďalšie parametre určené pri výskyte výnimky)

 - **ErrorMessage** – reťazec definovaný v bode, v ktorom sa vyskytla nespracovaná výnimka a ktorý popisuje povahu zlyhania

 - **ErrorType** – reťazec popisujúci kategóriu nespracovanej výnimky

 - **ExitCode** – celočíselná hodnota súvisiaca s výsledkom spustenia súčasti Bootstrapper, ktorá signalizuje úspech alebo špecifické typy zlyhania

### <a name="officeclicktorununiversalbootstrappercalculateparameters"></a>Office.ClickToRun.UniversalBootstrapper.CalculateParameters

Táto udalosť nahlasuje akciu, ktorá vyvodzuje záver zo vstupu získaného pomocou udalosti CollectParameters

- **BitField** – celočíselná hodnota argumentu BitField, ktorá signalizuje, či sa vyžaduje výslovný kanál inštalácie/aktualizácie (mesačný, Insiders Slow, Insiders Fast, polročný, polročný pre vybraných používateľov)

- **ChannelID** – celé číslo predstavujúce hodnotu enumerácie vybratého kanála aktualizácie/inštalácie (mesačný, Insiders Slow, Insiders Fast, polročný, polročný pre vybraných používateľov, neplatný)

- **CMDMode** – priateľský reťazec zodpovedajúci tomu, ktorý prepínač celkového režimu sa zistil v argumentoch cmd odovzdaných do súboru exe.

- **C2RClientUICulture** – kultúra klienta C2R na inštaláciu

- **ErrorCode** – celočíselná hodnota spojená s nespracovanou výnimkou

- **ErrorDetails** – reťazec, ktorý popisuje umiestnenie, v ktorom sa vyskytla nespracovaná výnimka (funkcia, súbor, číslo riadka, ďalšie parametre určené pri výskyte výnimky)

- **ErrorMessage** – reťazec definovaný v bode, v ktorom sa vyskytla nespracovaná výnimka a ktorý popisuje povahu zlyhania

- **ErrorType** – reťazec popisujúci kategóriu nespracovanej výnimky

- **ExcludedApps** – reťazec uvádzajúci názvy jednotlivých aplikácií balíka Office požadovaných na vylúčenie z nainštalovaných balíkov Office

- **InstalledCabVersion** – verzia „16.0.xxxxx.yyyyy“ už nainštalovaného klienta Office C2R

- **InstalledProductVersion** – verzia „16.0.xxxxx.yyyyy“ už nainštalovaného produktu Office C2R

- **IsC2RServiceRunning** – boolovský príznak, ktorý označuje, či je služba lokálneho počítača moderného klienta C2R spustená v zariadení

- **IsElevatedFlagSet** – boolovský príznak označujúca, či sa súčasť Bootstrapper už pokúsila získať úroveň správcu

- **IsFireFlyInstalled** – boolovský príznak označujúci, či je klient Office 2013 RTM C2R momentálne nainštalovaný

- **IsFireflyServiceRunning** – boolovský príznak, ktorý označuje, či je služba lokálneho počítača klienta 2013 RTM C2R spustená v zariadení

- **IsOfficeInstalled** – boolovský príznak označujúci, či je moderný klient balíka Office už nainštalovaný

- **OfficeCultures** – serializovaný zoznam kultúr balíka Office, ktoré sa majú nainštalovať

- **OfficeSourceType** – priateľský reťazec súvisiaci s hodnotou enumerácie zdroja inštalácie (CDN, HTTP, UNC, CMBITS, DVD, LOCAL)

- **Origin** – reťazcová hodnota, ktorá uvádza, ktorý z podporovaných pôvodov (Portoriko [PR], Singapur [SG], Dublin [DB]) sa má použiť na úvodné streamovanie inštalácie

- **PlatformFromLink** – reťazec označujúci požadovaný bitovú verziu (x86|x 64|predvolená) balíka Office požadovanú zo služby C2R Setup

- **PlatformOfExistingInstallation** – reťazec, ktorý označuje, či už bol v zariadení nainštalovaný balík x86 alebo x64

- **PlatformToInstall** – reťazec označujúci konečné rozhodnutie o tom, či sa má nainštalovať balík Office x86 alebo x64. Možnosti sú: autorun, configure, consumer, download, help, packager

- **PRID** – reťazcová hodnota predstavujúca požadovaný identifikátor vydania produktu v scenári spotrebiteľskej inštalácie (napríklad „O365ProPlusRetail“)

- **ProductsToAdd** – sarializovaný reťazec, ktorý klientovi C2R udáva pokyn, ktoré kombinácie produktu a kultúry má nainštalovať

- **ProductsToRemove** – sarializovaný reťazec, ktorý klientovi C2R udáva pokyn, ktoré kombinácie produktu a kultúry má odinštalovať

- **SharedComputerLicensing** – boolovská hodnota signalizujúca, či správca IT požadoval, aby inštalačný program povolil funkciu „SharedComputerLicensing“

- **ShouldActivate** – boolovská hodnota signalizujúca, či správca IT vo svojom súbore configuration.xml vyžiadal pokus a automatickú aktiváciu licencie

- **VersionToInstall** – reťazcová hodnota verzie balíka Office „16.0.xxxxx.yyyy“, ktorá sa inštaluje
 

### <a name="officeclicktorununiversalbootstrappercollectembeddedsignature"></a>Office.ClickToRun.UniversalBootstrapper.CollectEmbeddedSignature

Táto udalosť nahlasuje akciu, ktorá číta označený vstup z vloženého podpisu súboru exe.  Ide o neoverený koncept, ktorý predchádzajúca iterácia súboru setup.exe neimplementovala a na ktorý sa spoliehame pri prenose voľby používateľa týkajúcej sa produktu/jazyka/bitovej verzie z webovej stránky do procesu v rámci súboru setup.exe.
 
- **ErrorCode** – celé číslo súvisiace s nespracovanou výnimkou

- **ErrorDetails** – reťazec, ktorý popisuje umiestnenie, v ktorom sa vyskytla nespracovaná výnimka (funkcia, súbor, číslo riadka, ďalšie parametre určené pri výskyte výnimky)

- **ErrorMessage** – reťazec definovaný v bode, v ktorom sa vyskytla nespracovaná výnimka a ktorý popisuje povahu zlyhania

- **ErrorType** – reťazec popisujúci kategóriu nespracovanej výnimky

### <a name="officeclicktorununiversalbootstrappercollectparameters"></a>Office.ClickToRun.UniversalBootstrapper.CollectParameters

Táto udalosť nahlasuje parametre použité na inštaláciu balíka Office

- **BitField** – celočíselná hodnota argumentu BitField, ktorá signalizuje, či sa vyžaduje výslovný kanál inštalácie/aktualizácie (mesačný, Insiders Slow, Insiders Fast, polročný, polročný pre vybraných používateľov)

- **ChannelID** – celé číslo predstavujúce hodnotu enumerácie vybratého kanála aktualizácie/inštalácie (mesačný, Insiders Slow, Insiders Fast, polročný, polročný pre vybraných používateľov, neplatný)

- **CMDMode** – priateľský reťazec zodpovedajúci tomu, ktorý prepínač celkového režimu sa zistil v argumentoch cmd odovzdaných do súboru exe. Možnosti sú: autorun, configure, consumer, download, help, packager

- **C2RClientUICulture** – kultúra klienta C2R na inštaláciu

- **ErrorCode** – celočíselná hodnota spojená s nespracovanou výnimkou

- **ErrorDetails** – reťazec, ktorý popisuje umiestnenie, v ktorom sa vyskytla nespracovaná výnimka (funkcia, súbor, číslo riadka, ďalšie parametre určené pri výskyte výnimky)

- **ErrorMessage** – reťazec definovaný v bode, v ktorom sa vyskytla nespracovaná výnimka a ktorý popisuje povahu zlyhania

- **ErrorType** – reťazec popisujúci kategóriu nespracovanej výnimky

- **ExcludedApps** – reťazec uvádzajúci názvy jednotlivých aplikácií balíka Office požadovaných na vylúčenie z nainštalovaných balíkov Office

- **InstalledCabVersion** – verzia „16.0.xxxxx.yyyyy“ už nainštalovaného klienta Office C2R

- **InstalledProductVersion** – verzia „16.0.xxxxx.yyyyy“ už nainštalovaného produktu Office C2R

- **IsC2RServiceRunning** – boolovský príznak, ktorý označuje, či je služba lokálneho počítača moderného klienta C2R spustená v zariadení

- **IsElevatedFlagSet** – boolovský príznak označujúca, či sa súčasť Bootstrapper už pokúsila získať úroveň správcu

- **IsFireFlyInstalled** – boolovský príznak označujúci, či je klient Office 2013 RTM C2R momentálne nainštalovaný

- **IsFireflyServiceRunning** – boolovský príznak, ktorý označuje, či je služba lokálneho počítača klienta 2013 RTM C2R spustená v zariadení

- **IsOfficeInstalled** – boolovský príznak označujúci, či je moderný klient balíka Office už nainštalovaný

- **OfficeCultures** – serializovaný zoznam kultúr balíka Office, ktoré sa majú nainštalovať

- **OfficeSourceType** – priateľský reťazec súvisiaci s hodnotou enumerácie zdroja inštalácie (CDN, HTTP, UNC, CMBITS, DVD, LOCAL)

- **Origin** – reťazcová hodnota, ktorá uvádza, ktorý z podporovaných pôvodov (Portoriko [PR], Singapur [SG], Dublin [DB]) sa má použiť na úvodné streamovanie inštalácie

- **PlatformFromLink** – reťazec označujúci požadovaný bitovú verziu (x86|x 64|predvolená) balíka Office požadovanú zo služby C2R Setup

- **PlatformOfExistingInstallation** – reťazec, ktorý označuje, či už bol v zariadení nainštalovaný balík x86 alebo x64

- **PlatformToInstall** – reťazec označujúci konečné rozhodnutie o tom, či sa má nainštalovať balík Office x86 alebo x64.

- **ProductsToRemove** – sarializovaný reťazec, ktorý klientovi C2R udáva pokyn, ktoré kombinácie produktu a kultúry má odinštalovať

- **PRID** – reťazcová hodnota predstavujúca požadovaný identifikátor vydania produktu v scenári spotrebiteľskej inštalácie (napríklad „O365ProPlusRetail“)

- **ProductsToAdd** – sarializovaný reťazec, ktorý klientovi C2R udáva pokyn, ktoré kombinácie produktu a kultúry má nainštalovať

- **SharedComputerLicensing** – boolovská hodnota signalizujúca, či správca IT požadoval, aby inštalačný program povolil funkciu „SharedComputerLicensing“

- **ShouldActivate** – boolovská hodnota signalizujúca, či správca IT vo svojom súbore configuration.xml vyžiadal pokus a automatickú aktiváciu licencie

- **VersionToInstall** – reťazcová hodnota verzie balíka Office „16.0.xxxxx.yyyy“, ktorá sa inštaluje

### <a name="officeclicktorununiversalbootstrapperexecute"></a>Office.ClickToRun.UniversalBootstrapper.Execute

Táto udalosť nahlasuje prijaté akcie s vplyvom na zariadenie, ako sú určené na základe vyvodených údajov z udalosti CalculateParameters

- **AvailableClientVersionText** – reťazcová hodnota verzie „16.0. xxxxx.yyyy“ klienta C2R, ktorá sa nachádza vo formáte XML popisovača verzie a ktorá sa používa na určenie, či má byť aktuálne nainštalovaný klient C2R aktualizovaný

- **CleanFireflyAction** – má hodnotu „true“, ak je počas tejto inštalácie naplánované spustenie úlohy CleanFireFlyAction

- **CleanO15Action** – má hodnotu „true“, ak je počas tejto inštalácie naplánované spustenie úlohy CleanO15Action

- **CMDMode** – priateľský reťazec zodpovedajúci tomu, ktorý prepínač celkového režimu sa zistil v argumentoch cmd odovzdaných do súboru exe. Možnosti sú: autorun, configure, consumer, download, help, packager

- **DeliveryMechanism** – Identifikátor GUID „FFNRoot“ extrahovaný z formátu XML deskriptora verzie (s pečiatkou RDX), ktorý uvádza, z ktorého publika/kanála zdroj zostavy pochádzal

- **DownloadC2RClientAction** – má hodnotu „true“, ak je počas tejto inštalácie naplánované spustenie úlohy DownloadC2RClientAction

- **ErrorCode** – celočíselná hodnota spojená s nespracovanou výnimkou

- **ErrorDetails** – reťazec, ktorý popisuje umiestnenie, v ktorom sa vyskytla nespracovaná výnimka (funkcia, súbor, číslo riadka, ďalšie parametre určené pri výskyte výnimky)

- **ErrorMessage** – reťazec definovaný v bode, v ktorom sa vyskytla nespracovaná výnimka a ktorý popisuje povahu zlyhania

- **ErrorType** – reťazec popisujúci kategóriu nespracovanej výnimky

- **ExitCode** – celočíselná hodnota súvisiaca s výsledkom spustenia fázy Execute súčasti Bootstrapper, ktorá signalizuje úspech alebo špecifické typy zlyhania

- **LaunchAction** – má hodnotu „true“, ak je počas tejto inštalácie naplánované spustenie úlohy LaunchAction

- **LaunchUpdateAction** – má hodnotu „true“, ak je počas tejto inštalácie naplánované spustenie úlohy LaunchUpdateAction

- **PreReqResult** – celočíselná hodnota enumerácie výsledku, keď sa vykonali kontroly PreReq (úspech/neúspech/opätovné spustenie)

- **UnexpectedAction** – má hodnotu „true“, ak je počas tejto inštalácie naplánované spustenie úlohy UnexpectedAction (prípad chyby)

- **VersionToInstall** – reťazcová hodnota verzie balíka Office „16.0.xxxxx.yyyy“, ktorá sa inštaluje


## <a name="enhanced-configuration-service-ecs-events"></a>Udalosti služby Enhanced Configuration Service (ECS)

### <a name="officeexperimentationfeaturequerybatched"></a>Office.Experimentation.FeatureQueryBatched

Zhromažďuje informácie o bránach funkcií alebo bránach zmien dotazovaných spusteným kódom.

Zhromažďujú sa tieto polia:

  - **Count** – počet dotazovaných brán funkcií v tejto dávkovej udalosti

  - **Features** – informácie o dotazovanej bráne.

  - **Sequence** – poradie, v ktorom bola brána funkcií dotazovaná

### <a name="officeexperimentationflightnumberline"></a>Office.Experimentation.FlightNumberLine

Zhromažďuje zoznam konfigurácií prijatých klientom zo služby ECS

Zhromažďujú sa tieto polia:

  - **ECSConfigs** – zoznam konfigurácií služby ECS oddelený čiarkami

  - **LockType** – typ zámku FlightManagera

  - **TasFlightingVersion** – číslo verzie

  - **TimeToLock** – čas medzi iniciovaním libletu a zámkom FlightManagera

  - **UnmergedConfigs** – zoznam nezlúčených konfigurácií

### <a name="officeexperimentationtriggeranalysis"></a>Office.Experimentation.TriggerAnalysis

Táto udalosť umožňuje obmedziť analýzu používania produktov a metrík výkonu (napríklad zlyhaní, zablokovaní a podobne) na podmnožinu používateľov alebo zariadení oprávnených na používanie danej funkcie, čím prispieva k zabezpečeniu správneho fungovania produktu.

Zhromažďujú sa tieto polia:

  - **FeatureGate** – identifikuje množinu funkcií, na ktoré sa vzťahuje analýza aktivačných udalostí.

## <a name="licensing-events"></a>Udalosti licenčnej služby

### <a name="officelicensingaccepteulaforcurrentlicense"></a>Office.Licensing.AcceptEulaForCurrentLicense 

Táto udalosť sa zhromažďuje, keď používateľ získa licenciu a prijme zmluvu EULA pre aktuálnu licenciu.

Používa sa na určenie, či sa používateľ nachádza v dobrom stave alebo nie, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **ACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu

  - **DwEulaId** – číselný identifikátor typu licenčnej zmluvy koncového používateľa, ktorú používateľ práve prijal

### <a name="officelicensingactivation"></a>Office.Licensing.Activation 

Po nastavení licencie v počítači sa vykoná pokus o jej aktivovanie zavolaním služby AVS. Táto udalosť nahlasuje výsledok aktivačného volania.

Je to dôležité na zistenie, koľko používateľov má problémy s aktiváciou. Existuje zisťovanie anomálie na rozpoznávanie akejkoľvek regresie. Je to mimoriadne dôležité, pretože máme externú závislosť od služby AVS a tento signál signalizuje, či stav naši externých partnerov v poriadku. Používa sa aj na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **ACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu

  - **ReferralData** – identifikátor výrobcu OEM, ktorý nainštaloval balík Office do počítača

### <a name="officelicensingactivationwizard"></a>Office.Licensing.ActivationWizard 

Ak sa licenciu z nejakého dôvodu nepodarilo aktivovať automaticky, používateľovi sa zobrazí sprievodca aktiváciou. Táto udalosť hlási, že používateľovi sa zobrazuje sprievodca. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officelicensingenforcesigninqualified"></a>Office.Licensing.EnforceSignInQualified 

Toto je signál, z ktorého sa dozvieme, či experiment, pomocou ktorého sa snažíme používateľovi vynútiť prihlásenie v rámci licencovania, je úspešný. Je to dôležité na zistenie úspechu alebo neúspechu experimentu, ktorý núti používateľov prihlásiť sa, čo je povinný krok pre moderný postup licencovania. Neúspešné prihlásenie bude mať za následok, že používatelia nebudú môcť používať aplikáciu.

Zhromažďujú sa tieto polia:

  - **Qualified** – určuje, či používateľ je oprávnený na vynútenie prihlásenia

### <a name="officelicensingexpirationdialogshown"></a>Office.Licensing.ExpirationDialogShown

Táto udalosť sa zhromažďuje, keď sa používateľovi zobrazí dialógové okno o uplynutí platnosti licencie. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **LicNotificationState** – enumerátor, ktorý nás informuje, aký druh oznámenia sa používateľovi zobrazuje

### <a name="officelicensingfullvalidation"></a>Office.Licensing.FullValidation 

Táto udalosť sa zhromažďuje v každej relácii, ktorá nahlasuje licenčný stav zariadenia, a hlási chyby, ktoré sa používateľovi zobrazujú a pre ktoré nemôže používať aplikáciu. Táto udalosť označuje, či je stav zariadenia používateľa v poriadku alebo nie. Pre túto udalosť je vytvorené zisťovanie anomálie na rozpoznávanie, či regresia spôsobuje nevhodné správanie používateľa. Je to dôležité aj pri zisťovaní problémov používateľa a na monitorovanie stavu systému.

Zhromažďujú sa tieto polia:

  - **ACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu 

  - **IsSessionLicensing** – či je v súčasnosti spustený režim aktivácie v zdieľanom počítači alebo nie 

  - **LicenseCategory** – kategória licencie na Office, ktorú používateľ používa 

  - **Licenses** – zoznam názvov všetkých licencií na Office, ktoré sa nachádzajú v zariadení 

  - **LicenseStatuses** – stav všetkých licencií na Office, ktoré sa nachádzajú v zariadení 

### <a name="officelicensinggetentitlement"></a>Office.Licensing.GetEntitlement 

Túto udalosť zhromažďujeme, keď používateľ nastavuje zariadenie a volá sa licenčná služba, aby sa zistilo, či prihlásený používateľ má nárok na Office alebo nie. Táto udalosť nahlasuje výsledok tohto volania. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officelicensingheartbeat"></a>Office.Licensing.Heartbeat 

V každej relácii kontrolujeme, či od posledného obnovenia licencie uplynulo 72 hodín, a pokúšame sa predĺžiť platnosť aktuálnej licencie. Táto udalosť nahlasuje úspech alebo neúspech volania, ktoré uskutočňujeme preto, aby sa zaručilo, že môžeme predĺžiť platnosť licencie a ponechať inštaláciu balíka Office používateľa funkčnú. Je to dôležité na diagnostiku problémov používateľa súvisiacich s predplatným a na zistenie regresií pre používateľov s už aktivovaným predplatným.

Zhromažďujú sa tieto polia:

  - **Mode** – enumerátor predstavujúci postup licencovania balíka Office, ktorý sa používa v tomto zariadení

### <a name="officelicensinginrfm"></a>Office.Licensing.InRFM 

Ak zariadenie prejde do režimu obmedzenej funkčnosti, tento signál sa odosiela na signalizovanie, že zariadenie nie je v poriadku. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **ACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu

  - **DaysRemaining** – počet dní zostávajúcich do uplynutia platnosti aktuálnej licencie na Office

  - **Mode** – enumerátor predstavujúci postup licencovania balíka Office, ktorý sa používa v tomto zariadení

  - **ProductName** – názov produktu, ktorý používateľ momentálne používa

  - **Reason** – chybový kód signalizujúci dôvod aktuálneho stavu licencie

### <a name="officelicensinginstallkey"></a>Office.Licensing.InstallKey

Táto udalosť sa zhromažďuje, keď sa pokúšame nainštalovať do zariadenia kľúč na licencovanie zariadenia. Nahlasuje, či inštalácia bola úspešná a či sa po nej nezobrazil kód chyby. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **Prid** – názov skupiny produktov, pre ktorú sa inštaluje kľúč

  - **SkuId** – identifikátor GUID predstavujúci produkt balíka Office, pre ktorý sa inštaluje kľúč 

### <a name="officelicensinginvokelicensewizard"></a>Office.Licensing.InvokeLicenseWizard

V prípade problémov s postupom aktivácie sa spustí licenčný sprievodca a odošle sa signál signalizujúci túto skutočnosť. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **ACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu

  - **LicenseStatus** – stav licencie na Office, ktorú používateľ používa

  - **MachineKey** – alfanumerický identifikátor licenčného kľúča, ktorý bol vydaný používateľovi

### <a name="officelicensinglicensingbar"></a>Office.Licensing.LicensingBar

Ak sa v zariadení vyskytujú problémy s licencovaním a používateľovi sa zobrazí oznámenie, odošle sa tento signál, ktorý uvádza aj typ oznámenia. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **SuppressNotification** – označuje, či sa oznámenie potlačilo

  - **Title** – nadpis licenčného oznámenia zobrazeného používateľovi

  - **Type** – typ licenčného oznámenia zobrazeného používateľovi

### <a name="officelicensinglicexitofficeprocess"></a>Office.Licensing.LicExitOfficeProcess 

Ak dôjde k ukončeniu alebo zlyhaniu balíka Office z dôvodu licenčných problémov, odošleme tento signál na signalizáciu tejto skutočnosti. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **ExitCode** – interný kód, ktorý spôsobil ukončenie aplikácie

### <a name="officelicensingloadidentityticket"></a>Office.Licensing.LoadIdentityTicket

Počas pokusu o licencovanie zariadenia sa aplikácia pokúsi načítať identitu používateľa s cieľom zistiť, či má používateľ nárok na Office alebo nie. Táto udalosť nahlasuje úspech alebo zlyhanie tohto pokusu spoločne s kódom chyby. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **FederationProvider** – reťazec, ktorý identifikuje poskytovateľa federovania pre aktuálne prihláseného používateľa

  - **IdentityProvider** – reťazec, ktorý identifikuje poskytovateľa identity pre aktuálne prihláseného používateľa

### <a name="officelicensinglvuxeulaexplicitcrash"></a>Office.Licensing.LVUX.EULAExplicitCrash 

Táto udalosť sa zhromažďuje, ak používateľ neprijal zobrazenú zmluvu EULA, v dôsledku čoho aplikácia zlyhala alebo sa ukončila. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **ACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu

  - **OptInShown** – signalizuje, či sa dialógové okno s vyjadrením výslovného súhlasu zobrazované pri prvom spustení aplikácie už zobrazilo

### <a name="officelicensingnextuserlicensingeligible"></a>Office.Licensing.NextUserLicensingEligible 

Tento signál uvádza, či používateľ je oprávnený na prechod na nový postup licencovania. Je to dôležité na kvantifikovanie vplyvu na existujúcich používateľov pri zavádzaní nového postupu licencovania a zaručenie, že používatelia nestratia funkcie.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officelicensingnulfetcherfetchmodelfromols"></a>Office.Licensing.Nul.Fetcher.FetchModelFromOls

Keď sa v zariadení používa moderný postup licencovania, pokúšame sa získať súbor s licenciou priamo zo služby. Táto udalosť nahlasuje úspech alebo neúspech spoločne s kódom chyby volania služby. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave v modernom postupe licencovania, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **MetadataValidationResult** – výsledok overenia metaúdajov licencie na overenie, či sa s ňou nemanipulovalo

  - **SignatureValidationResult** – výsledok overenia podpisu licencie na overenie, či sa s ňou nemanipulovalo

### <a name="officelicensingnulvalidationfullvalidation"></a>Office.Licensing.Nul.Validation.FullValidation 

Táto udalosť sa zhromažďuje v každej relácii zariadenia, ktoré používa moderný postup licencovania. Nahlasuje stav licencovania zariadenia a chyby, ktoré sa používateľovi zobrazujú a pre ktoré nemôže používať aplikáciu. Táto udalosť signalizuje, či je zariadenie používateľa v dobrom stave v modernom postupe licencovania. Pre túto udalosť je vytvorené zisťovanie anomálie na rozpoznávanie, či regresia spôsobuje nevhodné správanie používateľa. Je to dôležité aj pri zisťovaní problémov používateľa a na monitorovanie stavu systému.

Zhromažďujú sa tieto polia:

  - **ACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu 

  - **AllAcids** – zoznam všetkých identifikátorov GUID produktu, pre ktorý je používateľ v súčasnosti licencovaný 

  - **Category** – kategória licencie na Office, ktorú používateľ používa 

  - **DaysRemaining** – počet dní zostávajúcich do uplynutia platnosti aktuálnej licencie na Office 

  - **LicenseId** – alfanumerický identifikátor licencie, ktorá bola vydaná používateľovi 

  - **LicenseType** – typ licencie na Office, ktorú používateľ používa 

### <a name="officelicensingofficeclientlicensingdolicensevalidation"></a>Office.Licensing.OfficeClientLicensing.DoLicenseValidation 

Toto sú metaúdaje licencovania, ktoré sa zhromažďujú zo zariadenia pri každom spustení a ktoré hlásia identifikátor acid licencie, stav a typ licencie a ďalšie vlastnosti licencie, ktoré sú dôležité pri identifikácii množiny funkcií dostupných používateľovi. Je to dôležité pri identifikácii množiny funkcií dostupných používateľovi a toho, či používateľovi chýba nejaká funkcia. Používa sa aj pri výpočte denného a mesačného počtu aktívnych používateľov a v rôznych ďalších zostavách rôznych tímov v rámci Office, pretože informuje o type produktu, ktorý používateľ používa, či ide o produkt s predplatným a či chýbajú nejaké kritické funkcie.

Zhromažďujú sa tieto polia:

  - **FullValidationMode** – režim signalizujúci, že ide o úplné potvrdenie overenia licencie 

  - **IsRFM** – označuje, či sa používateľ nachádza v režime obmedzenej funkčnosti alebo nie 

  - **IsSCA** – označuje, či je spustený režim aktivácie v zdieľanom počítači 

  - **IsSubscription** – označuje, či používateľ používa predplatenú licenciu alebo nie 

  - **IsvNext** – označuje, či sa používa nový moderný postup licencovania alebo nie 

  - **LicenseCategory** – kategória licencie na Office, ktorú používateľ používa 

  - **LicenseStatus** – stav licencie na Office, ktorú používateľ používa 

  - **LicenseType** – typ licencie na Office, ktorú používateľ používa 

  - **LicensingACID** – identifikátor GUID predstavujúci produkt balíka Office, na ktorý má používateľ licenciu 

  - **OlsLicenseId** – alfanumerický identifikátor licencie, ktorá bola vydaná používateľovi 

  - **SkuIdIsNull** – označuje, či sa vyskytla chyba a nevie sa, ktorý produkt má používateľ spustený 

  - **SlapiIsNull** – označuje, či sa vyskytol problém pri napĺňaní jedného z licenčných objektov 

### <a name="officelicensingonlinerepair"></a>Office.Licensing.OnlineRepair 

Táto udalosť sa spustí, ak z nejakého dôvodu nie je možné aktivovať používateľa a zobrazilo sa mu dialógové okno s požiadavkou na prechod online a vyskúšanie krokov opravy. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officelicensingpurchase"></a>Office.Licensing.Purchase 

Máme experiment, ktorý používateľovi umožňuje vyskúšať a nastaviť automatické platby za Office priamo z aplikácie bez opustenia kontextu aplikácie. Táto udalosť nahlasuje úspech alebo zlyhanie tohto experimentu spoločne s kódom chyby. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **StorePurchaseStatus** – predstavuje kód chyby kód alebo kód úspechu volania nákupu, ktoré sa uskutočnilo prostredníctvom Windows Storu

### <a name="officelicensingsearchforsessiontoken"></a>Office.Licensing.SearchForSessionToken

Ak je používateľ v režime aktivácie v zdieľanom počítači, snažíme sa vyhľadať v zariadení token relácie relácie, ktorý používateľovi umožňuje používať aplikáciu. Táto udalosť nahlasuje úspech alebo zlyhanie tohto scenára spoločne s kódom chyby. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **LoadLicenseResult** – predstavuje kód chyby alebo kód úspechu vyjadrujúci, či sa podarilo načítať licencie pre aktuálneho používateľa

  - **OpportunisticTokenRenewalAttempted** – signalizuje, či sa vykonal pokus o oportunistické obnovenie tokenu relácie používateľa

  - **SetAcidResult** – predstavuje kód chyby alebo kód úspechu vyjadrujúci, či sa podarilo nastaviť identifikátor acid na očakávanú hodnotu

### <a name="officelicensingshownewdeviceactivationdialog"></a>Office.Licensing.ShowNewDeviceActivationDialog

Pri prvom spustení aplikácie balíka Office sa vykoná pokus o zobrazenie dialógového okna s vopred vyplnenými povereniami, s ktorými používateľ stiahol balík Office. Používateľ potom môžete pokračovať prihlásením s týmito povereniami, použiť iné poverenia alebo zrušiť dialógové okno. Táto udalosť nahlasuje akciu, ktorú používateľ vykonal, keď sa mu zobrazilo toto dialógové okno. Je to dôležité na zistenie, či sa používateľ nachádza v dobrom stave v modernom postupe licencovania, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **UserAction** – identifikátor akcie, ktorú používateľ vykonal, keď sa mu zobrazilo dialógové okno

### <a name="officelicensingskutoskuconversion"></a>Office.Licensing.SkuToSkuConversion

Ak je v rámci licencovania používateľa nutné zmeniť SKU používateľa z jednej SKU na inú, odošleme tento signál spoločne s kódom úspechu alebo neúspechu. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **DestinationSku** – názov SKU, na ktorú sa aktuálne nainštalovaný produkt má skonvertovať

  - **PendingAcid** – ID produktu, pre ktorý sa má SKU skonvertovať

  - **SourceSku** – názov pôvodnej SKU, ktorá bola nainštalovaná v počítači

  - **UninstallProduct** – označuje, či sa starý produkt v rámci konverzie odinštaluje

### <a name="officelicensingusegracekey"></a>Office.Licensing.UseGraceKey

Ak z nejakého dôvodu nie je možné priradiť licenciu používateľovi, nainštaluje sa kľúč odkladu a odošle sa tento signál, ktorý to vyjadruje. Je to dôležité na určenie, či sa používateľ nachádza v dobrom stave a nechýba mu nejaká funkcia, na určenie stavu systému a na diagnostické účely, ak používateľ nahlási problém so zariadením.

Zhromažďujú sa tieto polia:

  - **OpportunisticTokenRenewalAttempted** – signalizuje, či sa vykonal pokus o oportunistické obnovenie pre používateľa v režime aktivácie v zdieľanom počítači

  - **ReArmResult** – označuje výsledok obnovenia aktivačného obdobia pre nainštalovaný kľúč, čím sa môže predĺžiť platnosť aktuálnej licencie

## <a name="microsoft-autoupdate-mau-events"></a>Udalosti služby Microsoft AutoUpdate (MAU)

### <a name="appdelegate_launch"></a>appdelegate_launch

Táto udalosť označuje, že sa vyskytol pokus o spustenie aplikácie. Zaznamenáme jej výsledok (zlyhanie alebo úspech). Táto udalosť sa používa na identifikáciu prípadov, v ktorých sa služba MAU nedokáže spustiť.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť
    
- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppversionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

 - **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – množina statického textu označujúca stav spustenia.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="appdelegate_terminate"></a>appdelegate_terminate

Táto udalosť označuje, že došlo k riadnemu ukončeniu aplikácie. Táto udalosť sa používa na odlíšenie riadnych ukončení aplikácie od mimoriadnych.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu
    
- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia
    
- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text označujúci, že služba Microsoft Autoupdate sa ukončila.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="appinstall_connecttoxpc"></a>appinstall_connecttoxpc

Táto udalosť označuje, že sa vyskytli chyby pri pripájaní k pomocnému nástroju služby MAU (komponent, ktorý vykonáva inštaláciu aplikácie).  Táto udalosť označuje možné poškodenie aplikácie MAU. Zariadenie nebude môcť inštalovať aktualizácie.

Zhromažďujú sa tieto polia: 

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie o chybe týkajúce sa problému s pripojením.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé tri oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="appregistry_info"></a>appregistry_info

Táto udalosť označuje, že aplikácia sa spustila. Táto udalosť sa používa na zobrazenie zoznamu aplikácií, pre ktoré môže služba MAU riadiť aktualizácie, počtu dostupných kópií a ich verzií a umiestnenia inštalácie (predvolené alebo iné).

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie o zozname identifikátorov, ktoré aplikácia používa na registráciu so službami Microsoft Autoupdate, a počte inštalácií zaregistrovaných pre aplikáciu.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="appregistry_remove"></a>appregistry_remove

Táto udalosť označuje, že došlo k pokusu o odstránenie aplikácie zo zoznamu aplikácií spravovaných službou MAU. Táto udalosť sa používa na overenie, že služba MAU spravuje len aplikácie vydané pre službu MAU (nemali by sa tu zobraziť žiadne aplikácie z obchodu s aplikáciami).

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – názov a identifikátor odstraňovanej aplikácie, informácia o tom, či aplikácia stále existuje v registrovanom umiestnení a či bola nainštalovaná z obchodu s aplikáciami.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="catalog_errorsignature"></a>catalog_errorsignature

Táto udalosť označuje, že došlo k zlyhaniu počas overovania podpisu kódu v súbore kolaterálu aktualizácie.  Akýkoľvek kolaterál so zlyhaním overenia podpisu kódu by sa mal považovať za neplatný.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov súboru katalógu s neplatným podpisom. Rôzny statický text popisuje rôzne chybové podmienky.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé tri oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="cloningtask_helpertoolconnection"></a>cloningtask_helpertoolconnection

Táto udalosť zaznamenáva problémy s inštaláciou na klon (t. j. buď sa nám nedarí pripojiť k pomocnému nástroju na použitie aktualizácie, alebo sa pripojíme, ale pomocný objekt nemôže použiť aktualizáciu). Ak sa nahlási záznam, znamená to, že inštalácia na klon zlyhala a teraz sa bude musieť vrátiť na aktualizáciu na mieste.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor na identifikáciu jednej aktivity aktualizácie a chybu servera proxy nahlásenú počas procesu klonovania.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé tri oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="configuration_channel"></a>configuration_channel

Táto udalosť zaznamenáva pokusy o prepínanie kanálov (cieľovej skupiny) v službe MAU.  Používa sa na zaznamenávanie pokusov a ich výsledkov (úspech alebo neúspech).

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov vybratého kanála.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé tri oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="configuration_metadata"></a>configuration_metadata

Táto udalosť sa zaznamenáva vždy, keď sa inicializuje služba MAU. Ide o typ udalosti prezenčného signálu služby MAU

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text s informáciou, či sa inicializujú jednotlivé metaúdaje alebo konfigurácia.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie.


### <a name="controller_alertmanager_reinstallresponse"></a>controller_alertmanager_reinstallresponse

Táto udalosť označuje, že služba MAU sa dostala do nepoužiteľného alebo neopraviteľného stavu a musí sa preinštalovať. Táto udalosť označuje, že došlo k neopraviteľnej chybe a vyžaduje sa zásah používateľa.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje vymenovaný výber používateľa.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_alertmanager_tmpdiskfull"></a>controller_alertmanager_tmpdiskfull

Táto udalosť označuje, že sa zistil nedostatok miesta na disku. Nebude možné inštalovať aktualizácie z dôvodu nedostatku miesta na disku.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_alertmanager_tmpdiskfullretry"></a>controller_alertmanager_tmpdiskfullretry

Táto udalosť označuje, že sa spustil opätovný pokus o inštaláciu aktualizácie po zistení nedostatku miesta na disku. Po nemožnosti nainštalovať aktualizácie z dôvodu nedostatku miesta na disku sa pokúsime inštaláciu vykonať znova.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie
    

### <a name="controller_alertmanager_tmpdiskfullretrycancel"></a>controller_alertmanager_tmpdiskfullretrycancel

Táto udalosť označuje, že došlo k zrušeniu opätovného pokusu o inštaláciu po zistení nedostatku miesta na disku. Táto udalosť sa používa na zistenie, či náš záložný mechanizmus bol postačujúci na to, aby mohol používateľa sprevádzať procesom aktualizácie, keď sa zistil nedostatok miesta na disku.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)
    
- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií
    
- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_checkwindow_noupdatefoundok"></a>controller_checkwindow_noupdatefoundok

Táto udalosť označuje, že pri vyhľadávaní aktualizácií sa nenašli žiadne aktualizácie. Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií, optimalizáciu zaťažení služby a definovanie frekvencie vyhľadávania aktualizácií. Tiež chceme optimalizovať frekvenciu vydávania na základe očakávania používateľov týkajúceho sa aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    

### <a name="controller_checkwindow_updatecheck"></a>controller_checkwindow_updatecheck

Táto udalosť označuje, že sa vykonala kontrola aktualizácií. Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií, optimalizáciu zaťažení služby a definovanie frekvencie vyhľadávania aktualizácií. Tiež chceme optimalizovať frekvenciu vydávania na základe očakávania používateľov týkajúceho sa aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia
    
- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_checkwindow_updatecheckcancel"></a>controller_checkwindow_updatecheckcancel

Táto udalosť označuje, že proces kontroly aktualizácií bol zrušený (buď používateľom alebo systémom). Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií, optimalizáciu zaťažení služby a definovanie frekvencie vyhľadávania aktualizácií. Tiež chceme optimalizovať frekvenciu vydávania na základe očakávania používateľov týkajúceho sa aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_checkwindow_updatecheckcanceluser"></a>controller_checkwindow_updatecheckcanceluser

Táto udalosť označuje, že proces kontroly aktualizácií bol zrušený používateľom.  Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií, optimalizáciu zaťažení služby a definovanie frekvencie vyhľadávania aktualizácií. Tiež chceme optimalizovať frekvenciu vydávania na základe očakávania používateľov týkajúceho sa aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie
    
- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_checkwindow_updatesfound"></a>controller_checkwindow_updatesfound

Táto udalosť označuje, že pri vyhľadávaní aktualizácií sa našli aktualizácie.  Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_checkwindow_uptodate"></a>controller_checkwindow_uptodate

Táto udalosť označuje, že pri vyhľadávaní aktualizácií sa nenašli žiadne aktualizácie, pretože aplikácie v zariadení sú aktuálne.  Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_applaunchwithpendingupdate"></a>controller_downloadwindow_applaunchwithpendingupdate

Táto udalosť označuje, že došlo k spusteniu aplikácie, pre ktorú práve prebieha proces získavania aktualizácie. Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií. Otvorené aplikácie by nemali získavať aktualizácie. Aplikácie sa pred aktualizovaním musia zavrieť.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy
    
- **SessionId** – identifikátor relácie

    
### <a name="controller_downloadwindow_closeapplicationdialog"></a>controller_downloadwindow_closeapplicationdialog

Táto udalosť označuje, že došlo k spusteniu aplikácie, pre ktorú práve prebieha proces získavania aktualizácie. Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií. Otvorené aplikácie by nemali získavať aktualizácie. Aplikácie sa pred aktualizovaním musia zavrieť.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_downloadwindow_curtasknull"></a>controller_downloadwindow_curtasknull

Táto udalosť označuje, že pri pokuse o použitie aktualizácie sa vyskytla chyba. Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_downloadwindow_downloadcancel"></a>controller_downloadwindow_downloadcancel

Táto udalosť označuje, že proces sťahovania bol zrušený používateľom.  Táto udalosť sa používa na zaručenie správnosti ponúkania aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – statický text. 

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_downloadwindow_downloadfailed"></a>controller_downloadwindow_downloadfailed

Táto udalosť označuje, že pri sťahovaní aktualizácie došlo k zlyhaniu. Táto udalosť sa používa na zaručenie správnosti ponúkania a sťahovania aktualizácií.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_downloadwindow_downloadfailedok"></a>controller_downloadwindow_downloadfailedok

Táto udalosť označuje, že pri sťahovaní aktualizácie došlo k zlyhaniu a používateľ bol informovaný. Táto udalosť sa používa na zaručenie správnosti ponúkania a sťahovania aktualizácií a toho, že v prípade zlyhania sa používateľovi zobrazí oznámenie.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_downloadpathmissing"></a>controller_downloadwindow_downloadpathmissing

Táto udalosť označuje, že pri sťahovaní aktualizácie došlo k zlyhaniu. Táto udalosť sa používa na zaručenie správnosti ponúkania a sťahovania aktualizácií. Táto udalosť označuje, že URL adresa sťahovania chýba.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_downloadtasknull"></a>controller_downloadwindow_downloadtasknull

Táto udalosť označuje, že pri sťahovaní aktualizácie došlo k zlyhaniu. Táto udalosť sa používa na zaručenie správnosti ponúkania a sťahovania aktualizácií. Táto udalosť označuje, že služba Microsoft AutoUpdate bola požiadaná o pozastavenie/obnovenie sťahovania, ale nepodarilo sa jej nájsť príslušného správcu sťahovania.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_filesignaturenotverified"></a>controller_downloadwindow_filesignaturenotverified

Táto udalosť označuje, že pri sťahovaní aktualizácie došlo k zlyhaniu. Táto udalosť označuje, že služba Microsoft AutoUpdate nedokázala overiť, že túto aktualizáciu vydala spoločnosť Microsoft. Táto udalosť sa používa na zaručenie správnosti ponúkania a sťahovania aktualizácií. 

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý obsahuje URL adresu sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_installcomplete"></a>controller_downloadwindow_installcomplete

Táto udalosť označuje, že inštalácia všetkých aktualizácií ponúknutých službou Microsoft AutoUpdate sa dokončila. Táto udalosť sa používa na zaručenie správnosti ponúkania a sťahovania aktualizácií. 

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená
    
- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_networkunavailablealert"></a>controller_downloadwindow_networkunavailablealert

Táto udalosť označuje, že počas sťahovania aktualizácií sa prerušilo sieťové pripojenie.  Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_downloadwindow_networkunavailablealertok"></a>controller_downloadwindow_networkunavailablealertok

Táto udalosť označuje, že počas sťahovania aktualizácií sa prerušilo sieťové pripojenie. Označuje tiež, že používateľ bol o tejto chybe informovaný. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_downloadwindow_noconnectionok"></a>controller_downloadwindow_noconnectionok

Táto udalosť označuje, že počas sťahovania aktualizácií sa prerušilo sieťové pripojenie. Označuje tiež, že používateľ bol o tejto chybe informovaný. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_repairrequired"></a>controller_downloadwindow_repairrequired

Táto udalosť označuje, že proces aktualizácie zlyhal. Označuje tiež, že aktualizácia bola dokončená, ale služba Microsoft AutoUpdate zistila problém s aktualizovanou aplikáciou a vyžaduje sa oprava. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)
    
- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia
    
- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

### <a name="controller_downloadwindow_updateaborted"></a>controller_downloadwindow_updateaborted

Táto udalosť označuje, že proces aktualizácie bol zrušený. Označuje tiež, že aktualizácia už prebiehala pomocou démona a používateľ klikol na tlačidlo OK na zrušenie sťahovania. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_updatefailed"></a>controller_downloadwindow_updatefailed

Táto udalosť označuje, že niektoré aktualizácie z aktuálnej dávky zlyhali. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_updatesuccessful"></a>controller_downloadwindow_updatesuccessful

Táto udalosť označuje, že všetky aktualizácie z aktuálnej dávky boli úspešné. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_userpaused"></a>controller_downloadwindow_userpaused

Táto udalosť označuje, že všetky aktualizácie z aktuálnej dávky boli úspešné. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_downloadwindow_userresumed"></a>controller_downloadwindow_userresumed

Táto udalosť označuje, že proces sťahovania aktualizácií bol po predchádzajúcom pozastavení úspešne obnovený. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť
    
- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_mainwindow_setautomaticdownloadinstall"></a>controller_mainwindow_setautomaticdownloadinstall

Táto udalosť označuje, že zariadenie bolo zaradené do režimu automatickej aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_mainwindow_setmanualchecking"></a>controller_mainwindow_setmanualchecking

Táto udalosť označuje, že zariadenie bolo zaradené do režimu manuálnej aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_templateawindow_cancel"></a>controller_templateawindow_cancel

Táto udalosť označuje, že používateľ sa rozhodol zrušiť alebo ignorovať zobrazené výstražné hlásenie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_templateawindow_enroll"></a>controller_templateawindow_enroll

Táto udalosť označuje, že používateľ sa rozhodol riadiť zobrazeným výstražným odporúčaním. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií
    
- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie



### <a name="controller_templateawindow_install"></a>controller_templateawindow_install

Táto udalosť označuje, že používateľ sa rozhodol riadiť zobrazeným výstražným odporúčaním týkajúcim sa spustenia akcie inštalácie softvéru. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_updatewindow_begindownloadingapps"></a>controller_updatewindow_begindownloadingapps

Táto udalosť označuje, že sťahovanie aktualizácií sa začalo prostredníctvom okna aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje slovník dostupných balíkov aktualizácií a informáciu o tom, či používateľ zvolil inštaláciu danej položky.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_updatewindow_networkretry"></a>controller_updatewindow_networkretry

Táto udalosť označuje, že na hárku aktualizácie sa spustil opakovaný pokus z dôvodov zlyhania siete. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.

Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_updatewindow_networkretrycancel"></a>controller_updatewindow_networkretrycancel

Táto udalosť označuje, že na hárku aktualizácie sa nepodarilo spustiť opakovaný pokus z dôvodov zlyhania siete. Táto udalosť označuje, že používateľ zvolil zrušenie aktualizácií po upozornení na nedostupnosť siete. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_updatewindow_networkunavailable"></a>controller_updatewindow_networkunavailable

Táto udalosť označuje, že sa náhle prerušilo sieťové pripojenie. Táto udalosť označuje, že server nie je dosiahnuteľný pri pokuse o stiahnutie balíka s aktualizáciou. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_updatewindow_noupdateavailable"></a>controller_updatewindow_noupdateavailable

Táto udalosť označuje, že došlo k vyhľadávaniu aktualizácií a nie sú k dispozícii žiadne aktualizácie. Táto udalosť označuje, že služba Microsoft Autoupdate nenašla žiadne dostupné aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_updatewindow_noupdatestoselect"></a>controller_updatewindow_noupdatestoselect

Táto udalosť označuje, že sa vyskytla chyba, ktorej výsledkom je prázdny zoznam aktualizácií. Táto udalosť označuje, že služba Microsoft Autoupdate zobrazuje prázdny hárok aktualizácie. Nemalo by sa to stať. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="controller_updatewindow_updateavailable"></a>Controller_UpdateWindow_UpdateAvailable

Táto udalosť označuje, že došlo k vyhľadávaniu aktualizácií a neponúkajú sa žiadne aktualizácie. Táto udalosť sa používa na určenie, či sa aktualizácie ponúknu používateľom na zobrazenie, či sa zobrazujú správne aktualizácie alebo či blokovanie aktualizácií funguje podľa očakávaní. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje slovník dostupných balíkov aktualizácií a stav voľby používateľa pre každý z nich.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="controller_updatewindow_updateavailablecancel"></a>controller_updatewindow_updateavailablecancel

Táto udalosť označuje, že používateľ zrušil akciu po zobrazení hárku aktualizácie so zoznamom aktualizácií. Táto udalosť sa používa na vysvetlenie dôvodov neaktualizovania (t .j. že používateľ ju vedome zrušil). Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadactor_pause"></a>downloadactor_pause

Táto udalosť označuje, že používateľ zadal požiadavku na pozastavenie sťahovania. Táto udalosť sa používa na vysvetlenie dôvodov zjavného nedokončenia aktualizácií. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadactor_redirect"></a>downloadactor_redirect

Táto udalosť označuje, že agent sťahovania je nasmerovaný na koncový bod, ktorý vydáva presmerovanie URL adresy pre požiadavku na sťahovanie. Táto udalosť sa používa na vysvetlenie dôvodov zlyhania sťahovania a diagnostiku problémov s proxy serverom. Takisto môže pomôcť diagnostikovať príčiny, keď sa u používateľov pozoruje inštalácia starších zostáv. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje URL adresu presmerovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="downloadactor_resume"></a>downloadactor_resume

Táto udalosť označuje, že používateľ zadal požiadavku na obnovenie pozastaveného sťahovania. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadactor_resumeerror"></a>downloadactor_resumeerror

Táto udalosť označuje, že používateľ zadal požiadavku na obnovenie pozastaveného sťahovania. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje URL adresu sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="downloadactor_status"></a>downloadactor_status

Táto udalosť zaznamenáva, že sa vyskytli pokusy o načítanie súborov kolaterálu, a ich výsledok (úspech alebo neúspech). Chceme poznať načítavané kolaterály a balíky. Načítanie nesprávneho súboru môže znamenať problém so zostavou alebo kolaterálom. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje URL adresu sťahovania a kód chyby v prípade zlyhania. URL adresa sťahovania je umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_downloadcatalogfail"></a>downloadmanifest_downloadcatalogfail

Táto udalosť označuje, že došlo k zlyhaniu sťahovania. Súbor, ktorý sa nepodarilo stiahnuť, sa zaznamená. Chceme poznať načítavané kolaterály a balíky. Zlyhanie stiahnutia manifestu môže poukazovať na zlyhanie vygenerovania kolaterálu, chybu konfigurácie siete CDN, chybu konfigurácie klienta alebo chybu siete. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje kód chyby sťahovania a URL adresu súboru sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="downloadmanifest_downloadcatalogsuccess"></a>downloadmanifest_downloadcatalogsuccess

Táto udalosť označuje, že súbor sa úspešne stiahol. Zlyhanie stiahnutia manifestu môže poukazovať na zlyhanie vygenerovania kolaterálu, chybu konfigurácie siete CDN, chybu konfigurácie klienta alebo chybu siete. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť
    
- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje kód chyby sťahovania a URL adresu súboru sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_downloadfail"></a>downloadmanifest_downloadfail

Táto udalosť označuje, že pri sťahovaní sa vyskytla chyba. Súbor manifestu alebo balíka, ktorý sa nepodarilo stiahnuť, ako aj podrobnosti o chybe, sa zaznamenajú. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje kód chyby sťahovania a URL adresu súboru sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_downloadfromurl"></a>downloadmanifest_downloadfromurl

Táto udalosť označuje, že sťahovanie súboru katalógu sa začalo. URL adresa, z ktorej sa súbor katalógu sťahuje, sa zaznamená. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje kód chyby sťahovania a URL adresu súboru sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_downloading"></a>downloadmanifest_downloading

Táto udalosť označuje, že sťahovanie súboru katalógu sa začalo. URL adresa, z ktorej sa súbor katalógu sťahuje, sa zaznamená. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje kód chyby sťahovania a URL adresu súboru sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_downloadsuccess"></a>downloadmanifest_downloadsuccess

Táto udalosť označuje, že súbor xml a súbor balíka sa úspešne stiahol. URL adresa, z ktorej sa súbor stiahol, sa zaznamená. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje kód chyby sťahovania a URL adresu súboru sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="downloadmanifest_downloadurl"></a>downloadmanifest_downloadurl

Táto udalosť označuje, že sa zadala požiadavka na stiahnutie súboru. URL adresa, z ktorej sa súbor stiahol, sa zaznamená. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť
    
- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje kód chyby sťahovania a URL adresu súboru sťahovania. Ide o umiestnenie so súbormi na stiahnutie spoločnosti Microsoft s výnimkou prípadov, keď je kanál nastavený na možnosť Vlastný. Pri vlastnom kanáli je táto hodnota nastavená na možnosť Custom Location (Vlastné umiestnenie).

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_filenameerror"></a>downloadmanifest_filenameerror

Táto udalosť označuje, že sa vyskytla neočakávaná chyba. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_invalidhash"></a>downloadmanifest_invalidhash

Táto udalosť označuje zlyhanie overenie zabezpečenia našich súborov. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov stiahnutého súboru s neplatnou hodnotou hash.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_missingdaemon"></a>downloadmanifest_missingdaemon

Táto udalosť označuje, že používateľ sa pokúsil vyhľadať aktualizácie a zistili sme, že v službe MAU chýba základný komponent (démon). Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_signatureerror"></a>downloadmanifest_signatureerror

Táto udalosť označuje, že zlyhalo overenie podpisu kódu pre balík. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov stiahnutého súboru s neplatnou hodnotou hash.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmanifest_status"></a>downloadmanifest_status

Táto udalosť zaznamenáva súhrnnú agregáciu pokusov/zlyhaní počas procesu sťahovania pre súbor manifestu a balíka. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie vrátane URL adresy (adresa spoločnosti Microsoft), predpony sťahovaného súboru, zistených chýb atď.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmgr_downloadend"></a>downloadmgr_downloadend

Táto udalosť zaznamenáva značku, ktorá označuje, že proces sťahovania sa dokončil samostatne. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie vrátane URL adresy (adresa spoločnosti Microsoft), predpony sťahovaného súboru, zistených chýb atď.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadmgr_downloadstart"></a>downloadmgr_downloadstart

Táto udalosť zaznamenáva aktualizáciu, ktorá sa chystá stiahnuť. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov sťahovanej aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadtask_downloadfailure"></a>downloadtask_downloadfailure

Táto udalosť zaznamenáva, že pri sťahovaní súboru balíka sa vyskytla chyba. Cesta aktualizácie a chyba sa zaznamená. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov sťahovanej aktualizácie a zistenú chybu.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="downloadtask_downloadsuccess"></a>downloadtask_downloadsuccess

Táto udalosť zaznamenáva úspešné stiahnutie súboru balíka. Použitá cesta aktualizácie sa zaznamená. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje cestu aktualizácie pre úspešné stiahnutie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_checkforupdate"></a>fba_checkforupdate

Táto udalosť označuje, že proces na pozadí vyhľadáva aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_checkforupdateskip"></a>fba_checkforupdateskip

Táto udalosť označuje, že proces na pozadí vynechal aktualizáciu, pretože je otvorené používateľské rozhranie služby MAU. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_launchstatus"></a>fba_launchstatus

Táto udalosť zaznamenáva zlyhania démona služby MAU pri pokuse o spustenie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje OSStatus (kód stavu Apple) zohľadňujúci stav spustenia.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_silentupdateoptin"></a>fba_silentupdateoptin

Táto udalosť označuje, že používateľ sa rozhodol pre tiché aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_skipforcedupdate"></a>fba_skipforcedupdate

Táto udalosť označuje, že vynútená kontrola aktualizácií sa vynechala z dôvodu otvorených aplikácií. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_startforcedupdate"></a>fba_startforcedupdate

Táto udalosť označuje, že sa vyskytol pokus o použitie vynútenej aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_terminate"></a>fba_terminate

Táto udalosť označuje, že démon služby MAU sa ukončil normálne. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fba_updatefound"></a>fba_updatefound

Táto udalosť označuje, že démon služby MAU našiel dostupné aktualizácie na ponúknutie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje počet nájdených dostupných aktualizácií.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="fba_updatetimer"></a>fba_updatetimer

Táto udalosť označuje, že proces démona služby Microsoft Autoupdate sa stal aktívny, aby skontroloval aktualizácie po nastavenom časovom úseku spánku. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie o aktuálnom dátume a čase.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_allappsclosed"></a>fbasilentupdate_allappsclosed

Táto udalosť zaznamenáva, či boli všetky aplikácie pred inštaláciou zavreté. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu
    
- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_applaunchafterupdate"></a>fbasilentupdate_applaunchafterupdate

Táto udalosť zaznamenáva pokus o opätovné spustenie aplikácie po tichej aktualizácii a režim aktualizácie (klon alebo nie). Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aplikácie, ktorá sa má spustiť.
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)
    
- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_applaunchwileinstalling"></a>fbasilentupdate_applaunchwileinstalling

Táto udalosť zaznamenáva, keď došlo k spusteniu aktualizácie počas inštalácie aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_appneedtoclose"></a>fbasilentupdate_appneedtoclose

Táto udalosť zaznamenáva, keď sa po spustení procesu aktualizácie zistí, že zistí, že došlo k otvoreniu aplikácie, ktorá sa má aktualizovať. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aplikácie a identifikátor zväzku aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_appterminationeventreceived"></a>fbasilentupdate_appterminationeventreceived

Táto udalosť označuje, že služba Microsoft Autoupdate prijala udalosť Apple, ktorá informuje o tom, že aplikácia sa ukončila. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a identifikátor zväzku aplikácie. Môže tiež obsahovať reťazec chyby, ak služba Microsoft Autoupdate určí, že aplikácia je stále spustená aj po prijatí udalosti ukončenia.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_codesignfailure"></a>fbasilentupdate_codesignfailure

Táto udalosť zaznamenáva výsledok overenia podpisu kódu po použití aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje výsledok operácie overenia podpisu kódu.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_download"></a>fbasilentupdate_download

Táto udalosť označuje, že sa sťahuje aktualizácia. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_downloadfailed"></a>fbasilentupdate_downloadfailed

Táto udalosť označuje, že počas sťahovania aktualizácie došlo k zlyhaniu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_downloadinbackground"></a>fbasilentupdate_downloadinbackground

Táto udalosť označuje, že sa spúšťa sťahovanie množiny aktualizácií na pozadí (zaznamenáva sa počet súčasne sťahovaných aktualizácií). Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje počet aktualizácií vo fronte.

    - **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_downloadingrepairupdate"></a>fbasilentupdate_downloadingrepairupdate

Táto udalosť označuje, že sa spustil pokus o stiahnutie opravy pre neúspešnú aktualizáciu. Verzia a aktualizácia sa zaznamená. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aktualizácie.
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_duplicatedownloadattempted"></a>fbasilentupdate_duplicatedownloadattempted

Táto udalosť označuje, že sa vyskytla chyba. Naraz by sa mala sťahovať len jedna aktualizácia pre danú aplikáciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_installattemptfailed"></a>fbasilentupdate_installattemptfailed

Táto udalosť označuje, že pokus o inštaláciu aktualizácie (verzie) zlyhal. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_installcomplete"></a>fbasilentupdate_installcomplete

Táto udalosť označuje, že sa skončila inštalácia všetkých aktualizácií v dávke. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_installed"></a>fbasilentupdate_installed

Táto udalosť označuje, že individuálna aktualizácia sa úspešne nainštalovala. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti. Obsahuje identifikátor aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="fbasilentupdate_installing"></a>fbasilentupdate_installing

Táto udalosť označuje, že sa spustila individuálna aktualizácia. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aplikácie a názov balíka aktualizácie.
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_notificationremoved"></a>fbasilentupdate_notificationremoved

Táto udalosť označuje, že aktualizácia, ktorá bola blokovaná, už nie je blokovaná. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor aplikácie (identifikátor, ktorý aplikácia používa na registráciu so službou Microsoft Autoupdate), ktorá bola predtým blokovaná
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_queueinstall"></a>fbasilentupdate_queueinstall

Táto udalosť označuje, že aktualizácia sa zaradí do frontu na tichú inštaláciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_requiredappsclosed"></a>fbasilentupdate_requiredappsclosed

Táto udalosť zaznamenáva, keď sa zatvorí aplikácia s čakajúcou aktualizáciou. Označuje čas, kedy samotná inštalácia môže pokračovať. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a identifikátor zväzku aplikácie.
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_updateavailablenotification"></a>fbasilentupdate_updateavailablenotification

Táto udalosť označuje spustenie oznámenia o dostupnej aktualizácii. Musí sa zabezpečiť, aby sa po zistení aktualizácie spustil postup s výzvou na aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_userclicknotification"></a>fbasilentupdate_userclicknotification

Táto udalosť označuje, že používateľ klikol na sekciu obsahu v oznámení o dostupnej aktualizácii a spúšťa sa používateľské rozhranie služby Microsoft AutoUpdate. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_userselectinstalllater"></a>fbasilentupdate_userselectinstalllater

Táto udalosť označuje, že po zobrazení oznámenia o dostupnej aktualizácii sa používateľ rozhodol inštalovať neskôr. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="fbasilentupdate_userselectinstallnow"></a>fbasilentupdate_userselectinstallnow

Táto udalosť označuje, že po zobrazení oznámenia o dostupnej aktualizácii sa používateľ rozhodol inštalovať ihneď. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installdata_checkrunning"></a>installdata_checkrunning

Táto udalosť zaznamenáva výsledok kontroly medzi aplikáciami, ktoré sa majú nainštalovať, a tým, či bude pokus o inštaláciu pokračovať, na základe otvorenej aplikácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installdata_cleanup"></a>installdata_cleanup

Súbory balíka sa po nainštalovaní majú odstrániť. Táto udalosť zaznamenáva inštancie, v ktorých sa ich nepodarilo odstrániť. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov stiahnutého súboru a podrobnosti o chybe.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installedapp_invalidbundle"></a>installedapp_invalidbundle

Táto udalosť označuje, že službe Microsoft Autoupdate sa nepodarilo načítať informácie o zväzku pre registrovanú aplikáciu v danej ceste. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installedapp_invalidpreference"></a>installedapp_invalidpreference

Táto udalosť zaznamenáva prípady, v ktorých preferencie používateľa obsahujú neplatnú položku aplikácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installedapp_nilbundleid"></a>installedapp_nilbundleid

Táto udalosť zaznamenáva prípady, v ktorých identifikátor zväzku chýbal pre aplikáciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installedapp_nilbundlename"></a>installedapp_nilbundlename

Táto udalosť zaznamenáva prípady, v ktorých názov zväzku chýbal pre aplikáciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installstatus_codesign"></a>installstatus_codesign

Táto udalosť zaznamenáva stav binárneho súboru podpisu kódu operačného systému. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť
    
- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installstatus_daemon"></a>installstatus_daemon

Táto udalosť zaznamenáva stav démona služby Microsoft AutoUpdate. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informáciu o tom, či komponent Daemon existuje v očakávanom umiestnení a či má podpísaný kód.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installstatus_helper"></a>installstatus_helper

Táto udalosť zaznamenáva stav pomocného nástroja služby Microsoft AutoUpdate. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informáciu o tom, či komponent PrivilegedHelperTool existuje v očakávanom umiestnení a či má podpísaný kód.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installupdatestask_applaunched"></a>installupdatestask_applaunched

Táto udalosť označuje, že služba Microsoft Autoupdate zistila spustenie aplikácie pre blokovanú aktualizáciu, ale nenašla zodpovedajúci inštalačný program. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov spustenej aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installupdatestask_applaunchwithpendingupdate"></a>installupdatestask_applaunchwithpendingupdate

Táto udalosť označuje, že služba Microsoft Autoupdate zistila spustenie aplikácie pre aplikáciu s čakajúcou aktualizáciou. Spustená aplikácia sa ukončí. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installupdatestask_codesignverificationfail"></a>installupdatestask_codesignverificationfail

Táto udalosť označuje, že zlyhalo overenie podpisu kódu pre aktualizáciu aplikácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aktualizovanej aplikácie a kód zlyhania.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installupdatestask_codesignverificationstart"></a>installupdatestask_codesignverificationstart

Táto udalosť označuje, že sa spustilo overenie podpisu kódu pre aktualizáciu aplikácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aktualizovanej aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installupdatestask_codesignverificationsuccess"></a>installupdatestask_codesignverificationsuccess

Táto udalosť označuje úspešné overenie podpisu kódu pre aktualizáciu aplikácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aktualizovanej aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installupdatestask_failsilentinstall"></a>installupdatestask_failsilentinstall

Táto udalosť zaznamenáva zlyhania pri použití tichých aktualizácií a to, či ide o klonovanú alebo bežnú inštaláciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 
    
- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a typ aktualizácie.
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installupdatestask_multiplerelocatablepackage"></a>installupdatestask_multiplerelocatablepackage

Táto udalosť označuje, že služba Microsoft Autoupdate našla v stiahnutom manifeste viacero inštancií položky aplikácie pre daný balík aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie a názov aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installupdatestask_removeclone"></a>installupdatestask_removeclone

Táto udalosť označuje, že klon bol odstránený. Klon sa odstráni buď po dokončení procesu inštalácie na klon, alebo keď sa spustí nový proces a v zariadení sa nájde staršia klonovaná verzia. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aktualizácie, názov balíka aktualizácie a stav odstránenia klonu alebo podrobnosti o chybe.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installupdatestask_retryfail"></a>installupdatestask_retryfail

Táto udalosť označuje, že počas procesu opakovania inštalácie sa vyskytli chyby. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aktualizácie a to, či by sa inštalácia má vykonať prostredníctvom funkcie Inštalovať na klon.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installupdatestask_retryproxyerror"></a>installupdatestask_retryproxyerror

Táto udalosť zaznamenáva chyby komunikácie vnútri procesu (komunikácia s pomocným nástrojom služby MAU). Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aplikácie a podrobnosti o nahlásenej chybe proxy servera.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="installupdatestask_retryproxyerror"></a>installupdatestask_retryproxyerror

Táto udalosť zaznamenáva chyby komunikácie vnútri procesu (komunikácia s pomocným nástrojom služby MAU). Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aplikácie a podrobnosti o nahlásenej chybe proxy servera.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    

### <a name="installupdatestask_retryresponse"></a>installupdatestask_retryresponse

Táto udalosť zaznamenáva, že opakovaný pokus nebol úspešný. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aktualizácie, verziu aplikácie, názov balíka aktualizácie a to, či bola funkcia Inštalovať na klon aktívna, či inštalácia bola úspešná a prípadné chyby nahlásené pri zlyhaní.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installupdatestask_retrysuccess"></a>installupdatestask_retrysuccess

Táto udalosť zaznamenáva úspešnú inštaláciu aktualizácie po zopakovaní. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, názov aktualizácie, verziu aplikácie, názov balíka aktualizácie a to, či bola funkcia Inštalovať na klon aktívna.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="installupdatestask_setreopengui"></a>installupdatestask_setreopengui

Táto udalosť označuje, či nastavenie predvoľby opätovného otvorenia používateľského rozhrania po inštalácii bolo úspešné. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text označujúci úspešnosť operácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="msupdate_cli_eventhandler_applyupdates_appids"></a>msupdate_cli_eventhandler_applyupdates_appids

Táto udalosť označuje, že bol vydaný príkaz rozhrania príkazového riadka (CLI) na použitie aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje zoznam identifikátorov aplikácií, ktoré sa majú aktualizovať.
    
- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="msupdate_cli_eventhandler_config"></a>msupdate_cli_eventhandler_config

Táto udalosť označuje, že modul rozhrania príkazového riadka služby Microsoft Autoupdate prijal udalosť Apple na konfiguráciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="msupdate_cli_eventhandler_updates"></a>msupdate_cli_eventhandler_updates

Táto udalosť označuje, že modul rozhrania príkazového riadka služby Microsoft Autoupdate prijal udalosť Apple na zobrazenie zoznamu aktualizácií. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="msupdate_monitor_progress_downloaded"></a>msupdate_monitor_progress_downloaded

Táto udalosť označuje, že aktualizácie boli stiahnuté. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje zoznam stiahnutých aktualizácií

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="msupdate_monitor_progress_failure"></a>msupdate_monitor_progress_failure

Táto udalosť zaznamenáva zoznam aktualizácií vo fronte, ktoré sa nepodarilo použiť. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje zoznam aktualizácií.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="msupdate_monitor_progress_finished"></a>msupdate_monitor_progress_finished

Táto udalosť zaznamenáva zoznam aktualizácií vo fronte, ktoré sa úspešne nainštalovali. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje zoznam aktualizácií.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="msupdate_monitor_progress_queued"></a>msupdate_monitor_progress_queued

Táto udalosť zaznamenáva zoznam aktualizácií vo fronte. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje zoznam aktualizácií.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="optinnotificationaction"></a>Optinnotificationaction

Táto udalosť zaznamená reakciu používateľa na dialógové okno registrácie tichých aktualizácií. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje statický text, ktorý predstavuje výber používateľa pre automatické stiahnutie a inštaláciu.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="sauupdateinfoprovider"></a>sauupdateinfoprovider

Táto udalosť sa zaznamenáva vždy, keď v kolateráli chýba kľúč manifestu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje reťazec, ktorý sa používa na vyhľadanie umiestnenia alebo veľkosti aktualizácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatecore_appregistration"></a>updatecore_appregistration

Táto udalosť zaznamenáva pokusy o zaregistrovanie aplikácie a výsledok alebo dôvod. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikátor použitý na sledovanie aktivity aktualizácie, informáciu, či je predvoľba k dispozícii, informáciu, či ide o opätovnú registráciu, a informáciu, či sa vyžaduje registrácia.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatecore_loadinglaunchagent"></a>updatecore_loadinglaunchagent

Táto udalosť označuje, že sa načítava agent spustenia. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatecore_server_connectionfail"></a>updatecore_server_connectionfail

Táto udalosť zapisuje chyby, ktoré sa vyskytli pri kontaktovaní siete CDN. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie o názve servera, o tom, či je server platný a či je dostupný.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefilterhelper_cannotretrievebuilddate"></a>updatefilterhelper_cannotretrievebuilddate

Aktualizácie môžeme filtrovať prostredníctvom služby MAU len vtedy, keď ponúkaná aktualizácia nie je staršia ako určitý počet dní. Táto udalosť zaznamenáva, že sa nám nepodarilo načítať dátum z metaúdajov aplikácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefilterhelper_invalidresponsefromupdatefiltering"></a>updatefilterhelper_invalidresponsefromupdatefiltering

Aktualizácie môžeme filtrovať prostredníctvom služby MAU len vtedy, keď ponúkaná aktualizácia nie je staršia ako určitý počet dní. Táto udalosť zaznamenáva, že v metaúdajoch aplikácie chýba dátum. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 
    
- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefilterhelper_missingbuilddate"></a>updatefilterhelper_missingbuilddate

Aktualizácie môžeme filtrovať prostredníctvom služby MAU len vtedy, keď ponúkaná aktualizácia nie je staršia ako určitý počet dní. Táto udalosť zaznamenáva, že v metaúdajoch aplikácie chýba dátum. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefilterhelper_updatebypassedoldage"></a>updatefilterhelper_updatebypassedoldage

Aktualizácie môžeme filtrovať prostredníctvom služby MAU len vtedy, keď ponúkaná aktualizácia nie je staršia ako určitý počet dní. Táto udalosť zaznamenáva, že došlo k obídeniu služby z dôvodu starého dátumu aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_check_start"></a>updatefinder_check_start

Táto udalosť sa zaznamenáva vždy, keď sa spustí operácia kontroly aktualizácií. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť
    
- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie o aktualizáciách v ponuke, registrovaných aplikáciách a dočasnom umiestnení, do ktorého sa uložia stiahnuté súbory.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_check_status"></a>updatefinder_check_status

Táto udalosť agreguje stav operácie vyhľadávania aktualizácií (kanál od vyhľadávania až po sťahovanie). Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informácie o aktualizáciách v ponuke, registrovaných aplikáciách a dočasnom umiestnení, do ktorého sa uložia stiahnuté súbory.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_check_updatefound"></a>updatefinder_check_updatefound

Táto udalosť sa zaznamenáva vždy, keď sa pri vyhľadávaní aktualizácií nájdu aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_check_updatenotfound"></a>updatefinder_check_updatenotfound

Táto udalosť sa zaznamenáva vždy, keď sa pri vyhľadávaní aktualizácií neponúknu žiadne aktualizácie, pretože sa nenašli žiadne aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_check_uptodate"></a>updatefinder_check_uptodate

Táto udalosť sa zaznamenáva vždy, keď sa pri vyhľadávaní aktualizácií neponúknu žiadne aktualizácie, pretože všetky aplikácie sú aktuálne. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_offerupdates_minoscheckfail"></a>updatefinder_offerupdates_minoscheckfail

Táto udalosť sa zaznamenáva pri každom zablokovaní aktualizácie z dôvodu nespĺňania požiadaviek operačného systému. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje minimálnu požadovanú verziu operačného systému určenú v stiahnutom súbore manifestu.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_offerupdates_nullbundleforappid"></a>updatefinder_offerupdates_nullbundleforappid

Táto udalosť označuje, že službe Microsoft Autoupdate sa nepodarilo načítať informácie o zväzku pre identifikáciu aplikácie určenú v stiahnutom súbore manifestu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_offerupdates_updaterulematched"></a>updatefinder_offerupdates_updaterulematched

Táto udalosť označuje, že sa našla aktualizácia pre aplikáciu a základný stav. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu aplikácie a informácie o verzii zväzku.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="updatefinder_registeredapps"></a>updatefinder_registeredapps

Táto udalosť zaznamenáva aplikácie nainštalované, registrované alebo riadené službou MAU. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu aplikácie a informácie o verzii zväzku.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="updatefinder_suite_missingcollateral"></a>updatefinder_suite_missingcollateral

Aktualizácia balíka – táto udalosť sa zaznamenáva vždy, keď aktualizácia balíka nie je uplatniteľná z dôvodu chýbajúceho kolaterálu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – text, ktorý označuje povahu udalosti.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_suite_staleversion"></a>updatefinder_suite_staleversion

Aktualizácia balíka – táto udalosť sa zaznamenáva vždy, keď aktualizácia balíka nie je uplatniteľná z dôvodu príliš starej verzie základného stavu. Zaznamenáva sa verzia základného stavu a identifikátor AddId balíka. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov balíka.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_suite_updateapplicable"></a>updatefinder_suite_updateapplicable

Aktualizácia balíka – táto udalosť sa zaznamenáva vždy, keď aktualizácia balíka je uplatniteľná. Zaznamenáva sa verzia základného stavu a identifikátor AddId balíka. Zaznamenáva sa verzia základného stavu a identifikátor AddId balíka. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov, základný stav a verziu aktualizácie pre balík.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_suite_updatenotapplicabledefaultpath"></a>updatefinder_suite_updatenotapplicabledefaultpath

Aktualizácia balíka – táto udalosť sa zaznamenáva vždy, keď sa aktualizácia balíka neponúka, pretože všetky aplikácie balíka nie sú nainštalované v predvolenom umiestnení. Zaznamenáva sa verzia základného stavu a identifikátor AddId balíka. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov, základný stav a verziu aktualizácie pre balík.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="updatefinder_suite_updatenotapplicableversion"></a>updatefinder_suite_updatenotapplicableversion

Aktualizácia balíka – táto udalosť sa zaznamenáva vždy, keď sa aktualizácia balíka neponúka, pretože všetky aplikácie balíka nemajú rovnakú verziu základného stavu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov, základný stav a verziu aktualizácie pre balík.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_suite_updatenotoffered"></a>updatefinder_suite_updatenotoffered

Aktualizácia balíka – táto udalosť sa zaznamenáva vždy, keď sa aktualizácia balíka neponúka, pretože veľkosť balíka je vyššia ako jednotlivé aktualizácie. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov balíka.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatefinder_suite_updateoffered"></a>updatefinder_suite_updateoffered

Aktualizácia balíka – táto udalosť sa zaznamenáva vždy, keď sa ponúka aktualizácia balíka. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje názov, základný stav a verziu aktualizácie pre balík.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="updatemanager_checkupdate"></a>updatemanager_checkupdate

Táto udalosť zaznamenáva počet aktualizácií nájdených službou Microsoft Autoupdate počas vyhľadávania dostupných aktualizácií. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje počet nájdených dostupných aktualizácií.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="updatemanager_updatespending"></a>updatemanager_updatespending

Táto udalosť označuje, že sa našli aktualizácie a čakajú na inštaláciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje informáciu o tom, či je úloha spustená v hlavnom vlákne, a počet čakajúcich aktualizácií.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="webservices_checkforsilentupdates"></a>webservices_checkforsilentupdates

Táto udalosť označuje, že sa našli kandidáti na tichú aktualizáciu. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje počet nájdených aktualizácií a identifikátor aplikácie.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="webservices_deltaupdater"></a>webservices_deltaupdater

Táto udalosť zaznamenáva interakcie medzi kódom klienta a bránou funkcií, ktorá určuje, či má klient umožniť aktualizácie delta. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje odpoveď z webových služieb a typ aktualizačného programu, ktorý sa má použiť.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="webservices_serviceaction"></a>webservices_serviceaction

Táto udalosť zaznamenáva chyby vyplývajúce z neočakávanej odpovede webovej služby. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje podrobnosti o akcii prichádzajúcej z webových služieb.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="webservices_serviceaction"></a>webservices_serviceaction

Táto udalosť zaznamenáva chyby vyplývajúce z neočakávanej odpovede webovej služby. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje podrobnosti o akcii prichádzajúcej z webových služieb.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie


### <a name="webservices_serviceresponse"></a>webservices_serviceresponse

Táto udalosť zaznamenáva požiadavky pre službu MAU, časy odozvy a chyby. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje ID požiadavky, názov aplikácie, čas odozvy a/alebo kód stavu.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

    
### <a name="webservices_silentupdate"></a>webservices_silentupdate

Táto udalosť zaznamenáva požiadavky na kontrolu pravidiel použiteľnosti vynútenej aktualizácie, t. j. v dôsledku určitého závažného problému je potrebné, aby používateľ prešiel zo zostavy N na zostavu N+1. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje ID požiadavky, názov aplikácie, čas odozvy a/alebo kód stavu.

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie



### <a name="webservices_webcontent"></a>webservices_webcontent

Táto udalosť zaznamenáva požiadavky a odpovede prijaté do webových služieb. Táto udalosť sa používa na zaistenie, že proces aktualizácie funguje podľa očakávaní, a na pomoc pri riešení chýb.
 
Zhromažďujú sa tieto polia:

- **App** – proces aplikácie odosielajúci udalosť

- **AppInfo_Language** – jazyk, v ktorom je aplikácia spustená

- **AppVersionLong** – verzia aplikácie

- **Channel** – preferencia pre cieľovú skupinu

- **Device_NetworkCountry** – krajina zariadenia (na základe IP adresy)

- **DeviceID** – identifikátor zariadenia

- **DeviceInfo_Model** – hardvérový model zariadenia

- **DeviceInfo_NetworkType** – typ siete (Wi-Fi, káblová, neznáma)

- **DeviceInfo_OsBuild** – verzia operačného systému

- **Event_ReceivedTime** – čas prijatia telemetrie

- **EventInfo_Name** – názov udalosti telemetrie, ktorá sa práve zaznamenáva

- **EventInfo_Time** – čas výskytu zaznamenanej udalosti 

- **HowTocheck** – preferencia pre kontrolu aktualizácií

- **Payload** – obsahuje identifikáciu volajúceho webových služieb

- **PipelineInfo_ClientCountry** – krajina zariadenia (na základe IP adresy)

- **PipelineInfo_ClientIp** – prvé 3 oktety IP adresy

- **SessionId** – identifikátor relácie

## <a name="onenote-sync-events"></a>Udalosti synchronizácie OneNotu

### <a name="officeonenotestoragenotebooksyncresult"></a>Office.OneNote.Storage.NotebookSyncResult
 
Táto udalosť zaznamenáva výsledok synchronizácie poznámkového bloku. Používa sa na zistenie počtu jedinečných cieľov synchronizácie vo výpočte skóre synchronizácie OneNotu.
 
Zhromažďujú sa tieto polia:

- **CachedError_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby vo vyrovnávacej pamäti a/alebo dôvodu, prečo sa vyskytla.

- **CachedError_Description** – popis chyby vo vyrovnávacej pamäti

- **CachedError_Tag** – označuje, kde v kóde došlo k chybe vo vyrovnávacej pamäti

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

- **SectionError_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby synchronizácie sekcie a/alebo dôvodu, prečo sa vyskytla

- **SectionError_Description** – popis chyby synchronizácie sekcie

- **SectionError_Tag** – označuje, kde v kóde došlo k chybe synchronizácie sekcie

- **SectionError_Type** – typ chyby synchronizácie sekcie, napríklad Win32Error atď

- **Success** – označuje, či je synchronizácia poznámkového bloku úspešná alebo nie.

- **SyncDestinationType** – typ cieľa synchronizácie, ako je OneDrive alebo SharePoint Online.

- **SyncId** – číslo jedinečné pre každú synchronizáciu poznámkového bloku.

- **SyncWasFirstInSession** – označuje, či je táto synchronizácia prvou synchronizáciou v aktuálnej relácii.

- **SyncWasUserInitiated** – označuje, či je táto synchronizácia iniciovaná používateľom alebo nie.

- **TenantId** – ID nájomníka SharePointu.

- **TimeSinceLastAttemptedSync** – čas od posledného pokusu o synchronizáciu poznámkového bloku.

- **TimeSinceLastSuccessfulSync** – čas od poslednej úspešnej synchronizácie poznámkového bloku.

### <a name="officeonenotestoragerealtimewebsocketsessioninfo"></a>Office.OneNote.Storage.RealTime.WebSocketSessionInfo
 
Táto udalosť zaznamenáva výsledok synchronizácie protokolu WebSocket pre modernú synchronizáciu obsahu strany aj modernú synchronizáciu hierarchie OneNotu. Používa sa na zistenie počtu jedinečných cieľov synchronizácie vo výpočte skóre synchronizácie OneNotu. Používa sa aj pre tabuľu výkonu modernej synchronizácie OneNotu.
 
Zhromažďujú sa tieto polia:
 
- **CloseReason** – dôvod zavretia protokolu WebSocket, napr. nezvyčajné zatvorenie a pod.

- **DataIsFreshCount** – počet úspešných žiadostí typu pull v relácii protokolu WebSocket

- **DeviceSessionId** – ID relácie zariadenia

- **DownloadCount** – počet stiahnutí v relácii protokolu WebSocket

- **Error** – je v podstate Exception_Type + Exception_Description + Exception_Code + Exception_Tag

- **Exception_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby a/alebo dôvodu, prečo sa vyskytla

- **Exception_Description** – popis chyby

- **Exception_Tag** – označuje, kde v kóde došlo k chybe

- **Exception_Type** – typ chyby, napríklad Win32Error atď.

- **FirstUpdateSize** – dĺžka hlásenia prvej aktualizácie

- **HasError** – označuje, či sa počas relácie protokolu WebSocket vyskytla chyba 

- **IsEducationNotebook** – označuje, či aktuálny poznámkový blok je vzdelávací poznámkový blok alebo nie

- **IsHierarchyResource** – označuje, či aktuálny zdroj je strana alebo sekcia

- **NotebookId** – ID onenotového poznámkového bloku

- **OperationWithError** – označuje, v ktorej operácii sa chyba vyskytla, ako je napríklad WebSocket.Close, WebSocket.Open atď.

- **ResourceId** – ID zdroja strany alebo sekcie OneNotu

- **SectionId** – ID sekcie OneNotu

- **ServerSessionId** – ID relácie použité na koreláciu požiadavky protokolu WebSocket na onenote.com

- **SessionDurationInMs** – trvanie relácie protokolu WebSocket v milisekundách

- **TenantId** – ID nájomníka SharePointu

- **TimeToFirstUpdateInMs** – čas v milisekundách trvania prijatia prvej aktualizácie zo servera po vytvorení relácie protokolu WebSocket

- **UploadAckCount** – počet potvrdení pre nahrávanie v relácii protokolu WebSocket

- **WebUrl** – webová URL adresa s odstránenými osobnými údjmi 

### <a name="officeonenotestoragesectionsyncresult"></a>Office.OneNote.Storage.SectionSyncResult
 
Táto udalosť zaznamenáva výsledok synchronizácie sekcie. Používa sa na zistenie počtu jedinečných cieľov synchronizácie vo výpočte skóre synchronizácie OneNotu. Používa sa aj pre tabuľu výkonu modernej synchronizácie OneNotu.
 
Zhromažďujú sa tieto polia:

- **Error_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby a/alebo dôvodu, prečo sa vyskytla

- **Error_Description** – popis chyby

- **Error_Tag** – označuje, kde v kóde došlo k chybe

- **Error_Type** – typ chyby, napríklad Win32Error atď.

- **ErrorLast** – kód naposledy zobrazenej chyby 

- **ExecutionTime** – čas v milisekundách, ktorý bol potrebný na replikovanie sekcie

- **InitialReplicationInSession** – označuje, či je táto replikácia prvou replikáciou poznámkového bloku po otvorení alebo nie

- **IsAttachedViaShortcut** – označuje, či je sekcia pripojená cez odkaz alebo nie

- **IsBackgroundSync** – označuje, či ide o synchronizáciu na pozadí alebo nie

- **IsEncrypted** – označuje, či je sekcia šifrovaná alebo nie

- **IsErrorSuppressed** – označuje, či je táto chyba potlačená alebo nie 

- **IsErrorTransient** – označuje, či je táto chyba krátkodobá alebo nie

- **IsErrorUnexpected** – označuje, či je táto chyba neočakávaná alebo nie

- **IsUsingRealtimeSync** – označuje, či synchronizácia sekcie používa modernú synchronizáciu obsahu strany alebo nie

- **NotebookId** – ID poznámkového bloku

- **NotebookPath** – URL adresa poznámkového bloku s odstránenými osobnými údajmi

- **SectionPath** – URL adresa sekcie s odstránenými osobnými údajmi

- **SectionReplicatingIsOutbound** – označuje, či je táto replikácia odchádzajúca alebo nie

- **SectionReplicatingIsSameIdentity** – označuje, či je táto replikácia založená na rovnakej identifikácii súboru alebo nie

- **SectionResourceId** – ID zdroja sekcie OneNotu

- **Success** – označuje, či je synchronizácia sekcie úspešná alebo nie

- **SyncDestinationType** – typ cieľa synchronizácie, ako je OneDrive alebo SharePoint Online

- **SyncId** – číslo jedinečné pre každú synchronizáciu sekcie

- **SyncWasFirstInSession** – označuje, či je táto synchronizácia prvou synchronizáciou v aktuálnej relácii

- **SyncWasUserInitiated** – označuje, či je táto synchronizácia iniciovaná používateľom alebo nie

- **TenantId** – ID nájomníka SharePointu

- **UnmappedGosid** – ID sekcie pred použitím identifikátora GUID priradenia


### <a name="officeonenotestoragesyncscore"></a>Office.OneNote.Storage.SyncScore
 
Táto udalosť zaznamenáva všetky negatívne faktory pri synchronizácii, ktoré sa používateľom zobrazujú. Používa sa na výpočet skóre synchronizácie OneNotu, čo je dôležitá metrika na vyhodnotenie fungovania synchronizácie používateľov OneNotu.
 
Zhromažďujú sa tieto polia:

- **AutoShowSyncStatus** – označuje, či sa stav synchronizácie zobrazuje automaticky alebo nie

- **Cause** – označuje, čo spôsobilo presun strán/sekcií OneNotu do nesprávnych sekcií

- **Context** – enumerácia, ktorá kategorizuje, čo sa používateľ pokúša urobiť, napr. premenovať sekciu, znova otvoriť poznámkový blok atď.

- **Error_Code** – číselný alebo alfanumerický kód, ktorý sa používa na určenie povahy chyby a/alebo dôvodu, prečo sa vyskytla

- **Error_Description** – popis chyby

- **Error_Tag** – označuje, kde v kóde došlo k chybe

- **Error_Type** – typ chyby, napríklad Win32Error atď.

- **ErrorText** – text chyby zobrazený v používateľskom rozhraní

- **Explanation** – vysvetľuje, aký druh čakajúcich odchádzajúcich zmien je potrebné premiestniť do nesprávnych sekcií

- **fishbowlType** – druh akvária, napr. akvárium strany, akvárium sekcie atď.

- **IDS** – celočíselný identifikátor pre text zobrazený v používateľskom rozhraní

- **idsFishbowl** – celočíselný identifikátor pre chybu akvária zobrazenú v používateľskom rozhraní

- **IsUsingRealtimeHierarchySync** – označuje, či sa používa moderná synchronizáciu hierarchie alebo nie

- **NotebookId** – ID poznámkového bloku

- **PageSyncUIState** – reťazec stavu synchronizácie strany, napr. UpToDate, Syncing, SaveOffline, SyncError atď. 

- **ServerGosid** – ID zdroja pre novovytvorenú konfliktnú stranu

- **Source** – enumerácia, ktorá označuje, ktorá udalosť spustila používateľské rozhranie, t. j. vytvorenie nového obrazu redx, chyba synchronizácie v používateľskom rozhraní synchronizácie, zobrazené dialógové okno chyby atď.


## <a name="services-configuration-events"></a>Udalosti služby Services Configuration

Služba Services Configuration nezhromažďuje žiadne požadované diagnostické údaje služieb.

## <a name="telemetry-events"></a>Udalosti služby telemetrie

### <a name="office_firstrun_apple_telemetryoptin"></a>Office_FirstRun_Apple_TelemetryOptIn

Táto udalosť sa zhromažďuje pre aplikácie balíka Office spustené v rámci platforiem Apple. Udalosť sa používa na sledovanie stavu postupu výslovného súhlasu s telemetriou pri prvom spustení. Zhromažďujeme kód, ktorý označuje, aký typ možností zhromažďovania diagnostických údajov používateľ vybral.

Zhromažďujú sa tieto polia:

 - **Data_EventId** – Kód označujúci preferenciu zhromažďovania diagnostických údajov vybratú používateľom.


### <a name="officesystemidentitychanged"></a>Office.System.IdentityChanged

Informácie o identite používateľa požadované na splnenie žiadostí dotknutých osôb.

Zhromažďujú sa tieto polia:

  - **IdentityChanged** – vždy pravda. Identita sa zmenila.

  - **TimerDetectedChange** – či sa zmena zistila pravidelne časovým pingom.

### <a name="officesystemprivacyfallbacktosettingsstore"></a>Office.System.PrivacyFallbackToSettingsStore

Používa sa na určenie, či sa vyskytnú zlyhania pri čítaní nastavení ochrany osobných údajov používateľa z roamingového ukladacieho priestoru.

Zhromažďujú sa tieto polia:

  - **Tag** – značka kódu označujúca, ktoré nastavenie sa vrátilo späť do ukladacieho priestoru nastavení.

### <a name="officesystemsessiondatao365"></a>Office.System.SessionDataO365

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **AppId** – identifikátor aplikácie balíka Office, ktorej sa tieto údaje týkajú.

  - **ApplicationArchitecture** – pre ktorú architektúru procesora je Office určený.

  - **AppVersionBuild** – verzia zostavy aplikácie balíka Office.

  - **AppVersionMajor** – hlavná verzia aplikácie balíka Office.

  - **AppVersionMinor** – vedľajšia verzia aplikácie balíka Office.

  - **AppVersionUpdate** – revízia zostavy aplikácie balíka Office.

  - **CollectorVersion** – identifikátor verzie pre logiku kolekcie klienta.

  - **DeviceHash** – jednosmerný hash identifikátora operačného systému zariadenia.

  - **DeviceName** – názov zariadenia, v ktorom je Office spustený.

  - **Domain** – doména zariadenia, v ktorom je Office spustený.

  - **IsCeip** – či inštalácia balíka Office bola zaregistrovaná v zrušenom programe zvyšovania spokojnosti zákazníkov.

  - **IsDebug** – či ide o zostavu ladenia balíka Office.

  - **IsImmersive** – či aplikácia balíka Office je typu Universal Windows alebo Immersive.

  - **IsLaptop** – či zariadenie, v ktorom je Office spustený, je notebook.

  - **IsMicrosoftInternal** – či používateľ systému Windows, ktorý má spustený Office, je zamestnancom spoločnosti Microsoft.

  - **IsO365** – či je inštalácia balíka Office súčasťou zrušeného programu Outlook 365.

  - **IsTablet** – či zariadenie, v ktorom je Office spustený, je tablet.

  - **IsTerminalServer** – pravda/nepravda, či ide o klienta terminálového servera

  - **MaxMemory** – Maximálne množstvo pamäte RAM dostupné v zariadení so spusteným balíkom Office.

  - **OsArchitecture** – architektúra procesora, pre ktorú je určený operačný systém so spusteným balíkom Office.

  - **OsVersionBuild** – verzia zostavy operačného systému.

  - **OsVersionMajor** – hlavná verzia operačného systému.

  - **OsVersionMinor** – vedľajšia verzia operačného systému.

  - **OsVersionUpdate** – revízia zostavy operačného systému.

  - **ProcessFileName** – názov spustiteľného súboru spustenej aplikácie.

  - **ProcessorArchitecture** – na ktorej architektúre procesora je Office spustený.

  - **ProcessorFrequency** – rýchlosť procesora v zariadení, v ktorom je Office spustený, v MHz.

  - **SessionStart** – čas, kedy sa začal proces spustenia balíka Office.

  - **UserName** – meno konta so spusteným balíkom Office.

### <a name="officesystemsystemhealthcoremetadata"></a>Office.System.SystemHealthCoreMetadata

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **AppBuild** – verzia zostavy aplikácie balíka Office.

  - **AppBuildRevision** – revízia zostavy aplikácie balíka Office.

  - **AppMajorVer** – hlavná verzia aplikácie balíka Office.

  - **AppMinorVer** – vedľajšia verzia aplikácie balíka Office.

  - **CID** – pseudonymizovaná identita používateľa

  - **CollectibleClassifications** – množina klasifikácií údajov, ktoré je možné zhromažďovať.

  - **CollectionTime** – čas, kedy sa metaúdaje zhromaždili.

  - **DeviceManufacturer** – výrobca zariadenia, v ktorom je Office spustený.

  - **DeviceModel** – model zariadenia, v ktorom je Office spustený.

  - **FirstRunTime** – čas prvého spustenia niektorej aplikácie balíka Office.

  - **IsClickToRunInstall** – či bola aplikácia balíka Office nainštalovaná pomocou technológie Klikni a spusti.

  - **IsDebug** – či ide o zostavu ladenia balíka Office.

  - **IsLabMachine** – či je balík Office spustený v laboratóriu spoločnosti Microsoft.

  - **IsLaptop** – či zariadenie, v ktorom je Office spustený, je notebook.

  - **IsMsftInternal** – či používateľ systému Windows, ktorý má spustený Office, je zamestnancom spoločnosti Microsoft.

  - **IsSubscription** – či je aplikácia balíka Office nainštalovaná v rámci licencie s predplatným.

  - **IsTablet** – či zariadenie, v ktorom je Office spustený, je tablet.

  - **IsTerminalServer** – či je balík Office spustený na terminálovom serveri.

  - **MsoAppId** – identifikátor aplikácie balíka Office, ktorej sa tieto údaje týkajú.

  - **OfficeArchitectureText** – pre ktorú architektúru procesora je Office určený.

  - **OsBuild** – verzia zostavy operačného systému.

  - **OsBuildRevision** – revízia zostavy operačného systému.

  - **OSEnvironment** – identifikátor prostredia, v ktorom je Office spustený.

  - **OsMajorVer** – hlavná verzia operačného systému.

  - **OsMinorVer** – vedľajšia verzia operačného systému.

  - **OSVersionString** – verzia operačného systému ako reťazec.

  - **ProcessorArchitecture** – na ktorej architektúre procesora je Office spustený.

  - **ProcessorCount** – počet procesorov v zariadení, v ktorom je Office spustený.

  - **ProcSpeedMHz** – rýchlosť procesora v zariadení, v ktorom je Office spustený, v MHz.

  - **RamMB** – množstvo pamäte RAM dostupnej v zariadení, v ktorom je Office spustený.

  - **SqmUserId** – náhodný identifikátor inštalácie balíka Office.

### <a name="officesystemsystemhealthdesktopsessionlifecycleandheartbeat"></a>Office.System.SystemHealthDesktopSessionLifecycleAndHeartbeat

Poskytuje informácie o metrike stavu systému.

Zhromažďujú sa tieto polia:

  - **InstallMethod** – či bola aktuálna zostava balíka Office inovovaná zo staršej zostavy, vrátená na staršiu zostavu alebo nanovo nainštalovaná.

  - **PreviousBuild** – verzia balíka Office, na ktorú bola táto zostava bola inovovaná alebo z ktorej bola vrátená na staršiu verziu.

  - **State** – stav, na ktorý sa relácia zmenila.

  - **Time** – čas, keď sa zmenil stav relácie.

### <a name="officesystemsystemhealthessentialidentitycount"></a>Office.System.SystemHealthEssentialIdentityCount

Zhromažďuje počet identít prihláseného používateľa

Zhromažďujú sa tieto polia:

  - **AllIdentityCount** – počet všetkých identít

  - **ValidIdentityCount** – počet overených identít

### <a name="officesystemsystemhealthessentialmetadataallidentities"></a>Office.System.SystemHealthEssentialMetadataAllIdentities

Monitoruje stav kont rozpoznaných balíkom Office v tejto relácii. Používa sa na izolovanie zlyhania na typ prihlásenia konta, ak je zlyhanie špecifické pre typ.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – čas, kedy sa zhromaždili informácie o identite.

  - **IdentityType** – typ overovania alebo konta

  - **IdentityUniqueId** – pseudonymizovaný identifikátor identity

  - **IdentityUniqueIdHashed** – jednosmerný hash jedinečného identifikátora identity

### <a name="officesystemsystemhealthmetadataapplicationadditional"></a>Office.System.SystemHealthMetadataApplicationAdditional

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **Alias** – ak používateľ, ktorý má spustený Office, je zamestnancom spoločnosti Microsoft, jeho interný podnikový alias.

  - **AppBuild** – verzia zostavy aplikácie balíka Office.

  - **AppBuildRevision** – revízia zostavy aplikácie balíka Office.

  - **AppMajorVer** – hlavná verzia aplikácie balíka Office.

  - **AppMinorVer** – vedľajšia verzia aplikácie balíka Office.

  - **CID** – pseudonymizovaná identita používateľa

  - **CollectibleClassifications** – množina klasifikácií údajov, ktoré je možné zhromažďovať.

  - **DeviceManufacturer** – výrobca zariadenia, v ktorom je Office spustený.

  - **DeviceModel** – model zariadenia, v ktorom je Office spustený.

  - **DeviceProcessorModel** – model procesora zariadenia, v ktorom je Office spustený.

  - **DigitizerInfo** – informácie o digitalizátore pripojenom k zariadeniu, v ktorom je Office spustený.

  - **DomainName** – názov domény, do ktorej je pripojené zariadenie, v ktorom je Office spustený (ak je pripojené).

  - **FirstRunTime** – čas prvého spustenia niektorej aplikácie balíka Office.

  - **HorizontalResolution** – vodorovné rozlíšenie obrazovky.

  - **IsDebug** – či ide o zostavu ladenia balíka Office.

  - **IsImmersive** – či aplikácia balíka Office je typu Universal Windows alebo Immersive.

  - **IsJoinedToDomain** – či zariadenie, v ktorom je Office spustený, je pripojené do domény.

  - **IsLabMachine** – či je balík Office spustený v laboratóriu spoločnosti Microsoft.

  - **IsLaptop** – či zariadenie, v ktorom je Office spustený, je notebook.

  - **IsMsftInternal** – či používateľ systému Windows, ktorý má spustený Office, je zamestnancom spoločnosti Microsoft.

  - **IsOEMInstalled** – či spustená aplikácia balíka Office bola nainštalovaná výrobcom OEM.

  - **IsOEMInstalled** – či spustená aplikácia balíka Office bola nainštalovaná výrobcom OEM.

  - **IsSubscription** – či je aplikácia balíka Office nainštalovaná v rámci licencie s predplatným.

  - **MsoAppId** – identifikátor aplikácie balíka Office, ktorej sa tieto údaje týkajú.

  - **NumProcPhysCores** – počet fyzických jadier procesora.

  - **OfficeBuild** – verzia zostavy zdieľaných knižníc balíka Office.

  - **OfficeBuildRevision** – verzia revízie zostavy zdieľaných knižníc balíka Office.

  - **OfficeMajorVer** – hlavná verzia zdieľaných knižníc balíka Office.

  - **OfficeMinorVer** – vedľajšia verzia zdieľaných knižníc balíka Office.

  - **OsBuild** – verzia zostavy operačného systému.

  - **OsBuildRevision** – revízia zostavy operačného systému.

  - **OsMajorVer** – hlavná verzia operačného systému.

  - **OsMinorVer** – vedľajšia verzia operačného systému.

  - **PowerPlatformRole** – identifikátor roly počítača zariadenia, v ktorom je Office spustený, preferovanej výrobcom OEM.

  - **ProcessFileName** – názov spustiteľného súboru spustenej aplikácie.

  - **ProcessorCount** – počet procesorov v zariadení, v ktorom je Office spustený.

  - **RamMB** – množstvo pamäte RAM dostupnej v zariadení, v ktorom je Office spustený.

  - **SqmUserId** – náhodný identifikátor inštalácie balíka Office.

  - **StudyId** – identifikátor štúdie metriky kvality softvéru.

  - **VerticalResolution** – zvislé rozlíšenie obrazovky.

  - **WinUserActType** – či používateľ systému Windows, ktorý má spustený Office, je lokálny správca, používateľ typu power user alebo bežný používateľ.

### <a name="officesystemsystemhealthmetadataapplicationandlanguage"></a>Office.System.SystemHealthMetadataApplicationAndLanguage

Metaúdaje sú požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **AppBuild** – verzia zostavy aplikácie balíka Office.

  - **AppBuildRevision** – revízia zostavy aplikácie balíka Office.

  - **AppMajorVer** – hlavná verzia aplikácie balíka Office.

  - **AppMinorVer** – vedľajšia verzia aplikácie balíka Office.

  - **AppState** – identifikátor stavu, v ktorom sa aplikácia balíka Office nachádza.

  - **Click2RunPackageVersionBuild** – verzia zostavy inštalačného balíka Klikni a spusti.

  - **Click2RunPackageVersionMajor** – hlavná verzia inštalačného balíka Klikni a spusti.

  - **Click2RunPackageVersionMinor** – vedľajšia verzia inštalačného balíka Klikni a spusti.

  - **Click2RunPackageVersionRevision** – revízia zostavy inštalačného balíka Klikni a spusti.

  - **DistributionChannel** – kanál, cez ktorý bol balík Office distribuovaný.

  - **InstallType** – identifikátor spôsobu inštalácie balíka Office.

  - **IsClickToRunInstall** – či bola aplikácia balíka Office nainštalovaná pomocou technológie Klikni a spusti.

  - **IsDebug** – či ide o zostavu ladenia balíka Office.

  - **IsImmersive** – či aplikácia balíka Office je typu Universal Windows alebo Immersive.

  - **IsMsftInternal** – či používateľ systému Windows, ktorý má spustený Office, je zamestnancom spoločnosti Microsoft.

  - **IsOEMInstalled** – či spustená aplikácia balíka Office bola nainštalovaná výrobcom OEM.

  - **IsOEMInstalled** – či spustená aplikácia balíka Office bola nainštalovaná výrobcom OEM.

  - **IsSubscription** – či je aplikácia balíka Office nainštalovaná v rámci licencie s predplatným.

  - **MsoAppId** – identifikátor aplikácie balíka Office, ktorej sa tieto údaje týkajú.

  - **OfficeArchitectureText** – pre ktorú architektúru procesora je Office určený.

  - **OfficeBuild** – verzia zostavy zdieľaných knižníc balíka Office.

  - **OfficeBuildRevision** – verzia revízie zostavy zdieľaných knižníc balíka Office.

  - **OfficeMajorVer** – hlavná verzia zdieľaných knižníc balíka Office.

  - **OfficeMinorVer** – vedľajšia verzia zdieľaných knižníc balíka Office.

  - **OfficeMuiCount** – počet nainštalovaných jazykových balíkov balíka Office.

  - **OfficeSkuLanguage** – jazyk nainštalovanej jednotky SKU.

  - **OfficeSkuLanguageTag** – jazyk nainštalovanej jednotky SKU.

  - **OfficeUiLang** – jazyk používateľského rozhrania aplikácie balíka Office.

  - **OfficeUiLangTag** – jazyk používateľského rozhrania aplikácie balíka Office.

  - **ProcessFileName** – názov spustiteľného súboru spustenej aplikácie.

  - **SqmAppId** – identifikátor aplikácie balíka Office, ktorej sa tieto údaje týkajú.

### <a name="officesystemsystemhealthmetadatadelayedlogin"></a>Office.System.SystemHealthMetadataDelayedLogin

Informácie o identite používateľa požadované na splnenie žiadostí dotknutých osôb.

Zhromažďujú sa tieto polia:

  - **CID** – pseudonymizovaná identita používateľa

### <a name="officesystemsystemhealthmetadatadevice"></a>Office.System.SystemHealthMetadataDevice

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – čas, kedy sa metaúdaje zhromaždili.

  - **ComputerSystemProductUuidHash** – jednosmerný hash identifikátora UUID základnej dosky.

  - **DeviceClass** – identifikátor typu zariadenia, v ktorom je Office spustený.

  - **DeviceMake** – identifikátor rodiny hardvérového systému zariadenia, v ktorom je Office spustený.

  - **DeviceManufacturer** – výrobca zariadenia, v ktorom je Office spustený.

  - **DeviceModel** – model zariadenia, v ktorom je Office spustený.

  - **DigitizerInfo** – informácie o digitalizátore pripojenom k zariadeniu, v ktorom je Office spustený.

  - **IsLaptop** – či zariadenie, v ktorom je Office spustený, je notebook.

  - **IsTablet** – či zariadenie, v ktorom je Office spustený, je tablet.

  - **LicensingACID** – identifikátor licencovania inštalácie balíka Office.

  - **MachineName** – názov zariadenia, v ktorom je Office spustený.

  - **NumProcPhysCores** – počet fyzických jadier procesora.

  - **NumProcShareSingleCache** – počet procesorov zdieľajúcich jednu vyrovnávaciu pamäť v zariadení, v ktorom je Office spustený.

  - **NumProcShareSingleCore** – počet procesorov na fyzické jadro v zariadení, v ktorom je Office spustený.

  - **OlsLicenseId** – identifikátor licenčnej služby inštalácie balíka Office.

  - **Platform** – identifikátor prostredia, v ktorom je Office spustený.

  - **PowerPlatformRole** – identifikátor roly počítača zariadenia, v ktorom je Office spustený, preferovanej výrobcom OEM.

  - **ProcessorCount** – počet procesorov v zariadení, v ktorom je Office spustený.

  - **ProcSpeedMHz** – rýchlosť procesora v zariadení, v ktorom je Office spustený, v MHz.

  - **ProcType** – architektúra procesora.

  - **ProcTypeText** – typ procesora v zariadení, v ktorom je Office spustený.

  - **RamMB** – množstvo pamäte RAM dostupnej v zariadení, v ktorom je Office spustený.

  - **SusClientId** – identifikátor služby Windows Update zariadenia, v ktorom je Office spustený.

  - **SystemFamily** – identifikátor rodiny hardvérového systému zariadenia, v ktorom je Office spustený.

  - **SystemSKU** – identifikátor jednotky SKU hardvérového systému zariadenia, v ktorom je Office spustený.

  - **SysVolFreeSpaceMB** – množstvo voľného miesta dostupného v systémovom zväzku v megabajtoch.

  - **SysVolSizeMB** – veľkosť systémového zväzku v megabajtoch.

  - **WindowErrorReportingMachineId** – identifikátor počítača priradený technológiou hlásenia chýb systému Windows zariadeniu, v ktorom je Office spustený.

  - **WindowSqmMachineId** – identifikátor počítača priradený systémom Windows zariadeniu, v ktorom je Office spustený.

### <a name="officesystemsystemhealthmetadatadeviceconsolidated"></a>Office.System.SystemHealthMetadataDeviceConsolidated

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **BootDiskType** – disk alebo SSD

  - **ComputerSystemProductUuidHash** – jednosmerný hash identifikátora UUID základnej dosky.

  - **DeviceClass** – identifikátor typu zariadenia, v ktorom je Office spustený.

  - **DeviceManufacturer** – výrobca zariadenia, v ktorom je Office spustený.

  - **DeviceModel** – model zariadenia, v ktorom je Office spustený.

  - **DeviceProcessorModel** – model procesora zariadenia, v ktorom je Office spustený.

  - **DigitizerInfo** – informácie o digitalizátore pripojenom k zariadeniu, v ktorom je Office spustený.

  - **HasSpectreFix** – či procesor zariadenia, v ktorom je Office spustený, má opravu Spectre.

  - **IsLaptop** – či zariadenie, v ktorom je Office spustený, je notebook.

  - **IsTablet** – či zariadenie, v ktorom je Office spustený, je tablet.

  - **MachineName** – názov zariadenia, v ktorom je Office spustený.

  - **NumProcPhysCores** – počet fyzických jadier procesora.

  - **NumProcShareSingleCache** – počet procesorov zdieľajúcich jednu vyrovnávaciu pamäť v zariadení, v ktorom je Office spustený.

  - **NumProcShareSingleCore** – počet procesorov na fyzické jadro v zariadení, v ktorom je Office spustený.

  - **Platform** – identifikátor prostredia, v ktorom je Office spustený.

  - **PowerPlatformRole** – identifikátor roly počítača zariadenia, v ktorom je Office spustený, preferovanej výrobcom OEM.

  - **PowerPlatformRole** – identifikátor roly počítača zariadenia, v ktorom je Office spustený, preferovanej výrobcom OEM.

  - **ProcessorCount** – počet procesorov v zariadení, v ktorom je Office spustený.

  - **ProcSpeedMHz** – rýchlosť procesora v zariadení, v ktorom je Office spustený, v MHz.

  - **ProcType** – architektúra procesora.

  - **ProcTypeText** – typ procesora v zariadení, v ktorom je Office spustený.

  - **RamMB** – množstvo pamäte RAM dostupnej v zariadení, v ktorom je Office spustený.

  - **SusClientId** – identifikátor služby Windows Update zariadenia, v ktorom je Office spustený.

  - **SysVolFreeSpaceMB** – množstvo voľného miesta dostupného v systémovom zväzku v megabajtoch.

  - **SysVolSizeMB** – veľkosť systémového zväzku v megabajtoch.

  - **SysVolSizeMB** – veľkosť systémového zväzku v megabajtoch.

  - **WindowErrorReportingMachineId** – identifikátor počítača priradený technológiou hlásenia chýb systému Windows zariadeniu, v ktorom je Office spustený.

  - **WindowSqmMachineId** – identifikátor počítača priradený systémom Windows zariadeniu, v ktorom je Office spustený.

### <a name="officesystemsystemhealthmetadataoperatingsystem"></a>Office.System.SystemHealthMetadataOperatingSystem

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – čas, kedy bola táto udalosť zaradená do frontu na nahratie

  - **IsTerminalServer** – pravda/nepravda, či ide o klienta terminálového servera

  - **OsBuild** – verzia zostavy operačného systému.

  - **OsBuildRevision** – revízia zostavy operačného systému.

  - **OSEnvironment** – Windows, iOS, Mac, Android atď.

  - **OsMajorVer** – hlavná verzia operačného systému.

  - **OsMinorVer** – vedľajšia verzia operačného systému.

  - **OSSDKVersionCode** – identifikátor verzie súpravy SDK operačného systému.

  - **OsSku** – jednotka SKU operačného systému.

  - **OsSuite2** – identifikátor balíka operačného systému.

  - **OSVersionString** – identifikátor verzie operačného systému.

  - **ServicePackMajorVer** – hlavná verzia balíka Service Pack operačného systému.

  - **ServicePackMinorVer** – vedľajšia verzia balíka Service Pack operačného systému.

### <a name="officesystemsystemhealthmetadataoperatingsystemdevice"></a>Office.System.SystemHealthMetadataOperatingSystemDevice

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **CollectionTime** – čas, kedy bola táto udalosť zaradená do frontu na nahratie

  - **DeviceClass** – identifikátor typu zariadenia, v ktorom je Office spustený.

  - **DeviceManufacturer** – výrobca zariadenia, v ktorom je Office spustený.

  - **DeviceModel** – model zariadenia, v ktorom je Office spustený.

  - **DigitizerInfo** – informácie o digitalizátore pripojenom k zariadeniu, v ktorom je Office spustený.

  - **IsLaptop** – či zariadenie, v ktorom je Office spustený, je notebook.

  - **IsTablet** – či zariadenie, v ktorom je Office spustený, je tablet.

  - **IsTerminalServer** – pravda/nepravda, či ide o klienta terminálového servera

  - **MachineName** – názov zariadenia, v ktorom je Office spustený.

  - **NumProcPhysCores** – počet fyzických jadier procesora.

  - **NumProcShareSingleCache** – počet procesorov zdieľajúcich jednu vyrovnávaciu pamäť v zariadení, v ktorom je Office spustený.

  - **NumProcShareSingleCore** – počet procesorov na fyzické jadro v zariadení, v ktorom je Office spustený.

  - **OsBuild** – verzia zostavy operačného systému.

  - **OsBuildRevision** – revízia zostavy operačného systému.

  - **OSEnvironment** – Windows, iOS, Mac, Android atď.

  - **OsMajorVer** – hlavná verzia operačného systému.

  - **OsMinorVer** – vedľajšia verzia operačného systému.

  - **OSSDKVersionCode** – identifikátor verzie súpravy SDK operačného systému.

  - **OsSku** – jednotka SKU operačného systému.

  - **OsSuite2** – identifikátor balíka operačného systému.

  - **OSVersionString** – identifikátor verzie operačného systému.

  - **Platform** – identifikátor prostredia, v ktorom je Office spustený.

  - **PowerPlatformRole** – identifikátor roly počítača zariadenia, v ktorom je Office spustený, preferovanej výrobcom OEM.

  - **ProcessorCount** – počet procesorov v zariadení, v ktorom je Office spustený.

  - **ProcSpeedMHz** – rýchlosť procesora v zariadení, v ktorom je Office spustený, v MHz.

  - **ProcTypeText** – typ procesora

  - **RamMB** – množstvo pamäte RAM dostupnej v zariadení, v ktorom je Office spustený.

  - **ServicePackMajorVer** – hlavná verzia balíka Service Pack operačného systému.

  - **ServicePackMinorVer** – vedľajšia verzia balíka Service Pack operačného systému.

  - **SysVolFreeSpaceMB** – množstvo voľného miesta dostupného v systémovom zväzku v megabajtoch.

  - **SysVolSizeMB** – veľkosť systémového zväzku v megabajtoch.

### <a name="officesystemsystemhealthmetadataos"></a>Office.System.SystemHealthMetadataOS

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **CountryRegion** – identifikátor krajiny/oblasti nastavenia operačného systému.

  - **HorizontalResolution** – vodorovné rozlíšenie obrazovky.

  - **IsTerminalServer** – pravda/nepravda, či ide o klienta terminálového servera

  - **KeyboardLanguage** – identifikátor jazyka klávesnice zariadenia

  - **KeyboardLanguageTag** – identifikátor jazyka klávesnice zariadenia

  - **OfficeWvd** – identifikuje stav virtuálnej pracovnej plochy Windowsu.

  - **OsBuild** – verzia zostavy operačného systému.

  - **OsBuildRevision** – revízia zostavy operačného systému.

  - **OSEnvironment** – Windows, iOS, Mac, Android atď.

  - **OsLocale** – identifikátor miestneho nastavenia operačného systému.

  - **OsLocaleTag** – identifikátor miestneho nastavenia operačného systému.

  - **OsMajorVer** – hlavná verzia operačného systému.

  - **OsMinorVer** – vedľajšia verzia operačného systému.

  - **OSSDKVersionCode** – identifikátor verzie súpravy SDK operačného systému.

  - **OsSku** – identifikátor jednotky SKU operačného systému.

  - **OsSuite2** – identifikátor balíka operačného systému.

  - **OsUiLang** – jazyk používateľského rozhrania operačného systému.

  - **OSVersionString** – identifikátor verzie operačného systému.

  - **ScreenDepth** – hĺbka obrazovky.

  - **ScreenDpi** – rozlíšenie (DPI) obrazovky.

  - **ServicePackMajorVer** – hlavná verzia balíka Service Pack operačného systému.

  - **ServicePackMinorVer** – vedľajšia verzia balíka Service Pack operačného systému.

  - **SystemLocale** – predvolené miestne nastavenie operačného systému.

  - **SystemLocaleTag** – predvolené miestne nastavenie operačného systému.

  - **TimeZoneBiasInMinutes** –rozdiel v minútach medzi miestnym časom a UTC.

  - **VerticalResolution** – zvislé rozlíšenie obrazovky.

### <a name="officesystemsystemhealthmetadatascreencultureusersqmid"></a>Office.System.SystemHealthMetadataScreenCultureUserSqmId

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **Alias** – alias zamestnanca spoločnosti Microsoft alebo automatizovaný alias používateľa.

  - **CID** – pseudonymizovaná identita používateľa

  - **CollectibleClassifications** – klasifikácie údajov, ktoré je možné zhromažďovať podľa nastavení ochrany osobných údajov klienta.

  - **CollectionTime** – čas, kedy bola táto udalosť zaradená do frontu na nahratie

  - **CountryRegion** – identifikátor krajiny/oblasti nastavenia operačného systému.

  - **DomainName** – Názov domény Microsoft.

  - **HorizontalResolution** – vodorovné rozlíšenie obrazovky.

  - **IntegratedScreenSize** – veľkosť integrovanej obrazovky.

  - **IsJoinedToDomain** – pravda/nepravda, či je klient pripojený k doméne

  - **IsLabMachine** – či ide o počítač testovacieho laboratória spoločnosti Microsoft.

  - **IsMsftInternal** – pravda/nepravda, či je počítač pripojený k podnikovej doméne spoločnosti Microsoft.

  - **IsSubscription** – či je aplikácia balíka Office nainštalovaná v rámci licencie s predplatným.

  - **KeyboardLanguage** – identifikátor jazyka klávesnice zariadenia

  - **KeyboardLanguageTag** – identifikátor jazyka klávesnice zariadenia

  - **OsLocale** – identifikátor miestneho nastavenia operačného systému.

  - **OsLocaleTag** – identifikátor miestneho nastavenia operačného systému.

  - **OsUiLang** – jazyk používateľského rozhrania operačného systému.

  - **ScreenDepth** – hĺbka obrazovky.

  - **ScreenDpi** – rozlíšenie (DPI) obrazovky.

  - **ScreenXDpi** – vodorovné rozlíšenie (DPI) obrazovky.

  - **ScreenYDpi** – zvislé rozlíšenie (DPI) obrazovky.

  - **SqmUserId** – náhodný identifikátor inštalácie balíka Office.

  - **StudyId** – identifikátor štúdie metriky kvality softvéru.

  - **SystemLocale** – predvolené miestne nastavenie operačného systému.

  - **SystemLocaleTag** – predvolené miestne nastavenie operačného systému.

  - **TimeZoneBiasInMinutes** –rozdiel v minútach medzi miestnym časom a UTC.

  - **VerticalResolution** – zvislé rozlíšenie obrazovky.

  - **WinUserActType** – či používateľ systému Windows, ktorý má spustený Office, je lokálny správca, používateľ typu power user alebo bežný používateľ.

### <a name="officesystemsystemhealthofficelensidentity"></a>Office.System.SystemHealthOfficeLensIdentity

Informácie o identite používateľa požadované na splnenie žiadostí dotknutých osôb.

Zhromažďujú sa tieto polia:

  - **CID** – pseudonymizovaná identita používateľa

### <a name="officesystemsystemhealthrollbacksessionmetadata"></a>Office.System.SystemHealthRollbackSessionMetadata

Metaúdaje požadované na izolovanie reprodukovania zlyhania.

Zhromažďujú sa tieto polia:

  - **InstallMethod** – nová inštalácia, aktualizácia alebo návrat na predchádzajúcu verziu.

  - **IsSubscription** – či je aplikácia balíka Office nainštalovaná v rámci licencie s predplatným.

  - **PreviousBuild** – predchádzajúca nainštalovaná verzia zostavy.

### <a name="officesystemsystemhealthsessionlifecycleandheartbeat"></a>Office.System.SystemHealthSessionLifecycleAndHeartbeat

Poskytuje informácie o metrike stavu systému.

Zhromažďujú sa tieto polia:

  - **InstallMethod** – či bola aktuálna inštalácia balíka Office inovovaná zo staršej verzie, vrátená na staršiu verziu alebo nanovo nainštalovaná.

  - **InteractionSessionID** – identifikátor relácie.

  - **PreviousBuild** – verzia balíka Office, na ktorú bola táto zostava bola inovovaná alebo z ktorej bola vrátená na staršiu verziu.

  - **State** – stav, na ktorý sa relácia zmenila.

  - **Time** – čas, keď sa zmenil stav relácie.

### <a name="officesystemsystemhealthsessionstarttime"></a>Office.System.SystemHealthSessionStartTime

Používa sa s údajmi o zlyhaní na oddelenie skorších a neskorších zlyhaní (t. j. určenie, či používateľ pred zlyhaním už aplikáciu určitý čas používal).

Zhromažďujú sa tieto polia:

  - **SessionStart** – čas, kedy telemetria začala spracúvať údaje.

### <a name="officesystemsystemhealthungracefulappexitdesktop"></a>Office.System.SystemHealthUngracefulAppExitDesktop

Používa sa na zaznamenanie metriky zlyhania.

Zhromažďujú sa tieto polia:

  - **AffectedProcessAppBuild** – identifikátor verzie zostavy ovplyvneného procesu.

  - **AffectedProcessAppBuildRevision** – identifikátor revízie zostavy ovplyvneného procesu.

  - **AffectedProcessAppMinorVer** – identifikátor vedľajšej verzie ovplyvneného procesu.

  - **AffectedProcessAppName** – názov ovplyvneného procesu.

  - **AffectedProcessExeBuildVersion** – číslo verzie zostavy ovplyvneného procesu.

  - **AffectedProcessExeMajorVersion** – číslo hlavnej verzie ovplyvneného procesu.

  - **AffectedProcessExeMinorVersion** – číslo vedľajšej verzie ovplyvneného procesu.

  - **AffectedProcessExeRevisionVersion** – číslo verzie revízie zostavy ovplyvneného procesu.

  - **AffectedProcessIsDebug** – či ovplyvnený proces je zostavou ladenia.

  - **AffectedProcessIsLabMachine** – či ovplyvnený proces je v laboratóriu spoločnosti Microsoft.

  - **AffectedProcessOsEnvironment** – identifikátor operačného systému pre ovplyvnený proces.

  - **AppName** – názov ovplyvnenej aplikácie.

  - **CrashedAssignedFlights** – skupiny funkcií priradené zlyhanému procesu.

  - **CrashedConfigIds** – konfigurácia priradená zlyhanému procesu.

  - **CrashedEcsETag** – identifikátor experimentu pre zlyhaný proces.

  - **CrashedImpressionId** – identifikátor impresie zlyhaného procesu.

  - **CrashedProcessSessionID** – jedinečný identifikátor zlyhaného procesu.

  - **CrashedProcessSessionInitTime** – čas začatia ovplyvneného procesu.

  - **CrashType** – identifikátor typu zlyhania.

  - **DetectionTime** – čas zistenia neočakávaného ukončenia.

  - **ErrorString** – popis chyby.

  - **ExceptionAddress** – adresa v programe, kde došlo k zlyhaniu.

  - **ExceptionCode** – identifikátor výnimky.

  - **FaultAppName** – názov zlyhanej aplikácie.

  - **InstallMethod** – či bola aktuálna zostava balíka Office inovovaná zo staršej zostavy, vrátená na staršiu zostavu alebo nanovo nainštalovaná.

  - **InstallType** – identifikátor spôsobu inštalácie balíka Office.

  - **InstallTypeName** – identifikátor spôsobu inštalácie balíka Office.

  - **IsLabMachine** – či je balík Office spustený v laboratóriu spoločnosti Microsoft.

  - **IsMsftInternal** – či používateľ systému Windows, ktorý má spustený Office, je zamestnancom spoločnosti Microsoft.

  - **ModuleBaseAddress** – základná adresa zlyhávajúceho modulu.

  - **ModuleBuildVersion** – číslo verzie zostavy zlyhávajúceho modulu.

  - **ModuleMajorVersion** – číslo hlavnej verzie zlyhávajúceho modulu.

  - **ModuleMinorVersion** – číslo vedľajšej verzie zlyhávajúceho modulu.

  - **ModuleName** – názov zlyhávajúceho modulu.

  - **ModuleOffset** – odsadenie v bajtoch od základnej adresy, kde došlo k zlyhaniu.

  - **ModuleRevisionVersion** – číslo verzie revízie zostavy zlyhávajúceho modulu.

  - **ModuleSize** – veľkosť zlyhávajúceho modulu v bajtoch.

  - **OSEnvironment** – identifikátor prostredia, v ktorom je Office spustený.

  - **PreviousBuild** – predchádzajúca nainštalovaná verzia zostavy.

  - **UAETypeName** – identifikátor spôsobu neočakávaného zlyhania aplikácie.

  - **VerifyElseCrashTag** – jedinečný identifikátor miesta zlyhania aplikácie.

### <a name="officesystemsystemhealthungracefulappexitimmersive"></a>Office.System.SystemHealthUngracefulAppExitImmersive

Používa sa na zaznamenanie metriky zlyhania.

Zhromažďujú sa tieto polia:

  - **AffectedProcessAppBuild** – identifikátor verzie zostavy ovplyvneného procesu.

  - **AffectedProcessAppBuildRevision** – identifikátor revízie zostavy ovplyvneného procesu.

  - **AffectedProcessAppMajorVer** – identifikátor hlavnej verzie ovplyvneného procesu.

  - **AffectedProcessAppMinorVer** – identifikátor vedľajšej verzie ovplyvneného procesu.

  - **AffectedProcessAppName** – názov ovplyvneného procesu.

  - **AffectedProcessExeBuildVersion** – číslo verzie zostavy ovplyvneného procesu.

  - **AffectedProcessExeMajorVersion** – číslo hlavnej verzie ovplyvneného procesu.

  - **AffectedProcessExeMinorVersion** – číslo vedľajšej verzie ovplyvneného procesu.

  - **AffectedProcessExeRevisionVersion** – číslo verzie revízie zostavy ovplyvneného procesu.

  - **AffectedProcessIsDebug** – či ovplyvnený proces je zostavou ladenia.

  - **AffectedProcessIsLabMachine** – či ovplyvnený proces je v laboratóriu spoločnosti Microsoft.

  - **AffectedProcessOsEnvironment** – identifikátor operačného systému pre ovplyvnený proces.

  - **AppName** – názov ovplyvnenej aplikácie.

  - **CrashedAssignedFlights** – skupiny funkcií priradené zlyhanému procesu.

  - **CrashedConfigIds** – konfigurácia priradená zlyhanému procesu.

  - **CrashedImpressionId** – identifikátor impresie zlyhaného procesu.

  - **CrashedInteractionSessionID** – identifikátor relácie interakcie pre ovplyvnený proces.

  - **CrashedInteractionSessionTime** – čas, kedy bola možná interakcia s ovplyvneným systémom.

  - **CrashedProcessSessionID** – jedinečný identifikátor zlyhaného procesu.

  - **CrashedProcessSessionInitTime** – čas začatia ovplyvneného procesu.

  - **DetectionTime** – čas zistenia neočakávaného ukončenia.

  - **IsLabMachine** – či je balík Office spustený v laboratóriu spoločnosti Microsoft.

  - **IsMsftInternal** – či používateľ systému Windows, ktorý má spustený Office, je zamestnancom spoločnosti Microsoft.

  - **OSEnvironment** – identifikátor prostredia, v ktorom je Office spustený.

  - **PreviousLifecycleState** – stav ovplyvneného procesu v čase zlyhania.

  - **UAETypeName** – identifikátor spôsobu neočakávaného zlyhania aplikácie.

### <a name="officesystemsystemhealthungracefulapplicationexitwin32"></a>Office.System.SystemHealthUngracefulApplicationExitWin32

Udalosť sa aktivuje pri abnormálnom ukončení (napríklad pri tvrdom ukončení pomocou Správcu úloh, zablokovaní aplikácie a podobne) klientskych aplikácií Office, ako je napríklad Word, Excel, PowerPoint alebo Outlook. Na meranie stavu klientskych produktov Office používame metriky neočakávaného ukončenia aplikácií. Ide o signál so zásadnou dôležitosťou pre firemnú prevádzku, na základe ktorého môžu technici zaoberajúci sa produktmi Office posudzovať stabilitu produktov.

Zhromažďujú sa tieto polia:

  - **CrashedAppBuild** – identifikátor verzie zostavy ovplyvneného procesu.

  - **CrashedAppMajor** – identifikátor hlavnej verzie ovplyvneného procesu.

  - **CrashedAppMinor** – identifikátor vedľajšej verzie ovplyvneného procesu.

  - **CrashedAppRevision** – identifikátor verzie revízie ovplyvneného procesu.

  - **CrashedEcsETag** – identifikátor experimentu pre zlyhaný proces.

  - **CrashedModuleName** – názov zlyhávajúceho modulu.

  - **CrashedSessionId** – jedinečný identifikátor zlyhaného procesu.

  - **CrashedSessionInitTime** – čas začatia ovplyvneného procesu.

  - **CrashType** – identifikátor typu zlyhania.

  - **DetectionTime** – čas zistenia neočakávaného ukončenia.

  - **ExceptionAddress** – adresa v programe, kde došlo k zlyhaniu.

  - **ExceptionCode** – identifikátor výnimky.

  - **HexCrashTag** – jedinečný identifikátor kódu zlyhania.

  - **HexExceptionAddress** – adresa v programe, kde došlo k zlyhaniu, v hexadecimálnom formáte.

  - **HexExceptionCode** – identifikátor výnimky v hexadecimálnom formáte.

  - **HexModuleBaseAddress** – základná adresa zlyhávajúceho modulu v hexadecimálnom formáte.

  - **HexModuleOffset** – odsadenie v bajtoch v hexadecimálnom formáte od základnej adresy, kde došlo k zlyhaniu.

  - **HexModuleSize** – veľkosť zlyhávajúceho modulu v bajtoch v hexadecimálnom formáte.

  - **HexVerifyElseCrashTag** – jedinečný identifikátor miesta zlyhania aplikácie v hexadecimálnom formáte.

  - **InstallMethod** – či bola aktuálna zostava balíka Office inovovaná zo staršej zostavy, vrátená na staršiu zostavu alebo nanovo nainštalovaná.

  - **IsLabMachine** – či je balík Office spustený v laboratóriu spoločnosti Microsoft.

  - **ModuleBaseAddress** – základná adresa zlyhávajúceho modulu.

  - **ModuleOffset** – odsadenie v bajtoch od základnej adresy, kde došlo k zlyhaniu.

  - **ModuleSize** – veľkosť zlyhávajúceho modulu v bajtoch.

  - **PreviousBuild** – predchádzajúca nainštalovaná verzia zostavy.

  - **UAEOSEnvironment** – identifikátor prostredia operačného systému.

  - **UninitLibletId** – jedinečný identifikátor zlyhávajúcej súčasti zlyhania.

  - **VerifyElseCrashTag** – jedinečný identifikátor miesta zlyhania aplikácie.

### <a name="officesystemungracefulapplicationexitdesktopappexit"></a>Office.System.UngracefulApplicationExit.DesktopAppExit

Používa sa na zaznamenanie metriky zlyhania.

Zhromažďujú sa tieto polia:

  - **AppBuildVersion** – identifikátor verzie zostavy ovplyvneného procesu.

  - **AppMajorVersion** – číslo hlavnej verzie ovplyvneného procesu.

  - **AppMinorVersion** – číslo vedľajšej verzie ovplyvneného procesu.

  - **AppName** – názov ovplyvnenej aplikácie.

  - **AppRevisionVersion** – identifikátor revízie zostavy ovplyvneného procesu.

  - **CrashedAssignedFlights** – skupiny funkcií priradené zlyhanému procesu.

  - **CrashedConfigIds** – konfigurácia priradená zlyhanému procesu.

  - **CrashedImpressionId** – identifikátor impresie zlyhaného procesu.

  - **CrashedInteractionSessionId** – identifikátor relácie interakcie zlyhaného procesu.

  - **CrashedProcessSessionId** – jedinečný identifikátor zlyhaného procesu.

  - **CrashType** – identifikátor typu zlyhania.

  - **ErrorString** – popis chyby.

  - **ExceptionAddress** – adresa v programe, kde došlo k zlyhaniu.

  - **ExceptionCode** – identifikátor výnimky.

  - **FaultAppName** – názov zlyhanej aplikácie.

  - **InstallMethod** – či bola aktuálna zostava balíka Office inovovaná zo staršej zostavy, vrátená na staršiu zostavu alebo nanovo nainštalovaná.

  - **InstallType** – identifikátor spôsobu inštalácie balíka Office.

  - **IsDebug** – či ide o zostavu ladenia balíka Office.

  - **IsHandledCrash** – či v relácii zlyhania došlo k vyvovaniu obslužného programu zlyhania.

  - **IsLabMachine** – či je balík Office spustený v laboratóriu spoločnosti Microsoft.

  - **ModuleBaseAddress** – základná adresa zlyhávajúceho modulu.

  - **ModuleName** – názov zlyhávajúceho modulu.

  - **ModuleOffset** – odsadenie v bajtoch od základnej adresy, kde došlo k zlyhaniu.

  - **ModuleSize** – veľkosť zlyhávajúceho modulu v bajtoch.

  - **OSEnvironment** – identifikátor prostredia, v ktorom je Office spustený.

  - **PreviousBuild** – predchádzajúca nainštalovaná verzia zostavy.

  - **PreviousInteractionSessionTime** – čas začatia predchádzajúcej relácie interakcie.

  - **PreviousLifecycleState** – identifikátor stavu životného cyklu predchádzajúcej relácie.

  - **PreviousSessionInitTime** – čas začatia predchádzajúcej relácie.

  - **StackHash** – identifikátor označujúci, kde v kóde ovplyvnený proces zlyhal.

  - **VerifyElseCrashTag** – jedinečný identifikátor miesta zlyhania aplikácie.

### <a name="officesystemuserchangeddiagnosticlevel"></a>Office.System.UserChangedDiagnosticLevel

Informácie požadované na zaručenie presadzovania volieb ochrany osobných údajov používateľa.

Zhromažďujú sa tieto polia:

  - **DiagnosticLevelChanged** – označuje, že používateľ zmenil svoju úroveň diagnostiky.

  - **NewDiagnosticLevel** – úroveň po zmene používateľa.

  - **OldDiagnosticLevel** – úroveň, ktorú používateľ používal pred zmenou.

### <a name="officetelemetryariaeventsinkhandlemsadevicetokenresponse"></a>Office.Telemetry.AriaEventSink.HandleMsaDeviceTokenResponse

Signál výpadku služby konta Microsoft.

Zhromažďujú sa tieto polia:

  - **RetryCount** – počet opakovaných pokusov o pripojenie k službe MSA.

### <a name="officetelemetryariaeventsinkrequestmsadevicetoken"></a>Office.Telemetry.AriaEventSink.RequestMsaDeviceToken

Signál výpadku služby konta Microsoft.

Zhromažďujú sa tieto polia:

  - **RetryCount** – počet opakovaných pokusov o pripojenie k službe konta Microsoft.

### <a name="officetelemetryclientsamplingoverridden"></a>Office.Telemetry.ClientSamplingOverridden

Vyžaduje sa správne získanie rýchlostí reprodukcie. Za normálnych okolností sa nevzťahuje na produkčnú cieľovú skupinu.

Zhromažďujú sa tieto polia:

  - **OverriddenMeasureEnabled** – či je klient nastavený na odosielanie viac než len udalostí bez vzoriek

  - **OverriddenNumberlinePosition** – nová pozícia čísla riadka na vzorkovanie

  - **OverriddenReportedSampleRate** – nová vykázaná vzorkovacia rýchlosť

  - **OverriddenSampleRate** – nová vzorkovacia rýchlosť

  - **PreviousNumberlinePosition** – pozícia vzorkovania na čísle riadka.

  - **PreviousSampleRate** – vzorkovacia rýchlosť pred prepísaním.

  - **WasMeasureEnabled** – či bol klient nastavený na odosielanie viac než len udalostí bez vzoriek

### <a name="officetelemetrycomplianceeventnotinbasicallowlist"></a>Office.Telemetry.Compliance.EventNotInBasicAllowList

Nahlasuje neplatné implementácie alebo nasadenia telemetrie

Zhromažďujú sa tieto polia:

  - **EventName** – názov udalosti, ktorá nie je v zozname

### <a name="officetelemetrycompliancemissingdatacategory"></a>Office.Telemetry.Compliance.MissingDataCategory

Nahlasuje neplatné implementácie alebo nasadenia telemetrie

Zhromažďujú sa tieto polia:

  - **EventName** – názov udalosti, ktorej chýba kategória

  - **IsFromRule** – či udalosť pochádzala z pravidla telemetrie

### <a name="officetelemetrycompliancemissingdatacategoryinrule"></a>Office.Telemetry.Compliance.MissingDataCategoryInRule

Nahlasuje neplatné implementácie alebo nasadenia telemetrie

Zhromažďujú sa tieto polia:

  - **RuleId** – identifikátor pravidla, ktorému chýba kategória údajov

  - **RuleVersion** – verzia pravidla, ktorému chýba kategória údajov

### <a name="officetelemetrydiagnosticdataviewerstatechanged"></a>Office.Telemetry.DiagnosticDataViewerStateChanged

Overuje, či používatelia môžu zobraziť údaje tak, ako opúšťajú ich počítač, pomocou zobrazovača diagnostických údajov.

Zhromažďujú sa tieto polia:

  - **DialogCancelled** – či bolo dialógové okno zobrazovača diagnostických údajov zrušené

  - **NewState** – nový stav zobrazovača diagnostických údajov

  - **WasDialogUsed** – či sa použilo dialógové okno zobrazovača diagnostických údajov

### <a name="officetelemetrydynamicconfigfetchconfigs"></a>Office.Telemetry.DynamicConfig.FetchConfigs

Údaje potrebné na meranie stavu služby konfigurácie telemetrie.

Zhromažďujú sa tieto polia:

  - **ParsedConfigCount** – počet analyzovaných dynamických konfigurácií

  - **ParsedConfigs** – počet analyzovaných dynamických konfigurácií

  - **RejectedConfigCount** – počet zamietnutých konfigurácií

  - **RejectedConfigs** – počet zamietnutých konfigurácií

  - **RejectedConfigsList** – zoznam zamietnutých konfigurácií oddelených čiarkou

### <a name="officetelemetrydynamicconfigparsejsonconfig"></a>Office.Telemetry.DynamicConfig.ParseJsonConfig

Údaje potrebné na meranie stavu služby konfigurácie telemetrie.

Zhromažďujú sa tieto polia:

  - **ErrorMessage** – analyzované chybové hlásenie

  - **NodeName** – uzol, ktorý sa nepodarilo analyzovať

### <a name="officetelemetrydynamicconfigpopulatedrequestignored"></a>Office.Telemetry.DynamicConfig.PopulatedRequestIgnored

Táto udalosť sa vygeneruje, keď zlyhá nastavenie kanála konfigurácie telemetrie.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officetelemetrydynamicconfigpopulatetreecalledagain"></a>Office.Telemetry.DynamicConfig.PopulateTreeCalledAgain

Údaje potrebné na meranie stavu služby konfigurácie telemetrie.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officetelemetryeventquarantined"></a>Office.Telemetry.EventQuarantined

Používa sa na overenie, že iné udalosti NSD pracujú správne.

Zhromažďujú sa tieto polia:

  - **EventName** – názov udalosti v karanténe

  - **Reason** – dôvod karantény

### <a name="officetelemetryflusheventbuffer"></a>Office.Telemetry.FlushEventBuffer 

Nahlasuje veľkosť medzipamäte udalostí a môže signalizovať zlyhania telemetrie týkajúce sa používania veľkej medzipamäte.

Zhromažďujú sa tieto polia:

  - **EventCount** – počet udalostí v medzipamäti

  - **FirstPassCount** – počet prvých prechodov udalostí

  - **SecondPassCount** – počet druhých prechodov udalostí

### <a name="officetelemetrygetfilteredpayloadsfromdisk"></a>Office.Telemetry.GetFilteredPayloadsFromDisk

Overuje, že určité časti staršej infraštruktúry telemetrie fungujú na platformách, ktoré ju ešte používajú.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officetelemetryinvaliddatacontractname"></a>Office.Telemetry.InvalidDataContractName

Nahlasuje neplatné implementácie alebo nasadenia telemetrie

Zhromažďujú sa tieto polia:

  - **DataContractName** – názov zmluvy na údaje telemetrie

  - **EventName** – názov udalosti s neplatnou zmluvou na údaje

  - **IsRuleEvent** – pravda/nepravda, či bola táto udalosť implementovaná pravidlom telemetrie

### <a name="officetelemetryinvaliddatafieldname"></a>Office.Telemetry.InvalidDataFieldName 

Nahlasuje neplatné implementácie alebo nasadenia telemetrie

Zhromažďujú sa tieto polia:

  - **DataFieldName** – názov poľa údajov telemetrie

  - **EventName** – názov udalosti s neplatným poľom

  - **IsRuleEvent** – pravda/nepravda, či bola táto udalosť implementovaná pravidlom telemetrie.

### <a name="officetelemetryinvalideventcontractname"></a>Office.Telemetry.InvalidEventContractName 

Nahlasuje neplatné implementácie alebo nasadenia telemetrie

Zhromažďujú sa tieto polia:

  - **EventContractName** – názov neplatnej zmluvy na telemetriu

  - **EventName** – názov udalosti s neplatným názvom zmluvy

  - **IsRuleEvent** – pravda/nepravda, či bola táto udalosť implementovaná pravidlom telemetrie

### <a name="officetelemetryloadxmlrules"></a>Office.Telemetry.LoadXmlRules

Nahlasuje, či analyzovanie pravidiel telemetrie bolo úspešné

Zhromažďujú sa tieto polia:

  - **DetachedDuration** – trvanie odpojenia v mikrosekundách

### <a name="officetelemetrymissingfielddetails"></a>Office.Telemetry.MissingFieldDetails

Nahlasuje informácie o chýbajúcich poliach na diagnostikovanie preklepov v konfigurácii telemetrie.

Zhromažďujú sa tieto polia:

  - **ErrorRuleId** – identifikátor pravidla telemetrie, ktoré vyžiadalo chýbajúce pole

  - **ErrorRuleVersion** – verzia pravidla telemetrie, ktoré vyžiadalo chýbajúce pole

  - **EtwEventGuid** – identifikátor GUID ETW požadovaného poľa

  - **EtwEventId** – identifikátor udalosti ETW požadovaného poľa

  - **MissingFieldName** – názov požadovaného poľa

  - **UlsTagId** – kódová značka chýbajúceho poľa

### <a name="officetelemetryprocessidlequeuejob"></a>Office.Telemetry.ProcessIdleQueueJob

Nahlasuje, že nečinné spracovanie telemetrie sa začalo podľa očakávania.

Zhromažďujú sa tieto polia:

  - **DetachedDuration** – trvanie odpojenia v mikrosekundách

  - **FailureDiagnostic** – zlyhaná operácia

### <a name="officetelemetryredstoneinboxsampling"></a>Office.Telemetry.RedstoneInboxSampling

Stav vzorkovania klienta potrebný na presné interpretovanie iných metrík.

Zhromažďujú sa tieto polia:

  - **MeasuresEnabled** – či sú merania povolené v tejto relácii

  - **SamplingClientIdValue** – hodnota vzorkovania pre tohto klienta

  - **SamplingKey** – kľúč vzorkovania pre tohto klienta

  - **SamplingMethod** – metóda vzorkovania pre tohto klienta

### <a name="officetelemetryredstoneinboxsamplingcritical"></a>Office.Telemetry.RedstoneInboxSamplingCritical

Stav vzorkovania klienta môže byť potrebný na presné interpretovanie iných metrík.

Zhromažďujú sa tieto polia:

  - **MeasuresEnabled** – či sú merania povolené v tejto relácii

  - **SamplingClientIdValue** – hodnota vzorkovania pre tohto klienta

  - **SamplingKey** – kľúč vzorkovania pre tohto klienta

  - **SamplingMethod** – metóda vzorkovania pre tohto klienta

### <a name="officetelemetryruleerrorsaggregated"></a>Office.Telemetry.RuleErrorsAggregated

Hlásenie chýb stavu telemetrie. Požadované na overenie iných údajov (vrátane NSD).

Zhromažďujú sa tieto polia:

  - **ErrorCount** – počet výskytov tejto chyby v rámci časového okna agregácie

  - **ErrorInfo** – počet diagnostických informácií o chybe

  - **ErrorRuleId** – identifikátor pravidla telemetrie, ktoré spôsobilo chybu

  - **ErrorRuleVersion** – verzia pravidla telemetrie, ktoré spôsobilo chybu

  - **WarningInfo** – počet diagnostických informácií o výstrahe

<!-- end list -->

  - **QueueFlushCount** – počet vyprázdnení frontu

  - **QueueFlushDueToSizeLimit** – veľkosť, pri ktorej telemetria vyprázdni front

  - **QueueFlushesDueToSize** – počet vyprázdnení frontu spôsobených veľkosťou medzipamäte

  - **QueueHardLimit** – limit vypnutia telemetrie

  - **QueueLimitHitTime** – kedy sa dosiahol limit vypnutia telemetrie

  - **ResultTime** – čas tejto udalosti

### <a name="officetelemetryrulesenginediskthrottled"></a>Office.Telemetry.RulesEngineDiskThrottled

Metriky obmedzovania DQ. Vyžadované na dôverovanie všetkým ďalším údajom.

Zhromažďujú sa tieto polia:

  - **DiskWriteLimit** – limit veľkosti disku na údaje telemetrie

  - **DiskWriteTotal** – celkové zapisovanie na disk na údaje telemetrie

  - **SessionDiskWriteTotal** – celkové zapisovanie na disk počas relácie na údaje telemetrie

  - **ThrottlingTimestamp** – čas obmedzenia relácie

### <a name="officetelemetryrulesenginemediumcostthrottled"></a>Office.Telemetry.RulesEngineMediumCostThrottled

Metriky obmedzovania DQ. Vyžadované na dôverovanie všetkým ďalším údajom.

Táto udalosť nezhromažďuje žiadne polia.

### <a name="officetelemetryrulesenginespikethrottled"></a>Office.Telemetry.RulesEngineSpikeThrottled

Metriky obmedzovania DQ. Vyžadované na dôverovanie všetkým ďalším údajom.

Zhromažďujú sa tieto polia:

  - **CurrentLimit** – aktuálny limit špičky

  - **Duration** – trvanie špičky

  - **Factor** – faktor špičky

  - **HighestImpactingRuleBytes** – väčšina bajtov zaznamenaných pravidlom telemetrie

  - **HighestImpactingRuleId** – identifikátor pravidla, ktoré zaznamenalo najviac bajtov

  - **HighestImpactingRuleVersion** – verzia pravidla, ktoré zaznamenalo najviac bajtov

  - **MaxLimit** – maximálny limit

  - **ThrottlingTimestamp** – čas obmedzenia telemetrie

### <a name="officetelemetryrulesenginethrottled"></a>Office.Telemetry.RulesEngineThrottled

Metriky obmedzovania DQ. Vyžadované na dôverovanie všetkým ďalším údajom.

Zhromažďujú sa tieto polia:

  - **ThrottlingTimestamp** – čas obmedzenia telemetrie

### <a name="officetelemetryrulesengineulsqueuesizebackgroundprocessinglevelreached"></a>Office.Telemetry.RulesEngineUlsQueueSizeBackgroundProcessingLevelReached

Nahlasuje, že vo fronte je príliš veľa udalostí na spracovanie počas obdobia nečinnosti aplikácie.

Zhromažďujú sa tieto polia:

  - **BackgroundProcessingLevelInBytes** – veľkosť frontu na začatie spracovania na pozadí.

  - **CurrentQueueSize** – počet udalostí vo fronte nULS.

  - **CurrentQueueSizeInBytes** – veľkosť frontu nULS v bajtoch.

  - **ReachedTimestamp** – čas začatia spracúvania na pozadí.

### <a name="officetelemetryrulesresultuploadlatencyrule"></a>Office.Telemetry.RulesResultUploadLatencyRule

Priemerná, minimálna a maximálna latencia nahrávania pre nahrávanie údajovej časti výsledkov pravidla každú hodinu

Zhromažďujú sa tieto polia:

  - **AverageLatency** – priemerná latencia nahrávania

  - **CollectionTime** – čas, kedy boli zhromaždené údaje o nahratí pravidla.

  - **LatencyGE201LE400** – počet nahratí s latenciou väčšou alebo rovnou 201 ms a menšou alebo rovnou 400 ms

  - **LatencyGE3001** – počet nahratí s latenciou väčšou alebo rovnou 3001 ms

  - **LatencyGE401LE600** – počet nahratí s latenciou väčšou alebo rovnou 401 ms a menšou alebo rovnou 600 ms

  - **LatencyGE601LE800** – počet nahratí s latenciou väčšou alebo rovnou 601 ms a menšou alebo rovnou 800 ms

  - **LatencyLE200** – počet nahratí s latenciou menšou alebo rovnou 200 ms

  - **MaxLatency** – najvyššia pozorovaná latencia.

  - **MinLatency** – najnižšia pozorovaná latencia.

### <a name="officetelemetrysamplingpolicy"></a>Office.Telemetry.SamplingPolicy

Stav vzorkovania klienta potrebný na presné interpretovanie iných metrík.

Zhromažďujú sa tieto polia:

  - **MeasuresEnabled** – či sú merania povolené v tejto relácii

  - **SamplingClientIdValue** – hodnota vzorkovania pre tohto klienta

  - **SamplingKey** – kľúč vzorkovania pre tohto klienta

  - **SamplingMethod** – metóda vzorkovania pre tohto klienta

### <a name="officetelemetrysamplingpolicyeventtrigger"></a>Office.Telemetry.SamplingPolicyEventTrigger

Stav vzorkovania klienta potrebný na presné interpretovanie iných metrík.

Zhromažďujú sa tieto polia:

  - **MeasuresEnabled** – či sú merania povolené v tejto relácii

  - **SamplingKey** – kľúč vzorkovania pre tohto klienta

  - **SamplingMethod** – metóda vzorkovania pre tohto klienta

### <a name="officetelemetrysessiontelemetryruleschanged"></a>Office.Telemetry.SessionTelemetryRulesChanged

Nahlasuje, že množina pravidiel telemetrie sa zmenila

Zhromažďujú sa tieto polia:

  - **ChangedRuleId** – identifikátor pravidla telemetrie, ktoré sa zmenilo v aktuálnej aktualizácii

  - **ChangedRuleVersion** – verzia pravidla telemetrie, ktoré sa zmenilo v aktuálnej aktualizácii

  - **OperationType** – značka operácie pridania alebo odstránenia

### <a name="officetelemetrysessiontelemetryrulescount"></a>Office.Telemetry.SessionTelemetryRulesCount

Nahlasuje počet načítaných pravidiel telemetrie

Zhromažďujú sa tieto polia:

  - **CountOfLoadedRules** – počet načítaných pravidiel telemetrie

  - **HadRuleFileAtBoot** – či existoval súbor s pravidlami telemetrie pri spustení aplikácie

### <a name="officetelemetrysessiontelemetryrulesinitialstate"></a>Office.Telemetry.SessionTelemetryRulesInitialState

Nahlasuje pravidlá telemetrie, ktoré boli načítané na začiatku relácie

Zhromažďujú sa tieto polia:

  - **HadRuleFileAtBoot** – či existoval súbor s pravidlami telemetrie pri spustení aplikácie

  - **LoadedRulesCount** – počet načítaných pravidiel telemetrie

  - **LoadedRulesList** – zoznam načítaných pravidiel telemetrie

### <a name="officetelemetrysystemhealthmetadatanetworkcost"></a>Office.Telemetry.SystemHealthMetadataNetworkCost

Sieťové náklady označujú našu schopnosť získať údaje alebo nie.

Zhromažďujú sa tieto polia:

  - **NetworkCost** – nová sieť s meranými alebo nemeranými nákladmi

  - **OldNetworkCost** – predchádzajúca sieť s meranými alebo nemeranými nákladmi

  - **Tag** – značka zdrojového kódu, ktorá zistila chybu

### <a name="officetelemetrysystemhealthmetadatanetworkcostchange"></a>Office.Telemetry.SystemHealthMetadataNetworkCostChange

Sieťové náklady označujú našu schopnosť získať údaje alebo nie.

Zhromažďujú sa tieto polia:

  - **NewNetworkCost** – nová sieť s meranými alebo nemeranými nákladmi

  - **OldNetworkCost** – predchádzajúca sieť s meranými alebo nemeranými nákladmi

  - **Tag** – značka zdrojového kódu, ktorá zistila chybu

### <a name="officetelemetrytelemetryactivityaggregationwindowstatistics"></a>Office.Telemetry.TelemetryActivityAggregationWindowStatistics

Nahlasuje počet skupín a inštancií agregovaných aktivít v každej nahrávanej aktivite.

Zhromažďujú sa tieto polia:

  - **GroupCount** – počet agregovaných aktivít odosielajúcich údaje.

  - **InstancesToSend** – počet inštancií agregovaných aktivít odosielajúcich údaje.

### <a name="officetelemetrytelemetryulsqueueusage"></a>Office.Telemetry.TelemetryUlsQueueUsage

Hlásenie chýb stavu telemetrie. Požadované na overenie iných údajov (vrátane NSD).

Zhromažďujú sa tieto polia:

  - **AverageEventCount** – priemerný počet udalostí vo fronte

  - **AverageQueueCB** – priemerná veľkosť pamäte frontu

  - **PeakEventCount** – špičkový počet udalostí vo fronte

  - **PeakQueueCB** – špičková veľkosť pamäte frontu

  - **QueueDisableRuleLimit** – limit, v ktorom sa zakážu pravidlá telemetrie

### <a name="officetelemetryulsqueuetopthrottlingtags"></a>Office.Telemetry.UlsQueueTopThrottlingTags

Nahlasuje najčastejšie značky, ktoré prispeli k vypnutiu frontu ULS.

Zhromažďujú sa tieto polia:

  - **Tag0** – značka, ktorá zabrala najväčšiu časť frontu

  - **Tag0Percent** – percento frontu zabratého značkou tag0

  - **Tag1** – značka, ktorá zabrala druhú najväčšiu časť frontu

  - **Tag10** – značka, ktorá zabrala 11. najväčšiu časť frontu

  - **Tag10Percent** – percento frontu zabratého značkou tag10

  - **Tag11** – značka, ktorá zabrala 12. najväčšiu časť frontu

  - **Tag11Percent** – percento frontu zabratého značkou tag11

  - **Tag12** – značka, ktorá zabrala 13. najväčšiu časť frontu

  - **Tag12Percent** – percento frontu zabratého značkou tag12

  - **Tag13** – značka, ktorá zabrala 14. najväčšiu časť frontu

  - **Tag13Percent** – percento frontu zabratého značkou tag13

  - **Tag14** – značka, ktorá zabrala 15. najväčšiu časť frontu

  - **Tag14Percent** – percento frontu zabratého značkou tag14

  - **Tag1Percent** – percento frontu zabratého značkou tag1

  - **Tag2** – značka, ktorá zabrala 3. najväčšiu časť frontu

  - **Tag2Percent** – percento frontu zabratého značkou tag2

  - **Tag3** – značka, ktorá zabrala 4. najväčšiu časť frontu

  - **Tag3Percent** – percento frontu zabratého značkou tag3

  - **Tag4** – značka, ktorá zabrala 5. najväčšiu časť frontu

  - **Tag4Percent** – percento frontu zabratého značkou tag4

  - **Tag5** – značka, ktorá zabrala 6. najväčšiu časť frontu

  - **Tag5Percent** – percento frontu zabratého značkou tag5

  - **Tag6** – značka, ktorá zabrala 7. najväčšiu časť frontu

  - **Tag6Percent** – percento frontu zabratého značkou tag6

  - **Tag7** – značka, ktorá zabrala 8. najväčšiu časť frontu

  - **Tag7Percent** – percento frontu zabratého značkou tag7

  - **Tag8** – značka, ktorá zabrala 9. najväčšiu časť frontu

  - **Tag8Percent** – percento frontu zabratého značkou tag8

  - **Tag9** – značka, ktorá zabrala 10. najväčšiu časť frontu

  - **Tag9Percent** – percento frontu zabratého značkou tag9

### <a name="officetelemetryvolumetrackingdata"></a>Office.Telemetry.VolumeTrackingData

Metrika sledovania objemu udalosti pre udalosti telemetrie

Zhromažďujú sa tieto polia:

  - **EventThreshold** – maximálny počet inštancií jednej udalosti, ktorý možno odoslať v časovom okne.

  - **HighestEventCount** – najvyšší počet inštancií jednej udalosti odoslaných v tomto okne.

  - **HighestEventName** – názov udalosti s najväčším počtom inštancií v tomto okne.

  - **TimeWindowInSeconds** – trvanie okna v sekundách.

  - **TotalEvents** – celkový počet udalostí odoslaných počas okna.

  - **UniqueEvents** – počet jedinečných udalostí odoslaných počas okna.

### <a name="officetelemetrywritepayloadstodisk"></a>Office.Telemetry.WritePayloadsToDisk

Overuje, že určité časti staršej infraštruktúry fungujú na platformách, ktoré ju ešte používajú.

Zhromažďujú sa tieto polia:

  - **DetachedDuration** – trvanie odpojenia v mikrosekundách
