# Ikarus Kodi Repository

Kodi repozitar pro automaticke aktualizace pluginu Ikarus.

## Adresa repozitare

```text
https://aligator80.github.io/Ikarus-repo/addons.xml
```

## Aktualni verze

- `plugin.video.ikarus` - `0.1.13`
- `repository.ikarus` - `1.0.1`

## Historie verzi

### 0.1.13

- Rozkoukane a zhlednute seznamy uz berou nazvy prioritne z TMDB misto michani nazvu z Trakt.TV.
- Opraveno pokracovani na dalsi epizodu tak, aby se po rucnim zastaveni prehravani nespoustel dalsi dil.
- Zpresnen filtr serialovych zdroju na WebShare, aby se lepe oddelily spravne shody od cizich serialu a slabych shod podle samotneho nazvu epizody.
- Opraveno rozpoznavani serialu jako `Akolytka / The Acolyte` pro `Hellspy`, `Prehraj.to` a `SkTOnline`.
- Zrychleno hledani zdroju u provideru `Prehraj.to`, `Hellspy`, `SkTOnline` a `WebShare` bez omezeni poctu nalezenych zdroju.
- Zrychleno dotahovani detailu a playback stavu u vysledku, aby se seznam nalezenych zdroju zobrazoval rychleji i pri vetsim poctu polozek.
- Doplneny interni debug a casove logy pro lepsi ladeni hledani zdroju.

### 0.1.12

- Zhlednute a rozkoukane se zobrazuji sjednocene z lokalniho souboru a z Trakt.TV.
- Synchronizace prehravaciho stavu pres GitHub/Gist byla nahrazena lokalnim ulozenim a volitelnym napojenim na Trakt.TV.
- Pridana rucni synchronizace lokalnich zhlednutych a rozkoukanych na Trakt.TV.
- Rucni oznaceni a zruseni oznaceni filmu, epizod, serii a serialu se uklada lokalne i na Trakt.TV.
- Pri prehravani se na Trakt.TV odesila rozkoukany stav a po dokonceni prehravani zhlednuty stav.
- Pri opakovanem zhlednuti filmu nebo epizody se na Trakt.TV prepise datum zhlednuti na aktualni cas.
- Opravena ochrana proti duplicitam a zachovani puvodniho data zhlednuti pri rucni synchronizaci starsich lokalnich zaznamu.
- Opraveno nacitani popularnich filmu v TMDB menu.
- AI oprava nacitani polozek z Databaze TMDB.

### 0.1.11

- Zpresneno hledani zdroju pro serialove epizody, aby obecny nazev epizody jako `Pilot` nespoustel shody s cizimi serialy.
- Pri pokracovani na dalsi epizodu se bere prvni nejlepsi zdroj ze seznamu a pri mrtvem zdroji plugin automaticky zkusi dalsi zdroj v poradi.
- U automatickeho pokracovani se mrtve WebShare zdroje preskakuji rychleji a bez zbytecne chybove hlasky pro kazdy spatny zdroj.
- Opravena prubezna aktualizace barev, fajfek a rozkoukaneho stavu po dokonceni filmu nebo epizody.
- Slozky se stejnymi WebShare zdroji prebira stav svych polozek, takze je videt rozkoukany nebo zhlednuty stav uz na slozce.
- Opraveno znaceni stavu pres Kodi overlay/playcount bez vkladani symbolu primo do nazvu polozek.
- Upraveno pojmenovani WebShare zdroju u serialu na tvar `Nazev serialu - S01E09 - nazev epizody` bez roku.

### 0.1.10

- Pri spusteni pluginu se zobrazi informativni upozorneni s povinnym potvrzenim souhlasu.
- Hlavni menu Ikarusu se spusti az po potvrzeni informativniho upozorneni.
- Do nastaveni byla pridana volba `Uz nezobrazovat informativni text pri startu`.
- V nastaveni je dostupne i rucni zobrazeni celeho informativniho textu.
- Upozorneni ma vlastni interni verzi, takze ho lze pri nektere dalsi aktualizaci znovu vynutit.
- Opraveno potvrzovaci okno pro Kodi 21, aby nezpusobovalo chybu pri startu pluginu.

### 0.1.9

