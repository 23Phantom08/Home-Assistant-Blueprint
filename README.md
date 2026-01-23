# Home-Assistant-Blueprint
Home Assistant Blueprints for Fully Kiosk Browser

# Fully Kiosk – Streaming Display Timeout Blueprints

Diese Blueprints steuern automatisch den Bildschirm-Timeout von **Fully Kiosk Browser**,
abhängig davon, ob eine Streaming-App im Vordergrund läuft.

## ✨ Features
- Display bleibt **dauerhaft an**, während Streaming-Apps laufen
- Timeout wird **automatisch wiederhergestellt**, sobald Streaming beendet wird
- Unterstützt:
  - Netflix
  - Disney+
  - Amazon Prime Video
  - WOW (Sky)

## 🔧 Voraussetzungen
- Fully Kiosk Browser
- Sensor, der die aktuell aktive App meldet
- Number-Entity für den Display-Timeout (z. B. Fully Kiosk Integration)

---

## 📺 Blueprint 1 – Streaming Bildschirmtimer **aus**

Setzt den Display-Timeout auf `0`, sobald eine Streaming-App im Vordergrund startet.

👉 **Installation:**

[![Install Blueprint](https://my.home-assistant.io/badges/blueprint.svg)](
https://my.home-assistant.io/redirect/blueprint_import/?url=https://raw.githubusercontent.com/23Phantom08/Home-Assistant-Blueprint/main/blueprints/fully_kiosk_streaming_timeout_off.yaml
)

---

## ⏱ Blueprint 2 – Streaming Bildschirmtimer **an**

Stellt den Display-Timeout wieder auf einen definierten Wert zurück,
sobald eine Streaming-App verlassen wird.

👉 **Installation:**

[![Install Blueprint](https://my.home-assistant.io/badges/blueprint.svg)](
https://my.home-assistant.io/redirect/blueprint_import/?url=https://raw.githubusercontent.com/23Phantom08/Home-Assistant-Blueprint/main/blueprints/fully_kiosk_streaming_timeout_restore.yaml
)

---

## ⚠️ Wichtiger Hinweis
Beide Blueprints sind als **Paar** gedacht.  
Nur zusammen sorgen sie für korrektes Ein- und Ausschalten des Display-Timers.

---

## 👤 Autor 23Phantom08

[![Install Blueprint](https://my.home-assistant.io/badges/blueprint.svg)](https://my.home-assistant.io/redirect/blueprint_import/?url=https://raw.githubusercontent.com/23Phantom08/Home-Assistant-Blueprint/main/blueprints/fully_kiosk_streaming_timeout_off.yaml)
