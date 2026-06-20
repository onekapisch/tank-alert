# Changelog

Alle nennenswerten Änderungen an Tank Alert (Web-App & iOS-App). Format angelehnt an
[Keep a Changelog](https://keepachangelog.com/de/1.1.0/); neueste Einträge oben.

👉 **Web-App:** [tankalert.de](https://tankalert.de) · **iOS-App:** in Prüfung – bald im App Store.

## [iOS 1.0.0] – Juni 2026 · _in Prüfung_

Erste Version der nativen iOS-App (SwiftUI, iOS 17+) – kostenlos, werbefrei, ohne Konto.

### Neu
- Günstigste Tankstellen live in der Nähe (Super E10, E5, Diesel)
- Preisalarm mit Push-Mitteilung, sobald eine nahe Tankstelle den Wunschpreis unterschreitet
- **Tankuhr** – beste Tankzeit mit 24-Stunden-Verlauf
- Homescreen-Widget mit dem günstigsten Preis in der Nähe
- Spritkosten-Rechner und E10/E5-Vergleich
- Kartenansicht mit Navigation über Apple Karten
- Komplett zweisprachig (Deutsch & Englisch), in der App umschaltbar

## [Web] – April 2026

### Neu
- Nationale Landingpages für **E10** und **E5** sowie ein statischer Marktupdate-Index
- Dated Marktupdate-Seiten für aktuelle Spritpreis-Suchanfragen
- **Tankwissen**-Bereich zur neuen Preisregel (eine Preiserhöhung pro Tag, 12-Uhr-Fenster) mit Primärquellen (Bundesregierung, Bundestag, ADAC)

### Geändert
- Tankuhr- und SEO-Empfehlungen auf das Vergleichsfenster **kurz vor 12:00 Uhr** aktualisiert
- Markenkonforme E-Mail-Logos in Preisalarm- und Magic-Link-Mails korrigiert

## [Web] – März/April 2026

### Neu
- **Preisalarme & Push-Benachrichtigungen** (Web-Push) inkl. Konto-Seite mit Statistiken
- **Preisverlauf-Charts** in der Favoriten-Detailansicht
- Passwortlose Anmeldung (Magic-Link) – keine Passwörter
- Fuel-Provider-Health-Endpunkte zur direkten Diagnose der Datenquelle

### Geändert
- Interaktive Anfragen haben Vorrang vor Hintergrund-Refreshes (schonendere Quellenabfrage)
- Stale-Cache-Fallback statt harter „nicht verfügbar"-Fehler bei kurzzeitigen Quellen-Aussetzern

### Behoben
- GA4-Consent-Bootstrap: korrekte Pageviews erst nach aktiver Einwilligung
- Rate-Limit-Handling der Fuel-Routen liefert nun zwischengespeicherte Daten statt Fehlzuständen

---

<sub>Preisdaten von <a href="https://creativecommons.tankerkoenig.de">Tankerkönig</a> · CC BY 4.0 · MTS-K / Bundeskartellamt.</sub>
