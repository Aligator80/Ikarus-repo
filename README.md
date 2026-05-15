# Ikarus Kodi Repository

Kodi repozitar pro automaticke aktualizace pluginu Ikarus.

## Adresa repozitare

```text
https://aligator80.github.io/Ikarus-repo/addons.xml
```

## Aktualni verze

- `plugin.video.ikarus` - `0.1.6`
- `repository.ikarus` - `1.0.1`

## Historie verzi

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
