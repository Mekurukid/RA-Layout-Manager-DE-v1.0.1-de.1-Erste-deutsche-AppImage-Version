# RA Layout Manager DE

Eine inoffizielle deutsche Linux-AppImage des **RetroAchievements Layout Managers** mit vollständig übersetzter Benutzeroberfläche, automatischer Übersetzung von Erfolgen und direkten lokalen OBS-Browserquellen.

> **Aktuelle Version:** `v1.0.2-de.1`

---

## Highlights

- Deutsche Benutzeroberfläche
- Automatische Übersetzung von Achievement-Namen und -Beschreibungen
- Linux-AppImage – keine klassische Installation notwendig
- Optimiert für Nobara Linux und andere aktuelle Linux-Distributionen
- Direkte OBS-Browserquellen als lokale HTML-Dateien
- Kein Fenster- oder Bildschirm-Capture des Trackers mehr notwendig
- Achievement- und Mastery-Benachrichtigungen direkt in OBS
- Lokaler Übersetzungs-Cache
- Englischer Originaltext als Fallback
- Bestehende Overlay-Funktionen bleiben erhalten

---

## Neu in v1.0.2-de.1

Mit Version `v1.0.2-de.1` wurden lokale OBS-Browserquellen ergänzt.

Die Overlays müssen dadurch nicht mehr als separates Tracker-Fenster geöffnet und anschließend über eine OBS-Fensteraufnahme aufgenommen werden.

Der Tracker erzeugt automatisch lokale Browserdateien, die direkt in OBS als **Browserquelle → Lokale Datei** eingebunden werden können.

### Verfügbare OBS-Browserquellen

- `Fokus.html`
- `Meldungen.html`
- `Erfolgsliste.html`
- `Letzte-Erfolge.html`
- `Benutzerinfo.html`
- `Spielinfo.html`
- `Spielfortschritt.html`
- `Medien.html`

Zusätzlich werden die benötigten lokalen Daten und Assets automatisch erzeugt bzw. aktualisiert.

---

## OBS-Browserquellen verwenden

1. Den RA Layout Manager DE starten.
2. Im Tracker den Bereich **Dateien & Einstellungen** öffnen.
3. Auf **OBS-Browserquellen öffnen** klicken.
4. OBS öffnen.
5. Eine neue Quelle hinzufügen:
   - **Browser**
   - **Lokale Datei** aktivieren
6. Die gewünschte HTML-Datei auswählen, zum Beispiel:
   - `Fokus.html`
   - `Meldungen.html`
7. Breite und Höhe einstellen.
8. Fertig.

Das zugehörige Overlay-Fenster muss im Tracker nicht geöffnet sein.

---

## Empfohlene OBS-Größen

| Browserquelle | Empfohlene Größe |
|---|---:|
| Fokus | 700 × 165 |
| Meldungen | 1024 × 768 |
| Benutzerinfo | 805 × 290 |
| Spielinfo | 1190 × 645 |
| Spielfortschritt | 805 × 350 |
| Letzte Erfolge | 511 × 600 |
| Erfolgsliste | 680 × 480 |
| Medien | 640 × 480 |

Die Größen sind Empfehlungen und können je nach OBS-Layout angepasst werden.

---

## Automatische deutsche Achievement-Übersetzung

Achievement-Titel und -Beschreibungen werden automatisch ins Deutsche übersetzt.

Die übersetzten Texte werden unter anderem verwendet für:

- Fokus
- Achievement-Liste
- Letzte Erfolge
- Achievement-Benachrichtigungen
- Mastery-Benachrichtigungen
- Stream-/OBS-Overlays

Übersetzungen werden lokal zwischengespeichert. Falls der Übersetzungsdienst vorübergehend nicht erreichbar ist, verwendet die App den englischen Originaltext als Fallback.

---

## Installation unter Linux / Nobara

Die Anwendung wird als AppImage bereitgestellt und benötigt keine klassische Installation.

### 1. AppImage herunterladen

Lade die aktuelle Datei aus dem Bereich **Releases** herunter:

```text
RA-Layout-Manager-DE-v1.0.2-de.1-x86_64.AppImage
```

### 2. Ausführbar machen

```bash
chmod +x RA-Layout-Manager-DE-v1.0.2-de.1-x86_64.AppImage
```

### 3. Starten

```bash
./RA-Layout-Manager-DE-v1.0.2-de.1-x86_64.AppImage
```

Unter vielen Desktop-Umgebungen kann die AppImage anschließend auch per Doppelklick gestartet werden.

---

## Nobara Linux

Die AppImage wurde speziell mit Blick auf Nobara Linux erstellt und getestet.

Falls sich AppImages bei dir nicht per Doppelklick starten lassen:

1. Rechtsklick auf die AppImage
2. **Eigenschaften**
3. Datei als ausführbar markieren

Alternativ:

```bash
chmod +x RA-Layout-Manager-DE-v1.0.2-de.1-x86_64.AppImage
```

---

## RetroAchievements

Für die Verwendung der RetroAchievements-Funktionen werden deine eigenen RetroAchievements-Zugangsdaten bzw. API-Daten benötigt.

Diese Daten gehören dir und sollten niemals öffentlich geteilt werden.

