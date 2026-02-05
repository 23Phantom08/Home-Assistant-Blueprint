# Home-Assistant-Blueprint
Home Assistant Blueprints for Fully Kiosk Browser (for Android)

# Fully Kiosk Browser – Streaming Display Timeout Blueprints

These blueprints automatically control the screen timeout of **Fully Kiosk Browser**,  
depending on whether a streaming app is running in the foreground.

## ✨ Features
- Display stays **permanently on** while streaming apps are running  
- Timeout is **automatically restored** once streaming ends  
- Supports:
  - Netflix
  - Disney+
  - Amazon Prime Video
  - WOW (Sky)
  - Jellyfin
  - 1&1 App
  - Amazon Music

## 🔧 Requirements
- Fully Kiosk Browser  
- Sensor that reports the currently active app  
- Number entity for display timeout (Fully Kiosk Integration)

---

## 📺 Blueprint 1 – Streaming Screen Timer **OFF**

Sets the display timeout to `0` as soon as a streaming app starts in the foreground.

👉 **Installation:**

[![Install Blueprint](https://my.home-assistant.io/badges/blueprint.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/23Phantom08/Home-Assistant-Blueprint/main/blueprints/fully_kiosk_streaming_timeout_off.yaml)

---

## ⏱ Blueprint 2 – Streaming Screen Timer **ON**

Restores the display timeout to a defined value once a streaming app is closed.

👉 **Installation:**

[![Install Blueprint](https://my.home-assistant.io/badges/blueprint.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/23Phantom08/Home-Assistant-Blueprint/main/blueprints/fully_kiosk_streaming_timeout_restore.yaml)

---
## ⚠️ Important Note
### Both blueprints are designed as a **pair**.  
Only together do they ensure correct activation and deactivation of the display timer.

---

# 📘 Fully Kiosk Browser – Streaming Apps Installation Guide

This guide describes step by step how to correctly set up streaming apps in Home Assistant with Fully Kiosk.

## Installation Guide:
 
### Step 1: Install App
  - Open Google Play Store or Amazon AppStore on your Fully Kiosk device
  - Download the desired streaming app:
    - Netflix
    - Disney+
    - Amazon Prime Video
    - Jellyfin
    - Amazon Music
    - WOW (Sky)

### Step 2: Edit Home Assistant Dashboard
  - Open Home Assistant
  - Go to your desired dashboard
  - Enable "Edit Dashboard"

### Step 3: Add Card
  - Click "Add Card"
  - Select card type "Picture"

### Step 4: Configure Picture
  - Select an existing image or upload your own
  - Optional: Use app logos for better overview

### Step 5: Configure Interactions
  - Go to "Interactions"
  - Select "Tap behavior"
  - Set mode to "Perform action"

### Step 6: Define Action
  - Select action "Launch app"
  - Enter the app path
    - Example:
      - com.disney.disneyplus
  - Select the desired Fully Kiosk device
  - Don't forget to save

### Step 7: Fully Kiosk Browser
  - Start Fully Kiosk Browser and set kiosk mode 
   - Press the created picture card on the dashboard, enter login credentials at the streaming provider

---

# 📦 Supported Apps & App Paths

## Apps:
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

# ✅ Done

---

### After successful setup, the blueprints can automatically control the display timeout as soon as one of the apps is started or closed.

---

## 👤 Author 23Phantom08
⭐ Feel free to leave a star ⭐
