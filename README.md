# Ikarus Kodi Repository

Kodi repozitar pro automaticke aktualizace pluginu Ikarus.

## Adresa repozitare

```text
https://aligator80.github.io/Ikarus-repo/addons.xml
```

## Aktualni verze

- `plugin.video.ikarus` - `0.1.16`
- `repository.ikarus` - `1.0.1`

## Historie verzi

### 0.1.16 - rychlejsi seznamy, hledani zdroju a stabilnejsi prehravani
- Zrychleno nacitani vlastnich seznamu, chytrych seznamu, rozkoukanych a zhlednutych polozek.
- Opraveno listovani ve vlastnich seznamech, aby navrat a prechod mezi strankami fungoval spravneji.
- Opraveno zobrazovani obrazku a popisu u polozek v chytrych seznamech.
- Zrychleno hledani zdroju ve filmech, serialech a rucnim hledani.
- Opraveno prehravani WebShare zdroju po upravach spolecneho prehravace.
- Lepe se oznacuji prehrane zdroje: lokalne prehrany konkretni zdroj se oznaci presneji, Trakt.TV stav zustava jen u nazvu filmu nebo serialu.
- Rucni hledani Prehraj.to, Hellspy, SkTonLine a WebShare ma spolecnejsi a odolnejsi zpracovani zdroju.
- Mrtve nebo nedostupne Hellspy streamy se zachyti driv a zapisi jasneji do logu.
- Do nastaveni byla pridana diagnostika Ikarusu pro rychlejsi kontrolu prihlaseni, Trakt.TV, seznamu, cache a fronty stahovani.
- Docasna cache nalezenych zdroju se cisti automaticky pri startu Kodi, ne pri kazdem otevreni menu.
- Doplneno podrobnejsi logovani zacatku, konce a trvani dulezitych akci, aby se lepe hledalo pripadne zaseknuti Kodi.
- Pridany dalsi ochrany proti chybejicim nebo spatnym parametrum u prehravani zdroju.

### 0.1.15 - dalsi zpřesnění seriálových názvů a epizod
- Zpřesněno hledání providerů Přehraj.to, Hellspy a WebShare pro seriály s nestandardně uloženými názvy epizod.
- Přidána podpora tolerantnější shody názvů epizod podle prefixu a významových tokenů u seriálů jako Životy slavných.
- Opraveno párování seriálu Sex O’Clock i v názvech typu S## O’Clock a S. O'Clock.
- U první série se nově rozpozná i zápis epizody ve stylu 10.díl nebo 10.diel.

### 0.1.14 - revize pokracovani serialu a zpresneni serialovych shod
- Udelana vetsi revize pokracovani na dalsi epizodu v TMDB prehravani.
- Auto-next zacina hledat dalsi epizodu driv i u kratsich dilu a ma zalozni synchronni pripravu na konci prehravani.
- Sjednocena kontrola, kdy je dalsi epizoda opravdu pripravena pro automaticke spusteni.
- Pro podporovane providery se dalsi epizoda pri auto-next snazi rozresolveovat a spoustet primo, aby byla mensi prodleva mezi dily a mene navrstvenych plugin behu.
- Zpresnena serialova filtrace na WebShare, aby kombinace spravneho cisla epizody a nazvu epizody zustala v hlavnich vysledcich.
- Slabe shody pouze podle nazvu epizody bez cisla se znovu odkladaji do posledni slozky mozne shody.

### 0.1.13 - dalsi ladeni zdroju a zrychleni hledani
- Rozkoukane a zhlednute seznamy uz berou nazvy prioritne z TMDB misto michani nazvu z Trakt.TV.
- Opraveno pokracovani na dalsi epizodu tak, aby se po rucnim zastaveni prehravani nespoustel dalsi dil.
- Zpresnen filtr serialovych zdroju na WebShare, aby se lepe oddelily spravne shody od cizich serialu a slabych shod podle samotneho nazvu epizody.
- Opraveno rozpoznavani serialu jako Akolytka / The Acolyte pro Hellspy, Prehraj.to a SkTOnline.
- Zrychleno hledani zdroju u provideru Prehraj.to, Hellspy, SkTOnline a WebShare bez omezeni poctu nalezenych zdroju.
- Zrychleno dotahovani detailu a playback stavu u vysledku, aby se seznam nalezenych zdroju zobrazoval rychleji i pri vetsim poctu polozek.
- Doplnene interni debug a casove logy pro lepsi ladeni hledani zdroju.

