# SideTrap Store

Eine AltStore-/SideStore-kompatible Source auf GitHub Pages.

## Einrichtung
1. Neues GitHub-Repo `ipa-store` anlegen und alle Dateien hochladen.
2. `SideTrap` in `source.json` und `index.html` durch deinen GitHub-Namen ersetzen.
3. Settings → Pages → Branch `main` / Root aktivieren.
4. In AltStore/SideStore: Sources → `+` → `https://sidetrap.github.io/ipa-store/source.json`

## Neue App hinzufügen
1. IPA nach `ipas/` kopieren.
2. Größe und SHA-256 ermitteln: `stat -c %s App.ipa` und `shasum -a 256 App.ipa`
3. Neuen Eintrag in `apps` in `source.json` ergänzen (Vorlage: HermesEnabler).
4. Für ein Update: neue Version **oben** in `versions` einfügen.

Hinweis: Lege außerdem ein `icon.png` (512×512) ins Repo.
