# Ikarus Kodi Repository

Kodi repozitar pro automaticke aktualizace pluginu Ikarus.

## Adresa repozitare

```text
https://aligator80.github.io/Ikarus-repo/addons.xml
```

## Aktualni verze

- `plugin.video.ikarus` - `0.1.9`
- `repository.ikarus` - `1.0.1`

## Historie verzi

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