> **Wichtig:** Veröffentliche niemals deinen RetroAchievements API-Key in GitHub Issues, Screenshots, Logs oder anderen öffentlichen Beiträgen.

---

## Datenschutz

Die Anwendung verarbeitet die für die RetroAchievements-Funktionen benötigten Daten lokal bzw. über die dafür erforderlichen externen Dienste.

Für die automatische Übersetzung können Achievement-Titel und -Beschreibungen an einen Übersetzungsdienst übertragen werden.

Der RetroAchievements API-Key wird nicht in die lokalen OBS-Browserdateien geschrieben.

---

## Prüfsumme

Für jeden Release sollte zusätzlich eine `SHA256SUMS.txt` bereitgestellt werden.

Beispiel:

```bash
sha256sum RA-Layout-Manager-DE-v1.0.2-de.1-x86_64.AppImage
```

Vergleiche die Ausgabe anschließend mit der Prüfsumme im jeweiligen GitHub Release.

---

## Bekannte Hinweise

- Die automatische Übersetzung benötigt für neue, noch nicht gecachte Texte eine Internetverbindung.
- Die Qualität automatischer Übersetzungen kann je nach Achievement variieren.
- Manche Eigennamen oder spielspezifischen Begriffe können im Original bleiben.
- Die lokalen OBS-Browserdateien sollten nicht manuell verschoben oder umbenannt werden, wenn der Tracker sie weiterhin automatisch aktualisieren soll.
- Nach einem größeren Update empfiehlt es sich, OBS-Browserquellen einmal neu zu laden.

---

## Fehler melden

Wenn du einen Fehler findest, erstelle bitte ein GitHub Issue und gib möglichst folgende Informationen an:

- Version der App
- Linux-Distribution
- Desktop-Umgebung
- OBS-Version, falls der Fehler ein Overlay betrifft
- kurze Beschreibung des Problems
- Schritte zum Reproduzieren

Screenshots sind ebenfalls hilfreich.

**Bitte entferne vorher API-Keys, Tokens, Benutzerdaten und andere private Informationen.**

---

## Upstream / Credits

Dieses Projekt basiert auf dem **RetroAchievements Layout Manager** von **Colossus-Gaming**.

Upstream-Projekt:

```text
https://github.com/Colossus-Gaming/retroachievements-layout-manager
```

Vielen Dank an die ursprünglichen Entwickler und an die RetroAchievements-Community.

RetroAchievements:

```text
https://retroachievements.org/
```

---

## Disclaimer

Dieses Projekt ist eine **inoffizielle deutsche Modifikation / Distribution**.

Es besteht keine offizielle Verbindung zu RetroAchievements, Colossus-Gaming oder den Rechteinhabern der unterstützten Spiele und Marken.

Alle genannten Produktnamen, Spiele, Marken, Logos und sonstigen Kennzeichen gehören ihren jeweiligen Rechteinhabern.

Diese Version wird ohne Gewähr bereitgestellt. Die Nutzung erfolgt auf eigene Verantwortung.

---

## Lizenz- und Verbreitungshinweis

Dieses Repository vergibt nicht automatisch neue Rechte an Bestandteilen des ursprünglichen Projekts oder an eingebundenen Drittanbieter-Komponenten.

Für Bestandteile des Upstream-Projekts und für Drittanbieter-Abhängigkeiten gelten die jeweils zugehörigen Lizenz- und Nutzungsbedingungen.

Prüfe vor einer öffentlichen Weitergabe von modifizierten Binärdateien, ob die erforderlichen Rechte und Bedingungen erfüllt sind.

---

## Versionen

### v1.0.2-de.1

- Lokale OBS-Browserquellen hinzugefügt
- Alle wichtigen Overlay-Typen als lokale HTML-Dateien verfügbar
- OBS kann die Overlays ohne Fensteraufnahme des Trackers anzeigen
- Achievement- und Mastery-Meldungen direkt an die Browserquelle angebunden
- Browserquellen werden automatisch im Benutzerordner erzeugt und aktualisiert
- Deutsches Interface beibehalten
- Automatische Achievement-Übersetzung beibehalten
- API-Key wird nicht in die OBS-Browserdateien geschrieben

### v1.0.1-de.1

- Deutsche Benutzeroberfläche
- Automatische Übersetzung von Achievement-Titeln
- Automatische Übersetzung von Achievement-Beschreibungen
- Deutscher Übersetzungs-Cache
- Linux-/Nobara-AppImage

---

## Screenshots

Später können Screenshots ergänzt werden:

```markdown
![Hauptfenster](screenshots/hauptfenster.png)

![OBS Browserquelle](screenshots/obs-browserquelle.png)

![Fokus Overlay](screenshots/fokus-overlay.png)
```

---

## Download

Die aktuelle AppImage findest du unter:

**GitHub → Releases → Latest Release**

Empfohlene Release-Dateien:

```text
RA-Layout-Manager-DE-v1.0.2-de.1-x86_64.AppImage
SHA256SUMS-v1.0.2-de.1.txt
```

---

## Support

Wenn dir ein Fehler auffällt oder du eine Verbesserung vorschlagen möchtest, nutze bitte die **GitHub Issues** dieses Repositories.

Feature-Wünsche für weitere Overlays, Übersetzungen oder OBS-Funktionen sind willkommen.