- Do ostatniho nastaveni pridany volby pro primarni audio stopu, sekundarni audio stopu a preferovane titulky.
- Pri spusteni zdroje se plugin nejdrive pokusi prepnout na primarni audio jazyk.
- Pokud primarni audio stopa neni dostupna, plugin zkusi sekundarni audio jazyk.
- Pokud neni dostupna ani primarni ani sekundarni audio stopa, zdroj se ponecha s aktualni audio stopou.
- Titulky se automaticky zapnou jen kdyz se lisi jazykova skupina prehravane audio stopy a preferovanych titulku.
- Pokud prehravane audio patri mezi `CZ/SK` a preferovane titulky jsou `CZ/SK`, titulky se nezapnou.
- Pokud je prehravane audio `EN` a preferovane titulky jsou `EN`, titulky se nezapnou.
- Pokud zdroj nema primarni ani sekundarni audio stopu a obsahuje jinou audio stopu, plugin se vzdy pokusi zapnout preferovane titulky.
- Pokud preferovane titulky ve zdroji nejsou dostupne, titulky zustanou vypnute.

### 0.1.8

- Oprava v nastaveni `Info o verzi` a kontrola aktualizace pluginu.
- Opraveno razeni a pojmenovani nalezenych zdroju na WebShare.
- WebShare zdroje se radi podle potvrzeneho audio jazyka: `CZ`, potom `SK`, potom `EN`, potom ostatni nebo nezname.
- V ramci stejneho jazyka se radi podle kvality: `4K`, `1080p`, `720p` a nizsi kvality.
- Pri stejne kvalite rozhoduje velikost souboru, vetsi soubor je vyse.
- Interni `score` shody zustava zachovane pro ladeni a jako pomocne kriterium pri shode ostatnich hodnot.
- Nazev WebShare zdroje se sklada z tagu jazyka, kvality a velikosti, napr. `[CZ][1080p][3.2 GB]`.
- Pokud ma zdroj potvrzene `CZ` audio, zobrazi se za tagy cesky nazev filmu nebo serialu s rokem misto dlouheho nazvu souboru.
- Pokud informace o souboru nejsou citelne nebo chybi, zobrazi se puvodni nazev souboru.
- Totozne WebShare zdroje se seskupuji do slozky s poctem zdroju.

### 0.1.7

- Pridana polozka `Zkontrolovat aktualizace Ikarus` do hlavniho menu pluginu.
- Pridano tlacitko `Zkontrolovat aktualizace` do sekce `Info o verzi`.
- Akce spousti Kodi kontrolu povolenych repozitaru pres vestavenou funkci `UpdateAddonRepos`.

### 0.1.6

- Polozka `Info o verzi` zustava jako tlacitko v levem menu nastaveni.
- Po prepnuti na `Info o verzi` se prehled verzi zobrazi rovnou v hlavni casti okna nastaveni.
- Prehled je upraven do beznych radku nastaveni, podobne jako ostatni zalozky.

### 0.1.5

- Informace o verzi se zobrazi hned po otevreni polozky `Info o verzi`.
- Odstraneno extra tlacitko `Zobrazit prehled verzi`.
- Prehled zmen je videt primo uprostred okna nastaveni.

### 0.1.4

- Opraveno otevreni tlacitka `Info o verzi` z nastaveni.
- Polozka `Info o verzi` presunuta pod `Stahovani` v levem menu nastaveni.
- Verze doplnena primo do nadpisu okna nastaveni.

### 0.1.3

- Pridano tlacitko `Info o verzi` do nastaveni v sekci `Stahovani`.
- Pridan prehled aktualni verze a zmen primo v nastaveni pluginu.
- Do nastaveni doplnen viditelny radek s aktualni verzi pluginu.

### 0.1.2

- Opraveno zobrazeni aktualni verze a zmen primo v okne Verze v Kodi.
- Do `addon.xml` byl doplnen prehled zmen, aby Kodi nezobrazovalo jen starsi zkusebni text.

### 0.1.1

- Upraveno navazani dalsi epizody u serialu z TMDB.
- V nastaveni je nova volba `Pokracovat dalsi epizodou`: automaticke pokracovani nebo vyberovy dialog.
- Vychozi rezim je automaticke spusteni dalsi epizody.
- Pri potvrzeni dalsi epizody dialogem uz plugin zbytecne neukoncuje aktualni prehravani hned v 80 procentech.
- Testovaci notifikace pro dalsi epizodu jsou ve vychozim stavu vypnute.

### 0.1.0

- Prvni zkusebni verze pluginu v Kodi repozitari.

## Postup pri dalsi aktualizaci

1. Zvednout verzi v `plugin.video.ikarus/addon.xml`.
2. Dopsat zmeny do sekce `Historie verzi` v tomto souboru.
3. Spustit `ikarus-repo-tools/build_and_upload_repo.cmd`.
