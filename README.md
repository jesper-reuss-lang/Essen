# Einkaufsplaner – PWA

Eine installierbare App (PWA) zum Planen von Gerichten, Abgleichen des Vorrats und cleveren Einkaufen.
Läuft komplett im Browser, alle Daten bleiben lokal auf dem Gerät.

## Dateien (alle ins GitHub-Repo hochladen)

- `index.html` – Einstieg (leitet zur App weiter)
- `Einkaufsplaner.html` – die eigentliche App
- `manifest.json` – App-Infos (Name, Icon, Farben) für die Installation
- `sw.js` – Service Worker (Offline-Betrieb)
- `icon.svg` – App-Icon

## Auf GitHub Pages veröffentlichen

1. Auf [github.com](https://github.com) anmelden (oder kostenlos registrieren).
2. Oben rechts **+** → **New repository**. Name z. B. `einkaufsplaner`, **Public**, **Create repository**.
3. **Add file** → **Upload files** → alle oben genannten Dateien hineinziehen → **Commit changes**.
4. **Settings** → links **Pages** → unter *Build and deployment* die *Source* auf **Deploy from a branch** stellen, Branch **main** / Ordner **/(root)** → **Save**.
5. Nach ~1 Minute erscheint die Adresse: `https://DEIN-NAME.github.io/einkaufsplaner/`

## Auf dem Handy installieren

- **iPhone (Safari):** Adresse öffnen → Teilen-Symbol → **Zum Home-Bildschirm**.
- **Android (Chrome):** Adresse öffnen → Menü (⋮) → **App installieren** / **Zum Startbildschirm**.

## App aktualisieren

Wenn die App-Dateien geändert werden: in `sw.js` die Zeile `const CACHE = 'einkaufsplaner-v1';`
hochzählen (z. B. `-v2`) und die Dateien neu hochladen. Beim nächsten Öffnen lädt die neue Version.

## Daten sichern

Die Rezepte und der Vorrat liegen nur im Browser des jeweiligen Geräts.
In der App unter ⚙️ → **Daten exportieren** regelmäßig ein Backup erstellen
und auf einem anderen Gerät über **Daten importieren** einspielen.
