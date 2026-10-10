### Plugin: Bible Fragment Linker

- Włączony w vaultcie
- Skrót: Alt+G (Alt+C zostaje dla Bible Linker)
- Modal jak w Bible Linker → wpisujesz np. `Mt 1,1-3.6` → tworzy fragment (jeśli trzeba) i wstawia:

`[[Bible_notes/Bible_Fragments/Mt 1#**Mt 1,1-3.6**|Mt 1,1-3.6]]`

Pojedynczy werset (sam numer, bez `-`, `.`, `n`) — bez zapisu do `Bible_Fragments`, tylko link do `Bible_notes`. Ścieżka i nagłówek bez spacji w księgach numerowanych (jak w plikach), alias po `|` ze spacją:

- `Mt 1,1` → `[[Bible_notes/Mt 1#**Mt 1,1**|Mt 1,1]]`
- `1P 2,5` albo `1 Sm 3,1` → `[[Bible_notes/1P 2#**1P 2,5**|1 P 2,5]]` / `[[Bible_notes/1Sm 3#**1Sm 3,1**|1 Sm 3,1]]`

Zakresy (`Mt 1,1-3`, `Mt 1,1-3.6`, `1P 2,5.9`) tworzą/dopisują fragment i linkują do `Bible_Fragments`.

Ścieżki ustawisz w Settings → Bible Fragment Linker. Po instalacji zrób Reload app w Obsidianie.

### Instalacja

W tym archiwum jest już dodany, ale dodanie do nowego archiwum:

Skopiuj folder pluginu do drugiego vaultu:

```
<source_vault>/.obsidian/plugins/bible-fragment-linker/
```

zawartość:

- `manifest.json`
- `main.js`
- `styles.css`
- (opcjonalnie) `data.json` — ustawienia

do:

```
<other_vault>/.obsidian/plugins/bible-fragment-linker/
```

Potem w tym vaultcie:

1. Settings → Community plugins → włącz _Restricted mode_ off (jeśli jest)
2. Znajdź Bible Fragment Linker na liście i włącz
3. Albo dopisz `"bible-fragment-linker"` do `.obsidian/community-plugins.json`
4. Reload app (albo zrestartuj Obsidian)

Skrót Alt+G jest w `hotkeys.json` — w nowym vaultcie trzeba go ustawić ręcznie: Settings → Hotkeys → „Insert Bible fragment link”.

W ustawieniach pluginu sprawdź ścieżki (`Bible_notes` / `Bible_notes/Bible_Fragments`), jeśli w drugim vaultcie folderów nazywasz inaczej.

