# Ikarus Kodi Repository

Kodi repozitar pro automaticke aktualizace pluginu Ikarus.

## Adresa repozitare

```text
https://aligator80.github.io/Ikarus-repo/addons.xml
```

## Aktualni verze

- `plugin.video.ikarus` - `0.1.1`
- `repository.ikarus` - `1.0.1`

## Historie verzi

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
