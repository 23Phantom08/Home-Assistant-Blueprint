# Home-Assistant-Blueprint
Home Assistant Blueprints for Fully Kiosk Browser (für Android)

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
  - Jellyfin
  - 1&1 App
  - Amazon Music

## 🔧 Voraussetzungen
- Fully Kiosk Browser  
- Sensor, der die aktuell aktive App meldet  
- Number-Entity für den Display-Timeout (z. B. Fully Kiosk Integration)

---

## 📺 Blueprint 1 – Streaming Bildschirmtimer **aus**

Setzt den Display-Timeout auf `0`, sobald eine Streaming-App im Vordergrund startet.

👉 **Installation:**

[![Install Blueprint](https://my.home-assistant.io/badges/blueprint.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/23Phantom08/Home-Assistant-Blueprint/main/blueprints/fully_kiosk_streaming_timeout_off.yaml)

---

## ⏱ Blueprint 2 – Streaming Bildschirmtimer **an**

Stellt den Display-Timeout wieder auf einen definierten Wert zurück, sobald eine Streaming-App verlassen wird.

👉 **Installation:**

[![Install Blueprint](https://my.home-assistant.io/badges/blueprint.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/23Phantom08/Home-Assistant-Blueprint/main/blueprints/fully_kiosk_streaming_timeout_restore.yaml)

---

## ⚠️ Wichtiger Hinweis
Beide Blueprints sind als **Paar** gedacht.  
Nur zusammen sorgen sie für korrektes Ein- und Ausschalten des Display-Timers.

---

## 👤 Autor 23Phantom08

⭐ Lasst mir gerne einen Stern da ⭐

---

# 📘 Fully Kiosk Browser – Streaming Apps Installation Guide

Diese Anleitung beschreibt Schritt für Schritt,wie Streaming-Apps in Home Assistant mit Fully Kiosk korrekt eingerichtet werden.

## Installation_guide:
 
 Schritt 1: App installieren
  - Öffne den Google Play Store oder Amazon AppStore auf deinem Fully-Kiosk-Gerät
  - Lade die gewünschte Streaming-App herunter:
    - Netflix
    - Disney+
    - Amazon Prime Video
    - Jellyfin
    - Amazon Music
    - WOW (Sky)

 Schritt 2: Home Assistant Dashboard bearbeiten
  - Öffne Home Assistant
  - Gehe zu deinem gewünschten Dashboard
  - Aktiviere "Dashboard bearbeiten"

 Schritt 3: Karte hinzufügen
  - Klicke auf "Karte hinzufügen"
  - Wähle die Kartenart "Bild"

 Schritt 4: Bild konfigurieren
  - Wähle ein vorhandenes Bild aus oder lade ein eigenes hoch
  - Optional: Nutze App-Logos für bessere Übersicht

 Schritt 5: Interaktionen konfigurieren
  - Gehe zu "Interaktionen"
  - Wähle "Verhalten beim Antippen"
  - Setze den Modus auf "Aktion ausführen"

  Schritt 6:
    Aktion definieren
         - Wähle die Aktion "App starten"
         - Trage den App Pfad ein
              Beispiel:
               - com.disney.disneyplus
         - Wähle das gewünschte Fully-Kiosk-Gerät aus
         - Speichern nicht vergessen

 Schritt 7:
  - Fully Kiosk Browser starten und den Kiosk Mode einstellen 
   - im Dashboard auf die gebaute Bild Karte drücken, Anmeldedaten beim Streaming Anbieter eingeben und fertig

---

# 📦 Unterstützte Apps & App-Pfade

# Apps:
  - name: Netflix
  - app_id: com.netflix.mediaclient

  - name: Disney+
  - app_id: com.disney.disneyplus

  - name: Amazon Prime Video
  - app_id: com.amazon.avod

  - name: WOW (Sky)
  - app_id: de.sky.online

  - name: Jellyfin
  - app_id: org.jellyfin.mobile

  - name: Amazon Music
  - app_id: com.amazon.mp3

  - name: 1&1 TV
  - app_id: com.einsundeinstv.player

---

# ✅ Fertig
---

# Nach erfolgreicher Einrichtung können die Blueprints den Display-Timeout automatisch steuern, sobald eine der Apps gestartet oder beendet wird.

---
