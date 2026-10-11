# Dog Coach Website

Statische Webseite für Impressum, Datenschutz, AGB und Support.
Deutsch + Englisch auf jeder Seite (deutsche Version oben, englische unten).

## Rechtlicher Rahmen (Stand: werbefreie Privatperson-App)

Die App ist **kostenlos, werbefrei und sammelt keine Daten**. Damit:

- **App Store Connect:** Bei der Frage „Trader?" → **Nein** wählen (keine Werbeeinnahmen, kein Gewerbe). Name/Adresse werden dann **nicht** im Store veröffentlicht.
- **App-Privacy-Fragebogen:** „Data Not Collected" – die App speichert alles nur lokal.
- **Impressum:** Als reine Privatperson ohne Geschäftszweck wäre ein Impressum streng genommen nicht Pflicht – die Seite bleibt trotzdem drin, sie schadet nicht und ist für später nützlich.

## Eingetragene Daten

- **Name:** Ali Idrissi-Houari
- **Land:** Deutschland (Postadresse bewusst nicht veröffentlicht – nicht Pflicht bei kostenloser, werbefreier Privatperson-App)
- **E-Mail:** deconett@gmail.com
- **Datum:** 11.10.2026 / October 11, 2026

## Hosting mit GitHub Pages (kostenlos)

1. Neues Repository auf github.com erstellen, z. B. `dogcoach-website` (public).
2. Inhalt dieses Ordners hineinpushen:
   ```
   cd website
   git init && git add . && git commit -m "Website"
   git remote add origin https://github.com/DEINNAME/dogcoach-website.git
   git push -u origin main
   ```
3. In den Repo-Einstellungen: **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
4. Nach ca. 1 Minute ist die Seite erreichbar unter:
   `https://DEINNAME.github.io/dogcoach-website/`

## URLs für die App (AppLinks.swift)

Dann in `DogCoach/AppLinks.swift` die Zeile `base` ändern auf:

```swift
private static let base = "https://DEINNAME.github.io/dogcoach-website"
```

Die Links zeigen dann auf `…/imprint.html`, `…/terms.html`, `…/privacy.html`.

## URLs für App Store Connect

- **Support-URL:** `https://DEINNAME.github.io/dogcoach-website/`
- **Datenschutz-URL:** `https://DEINNAME.github.io/dogcoach-website/privacy.html`

## Eigene Domain (optional, später)

GitHub Pages → Custom Domain eintragen + CNAME-Datei. Danach `base` in AppLinks.swift entsprechend ändern.