### 0.1.12 - sjednoceni zhlednutych a rozkoukanych s Trakt.TV
- Zhlednute a rozkoukane se zobrazuji sjednocene z lokalniho souboru a z Trakt.TV.
- Synchronizace prehravaciho stavu pres GitHub/Gist byla nahrazena lokalnim ulozenim a volitelnym napojenim na Trakt.TV.
- Pridana rucni synchronizace lokalnich zhlednutych a rozkoukanych na Trakt.TV.
- Rucni oznaceni a zruseni oznaceni filmu, epizod, serii a serialu se uklada lokalne i na Trakt.TV.
- Pri prehravani se na Trakt.TV odesila rozkoukany stav a po dokonceni prehravani zhlednuty stav.
- Pri opakovanem zhlednuti filmu nebo epizody se na Trakt.TV prepise datum zhlednuti na aktualni cas.
- Opravena ochrana proti duplicitam a zachovani puvodniho data zhlednuti pri rucni synchronizaci starsich lokalnich zaznamu.
- Opraveno nacitani popularnich filmu v TMDB menu.
- AI oprava nacitani polozek z Databaze TMDB.

### 0.1.11 - opravy hledani zdroju, znaceni a pokracovani serialu
- Zpresneno hledani zdroju pro serialove epizody, aby obecny nazev epizody jako Pilot nespoustel shody s cizimi serialy.
- Pri pokracovani na dalsi epizodu se bere prvni nejlepsi zdroj ze seznamu a pri mrtvem zdroji plugin automaticky zkusi dalsi zdroj v poradi.
- U automatickeho pokracovani se mrtve WebShare zdroje preskakuji rychleji a bez zbytecne chybove hlasky pro kazdy spatny zdroj.
- Opravena prubezna aktualizace barev, fajek a rozkoukaneho stavu po dokonceni filmu nebo epizody.
- Slozky se stejnymi WebShare zdroji prebira stav svych polozek, takze je videt rozkoukany nebo zhlednuty stav uz na slozce.
- Opraveno znaceni stavu pres Kodi overlay/playcount bez vkladani symbolu primo do nazvu polozek.
- Upraveno pojmenovani WebShare zdroju u serialu na tvar Nazev serialu - S01E09 - nazev epizody bez roku.

### 0.1.10 - informativni upozorneni pri startu
- Pri spusteni pluginu se zobrazi informativni upozorneni s povinnym potvrzenim souhlasu.
- Hlavni menu Ikarusu se spusti az po potvrzeni informativniho upozorneni.
- Do nastaveni byla pridana volba Uz nezobrazovat informativni text pri startu.
- V nastaveni je dostupne i rucni zobrazeni celeho informativniho textu.
- Upozorneni ma vlastni interni verzi, takze ho lze pri nektere dalsi aktualizaci znovu vynutit.

### 0.1.9 - vyber audio stopy a titulku
- Do ostatniho nastaveni pridany volby pro primarni audio stopu, sekundarni audio stopu a preferovane titulky.
- Pri spusteni zdroje se plugin nejdrive pokusi prepnout na primarni audio jazyk.
- Pokud primarni audio stopa neni dostupna, plugin zkusi sekundarni audio jazyk.
- Pokud neni dostupna ani primarni ani sekundarni audio stopa, zdroj se ponecha s aktualni audio stopou.
- Titulky se automaticky zapnou jen kdyz se lisi jazykova skupina prehravane audio stopy a preferovanych titulku.
- Pokud prehravane audio patri mezi CZ/SK a preferovane titulky jsou CZ/SK, titulky se nezapnou.
- Pokud je prehravane audio EN a preferovane titulky jsou EN, titulky se nezapnou.
- Pokud zdroj nema primarni ani sekundarni audio stopu a obsahuje jinou audio stopu, plugin se vzdy pokusi zapnout preferovane titulky.
- Pokud preferovane titulky ve zdroji nejsou dostupne, titulky zustanou vypnute.

