# Schwarzwald Rider 6.2 – installierbare Android-Web-App (PWA)

Dies ist **keine APK**. Die App wird über eine HTTPS-Webseite auf dem Handy installiert.

## GitHub Pages (kostenlos)
1. Entpacke die ZIP-Datei.
2. Erstelle auf GitHub ein **öffentliches Repository** (z. B. `schwarzwald-rider`).
3. Lade **den Inhalt des Ordners** hoch, sodass `index.html`, `manifest.webmanifest`, `service-worker.js` und der Ordner `icons` direkt im Hauptverzeichnis des Repositories liegen.
4. Öffne **Settings → Pages** und wähle **Deploy from a branch**, Branch `main`, Ordner `/(root)`; speichere.
5. Warte auf die veröffentlichte Adresse `https://DEIN-NAME.github.io/schwarzwald-rider/`.
6. Öffne sie auf Android in **Chrome**. Tippe auf das Menü `⋮` und wähle **App installieren** bzw. **Zum Startbildschirm hinzufügen**.

**Wichtig:** Das Spiel lädt Three.js zunächst von einem externen CDN. Beim ersten Start ist eine Internetverbindung erforderlich. Der Service Worker versucht, die Engine nach dem ersten erfolgreichen Laden für spätere Offline-Nutzung zu speichern. Ohne erfolgreichen Download funktioniert die 3D-Grafik offline nicht. Das Öffnen der `index.html` als lokale Datei (`file://`) reicht für die Installation nicht aus. Die maximale FPS hängt weiterhin vom Gerät ab.
