# Sicherheit & Datenschutz

Tank Alert ist eine Spritpreis-App für Deutschland. Datensparsamkeit ist ein Kernprinzip –
diese Seite erklärt **welche Daten wohin fließen**, wie wir mit Tracking umgehen und **wie du eine
Sicherheitslücke meldest**.

## Datenfluss – wer spricht mit wem

```
Clients (Web-App / iOS-App)  →  eigenes Backend (tankalert.de)  →  Tankerkönig (MTS-K)
```

- **Clients sprechen nie direkt mit Tankerkönig.** Jede Preisabfrage läuft über das eigene Backend.
  Nur das Backend kennt den Tankerkönig-API-Schlüssel.
- Das Backend **zwischenspeichert** Preisdaten und fragt die Quelle **schonend und nur bei Bedarf**
  ab (kein automatisches Dauer-Polling), im Einklang mit den Tankerkönig-Nutzungsbedingungen.

## Welche Daten verarbeitet werden

| Datum | Wofür | Wohin |
|---|---|---|
| **Standort** (GPS oder eingegebener Ort) | Tankstellen in der Nähe finden | An das eigene Backend, um Preise im Umkreis zu liefern. Wird nicht verkauft und nicht zum Tracking genutzt. |
| **E-Mail-Adresse** (nur optionales Web-Konto) | Passwortlose Anmeldung (Magic-Link) und Preisalarm-Benachrichtigung | Eigenes Backend + E-Mail-Versand. Keine Weitergabe an Dritte. |
| **Preisalarm-Einstellungen / Favoriten** | Dich benachrichtigen, Stammtankstellen merken | Eigenes Backend (Web-Konto) bzw. lokal auf dem Gerät (iOS). |
| **Push-Token** (bei aktivierten Benachrichtigungen) | Preisalarm als Push zustellen | Eigenes Backend → Web-Push bzw. Apple APNs. |

## Konten & Anmeldung

- Die Anmeldung ist **optional und passwortlos** (Magic-Link per E-Mail) – wir speichern **keine Passwörter**.
- Ein Konto wird nur benötigt, um Favoriten und Preisalarme **geräteübergreifend** zu synchronisieren.
- Die **iOS-App funktioniert komplett ohne Konto** – Favoriten und Alarme bleiben auf dem Gerät.

## Tracking & Telemetrie – im Klartext

- **Keine Werbung, keine Werbe-IDs, keine Datenweitergabe an Werbenetzwerke.**
- **Website:** datenschutzfreundliche Reichweitenmessung **nur nach aktiver Einwilligung** über das
  Cookie-Banner. Ohne Einwilligung wird keine Statistik geladen.
- **iOS-App:** ausschließlich **anonyme, DSGVO-konforme** Nutzungsstatistik **ohne Werbe-IDs** und ohne
  geräteübergreifendes Tracking. Der Standort wird nur zur Tankstellensuche verwendet.

## Datengrundlage & Lizenz

Preisdaten stammen von **[Tankerkönig](https://creativecommons.tankerkoenig.de)** unter der Lizenz
**CC BY 4.0**, basierend auf den offiziellen Meldungen der **Markttransparenzstelle für Kraftstoffe
(MTS-K)** beim Bundeskartellamt. Tank Alert ist ein unabhängiges Projekt ohne Verbindung zu
Mineralölunternehmen.

## Eine Sicherheitslücke melden

Wir nehmen Sicherheitsmeldungen ernst und sind für verantwortungsvolle Hinweise dankbar.

- 📧 **E-Mail:** [security@tankalert.de](mailto:security@tankalert.de)
- Bitte **kein öffentliches GitHub-Issue** für Sicherheitsthemen verwenden.
- Hilfreich für uns: betroffener Bereich (Web/iOS), Beschreibung, Schritte zum Nachstellen und – falls
  vorhanden – ein Proof-of-Concept.
- Bitte gib uns eine **angemessene Frist zur Behebung**, bevor du Details veröffentlichst (Coordinated Disclosure).

Vielen Dank, dass du hilfst, Tank Alert sicher zu halten. 🙏
