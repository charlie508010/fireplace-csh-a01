# Fireplace CSH-A01

Eigenständige Home-Assistant-Integration für den elektrischen Kamin
**Fireplace CSH-A01** über das lokale Tuya-Protokoll.

Diese HACS-Version verwendet die eigene Domain `fireplace_csh_a01`. Dadurch
erscheint sie getrennt von **Tuya Local** und kann neben der allgemeinen
Integration installiert werden. Dasselbe physische Gerät darf aber nicht
gleichzeitig in beiden Integrationen eingerichtet sein.

## Installation mit HACS

1. In HACS **Benutzerdefinierte Repositories** öffnen.
2. `https://github.com/charlie508010/fireplace-csh-a01` eintragen.
3. Kategorie **Integration** auswählen.
4. **Fireplace CSH-A01** herunterladen.
5. Home Assistant neu starten.
6. Unter **Einstellungen → Geräte & Dienste → Integration hinzufügen** nach
   **Fireplace CSH-A01** suchen.

## Finding your device ID and local key

Für die Einrichtung werden Geräte-ID, lokaler Schlüssel, lokale IP-Adresse
und Protokollversion benötigt. Diese Daten können beispielsweise aus der
Tuya-Entwicklerplattform oder einer Tuya-Gerätediagnose ermittelt werden.
Geheimnisse wie Geräte-ID und Local Key niemals in Issues oder Screenshots
veröffentlichen.

## Unterstützte Funktionen

- Gerätestrom
- Flamme mit Farbwiederherstellung in einem Tuya-Paket
- Heizstufe Aus, Stufe 1 und Stufe 2
- Soll- und Isttemperatur
- Countdown
- Flammen- und Glutbettfarbe
- Flammen- und Glutbetthelligkeit
- Temperatur-Einheit

## Optionales Dashboard

Ein modernes Beispiel-Dashboard liegt unter
[`examples/csha01_fireplace_dashboard`](examples/csha01_fireplace_dashboard/README.md).

## Herkunft und späterer Upstream-Beitrag

Die lokale Tuya-Kommunikation basiert auf dem MIT-lizenzierten Projekt
[make-all/tuya-local](https://github.com/make-all/tuya-local). Die getestete
CSH-A01-Gerätebeschreibung wird parallel in einem Fork gepflegt, damit sie
später als Pull Request an das Originalprojekt vorgeschlagen werden kann.
Dieses Repository erstellt selbst keinen Pull Request.