### 0.1.8 - razeni a pojmenovani WebShare zdroju
- Oprava v nastaveni Info o verzi a kontrola aktualizace pluginu.
- Opraveno razeni nalezenych WebShare zdroju v TMDB knihovne.
- WebShare zdroje se radi podle potvrzeneho audio jazyka: CZ, potom SK, potom EN a nakonec ostatni nebo nezname.
- V ramci stejneho jazyka se radi podle kvality: 4K, 1080p, 720p a nizsi kvality.
- Pri stejne kvalite rozhoduje velikost souboru, vetsi soubor je vyse.
- Interni score shody zustava zachovane pro ladeni a jako pomocne kriterium pri shode ostatnich hodnot.
- Nazev WebShare zdroje se sklada z tagu jazyka, kvality a velikosti, napr. [CZ][1080p][3.2 GB].
- Pokud ma zdroj potvrzene CZ audio, zobrazi se za tagy cesky nazev filmu nebo serialu s rokem misto dlouheho nazvu souboru.
- Pokud informace o souboru nejsou citelne nebo chybi, zobrazi se puvodni nazev souboru.
- Totozne WebShare zdroje se seskupuji do slozky s poctem zdroju.

### 0.1.7 - kontrola aktualizaci z pluginu
- Polozka Zkontrolovat aktualizace Ikarus odstranena z hlavniho menu.
- V nastaveni zustava samostatna leva polozka Zkontrolovat aktualizace.
- Sekce Info o verzi otevre cisty scrollovatelny prehled zmen.
- Akce spousti Kodi kontrolu povolenych repozitaru.

### 0.1.6 - prehled verzi jako obsah nastaveni
- Polozka Info o verzi zustava v levem menu nastaveni.
- Po prepnuti na Info o verzi se prehled zobrazi rovnou v hlavni casti okna.
- Prehled verzi je upraven do beznych radku nastaveni.

### 0.1.5 - info o verzi přímo v nastavení
- Informace o verzi se zobrazí hned po otevření položky Info o verzi.
- Odstraněno extra tlačítko Zobrazit přehled verzí.
- Přehled změn je vidět přímo uprostřed okna nastavení.

### 0.1.4 - úprava okna nastavení
- Opraveno otevření tlačítka Info o verzi z nastavení.
- Položka Info o verzi přesunuta pod Stahování v levém menu nastavení.
- Verze doplněna přímo do nadpisu okna nastavení.

### 0.1.3 - info o verzi v nastavení
- Přidáno tlačítko Info o verzi do nastavení v sekci Stahování.
- Přidán přehled aktuální verze a změn přímo v nastavení pluginu.
- Do nastavení doplněn viditelný řádek s aktuální verzí pluginu.

### 0.1.2 - oprava zobrazení verze a seznamu změn
- V okně Verze se budou zobrazovat aktuální změny pluginu Ikarus.
- Doplněn přehled změn podle changelogu.

### 0.1.1 - navazování další epizody
- Upraveno navázání další epizody u seriálů z TMDB.
- V nastavení je nová volba Pokračovat další epizodou: automatické pokračování nebo výběrový dialog.
- Výchozí režim je automatické spuštění další epizody.
- Při potvrzení další epizody dialogem už plugin zbytečně neukončuje aktuální přehrávání hned v 80 procentech.
- Testovací notifikace pro další epizodu jsou ve výchozím stavu vypnuté.

### 0.1.0 - první verze
- První zkušební verze pluginu v Kodi repozitáři.
- TMDB katalog: filmy, seriály, osoby, trendující obsah a vyhledávání.
- Přehled zhlédnutých a rozkoukaných filmů a seriálů.
- Vlastní seznamy, Trakt.TV seznamy a chytré seznamy.
- Hledání zdrojů na Přehraj.to, Hellspy, SkTonLine a WebShare.
- Přehrávání zdrojů z WebShare s podporou účtu a obnovy tokenu.
- Fronta stahování a volitelné ukládání nalezených zdrojů.
- Navazování další epizody u seriálů a volba preferovaného zdroje.
- Synchronizace stavu přehrávání přes GitHub Gist.
- Vlastní seznamy se synchronizují přes Trakt.TV.

## Postup pri dalsi aktualizaci

1. Zvednout verzi v `plugin.video.ikarus/addon.xml`.
2. Dopsat zmeny do `<news>` v `plugin.video.ikarus/addon.xml` a pripadne do `plugin.video.ikarus/resources/lib/version_info.py`.
3. Spustit `ikarus-repo-tools/build_and_upload_repo.cmd`.
