# AR Model Viewer (Folder Mode)

Ein webbasierter 3D-Modell-Viewer, der es ermöglicht, ganze Ordner mit .glb-Dateien zu laden, sie im Browser zu betrachten und per Cloud-Link für Augmented Reality (AR) zu teilen.

---

## Features

* **Ordner-Upload:** Lade einen kompletten lokalen Ordner hoch und wähle Modelle bequem über ein Dropdown-Menü aus.
* **Instant Preview:** Modelle werden sofort lokal im Browser gerendert (via Google <model-viewer>).
* **Cloud Sharing:** Automatischer Upload zu Litterbox (24h Speicher), um einen teilbaren Link und einen QR-Code zu generieren.
* **Smart Receiver Workflow (Direkt-Download):** Der erzeugte Link startet beim Empfänger sofort einen automatischen Hintergrund-Download der ausgewählten .glb-Datei auf das Endgerät (inklusive automatischem Zeitstempel-Dateinamen). Zusätzlich erhält der Empfänger einen Button, um das Modell mit einem Klick direkt im Browser-AR zu öffnen.
* **Augmented Reality (AR):** Betrachte die Modelle direkt in deiner Umgebung (unterstützt WebXR, Scene-Viewer und Quick-Look).
* **Theme Toggle:** Wechsel zwischen einem sauberen weißen Modus und einem eleganten Off-White (Creme) Design.
* **Responsive Design:** Optimiert für Desktop und mobile Endgeräte.

---
Aufruf: https://skaterdenni-coder.github.io/Model_Viewer_Folder/ 
## Technologien

* **Framework:** Google Model Viewer
* **Bibliotheken:** qrcode.js für die Generierung von QR-Codes.
* **Hosting/API:** Litterbox API für den temporären Datei-Host (Dateien werden nach 24h gelöscht).
* **Sprachen:** HTML5, CSS3 (CSS Variables für Themes), JavaScript (ES6+).

---

## Installation & Nutzung

Da es sich um eine reine Client-seitige HTML-Datei handelt, ist keine Installation notwendig:

1. **Datei speichern:** Speichere den Code als index.html.
2. **Im Browser öffnen:** Öffne die Datei einfach in einem modernen Browser (Chrome, Edge oder Safari empfohlen).
3. **Modelle laden:**
   * Klicke auf das gestrichelte Upload-Feld.
   * Wähle einen Ordner auf deinem Computer aus, der .glb-Dateien enthält.
   * Bestätige die Browser-Abfrage zum Zugriff auf den Ordner.
4. **Teilen & Empfangen:** Sobald ein Modell über das Dropdown ausgewählt ist, wird im Hintergrund ein Link generiert. Kopiere den Link oder lass den QR-Code scannen. Der Empfänger erhält beim Aufrufen sofort die Datei als Download auf sein Gerät und kann über den integrierten Button direkt in die AR-Projektion springen.

> Wichtig: Für die AR-Funktionen muss die Seite über HTTPS aufgerufen werden (z. B. via GitHub Pages).

---

## Einschränkungen & Voraussetzungen

* **Dateiformat:** Nur .glb (glTF Binary) wird unterstützt.
* **Internetverbindung:** Erforderlich für das Laden der Skripte (CDN) und den Cloud-Upload.
* **AR-Support:** Ein AR-fähiges Mobilgerät (Android mit ARCore oder iOS mit ARKit).
* **Gültigkeit:** Da Externer Dienst genutzt wird, werden hochgeladene Dateien nach 24 Stunden automatisch gelöscht.

---

## Lizenz & Credits

* **Entwickelt von:** Simba
* **Nutzung:** Dieses Projekt ist für Testzwecke und Präsentationen optimiert. Beachte, dass hochgeladene Dateien über den Litterbox-Dienst öffentlich (via Link) zugänglich sind.
