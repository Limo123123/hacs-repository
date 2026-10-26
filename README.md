# 🏠 HACS Custom Repositories Index

[![HACS Custom](https://img.shields.io/badge/HACS-Custom%20Repositories-orange.svg)](https://github.com/hacs/integration)
[![Home Assistant](https://img.shields.io/badge/Home%20Assistant-2024.1+-blue.svg)](https://www.home-assistant.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

Dieses Repository dient als zentraler Katalog und Index für benutzerdefinierte **Home Assistant HACS-Integrationen und Plugins**.

---

## 📦 Enthaltene Integrationen

| Integration | Kategorie | Status | Beschreibung | Repository-Link |
| :--- | :--- | :--- | :--- | :--- |
| **Tomons / Inateck EV Wallbox** | `Integration` | 🟢 Aktiv (v1.0.0) | Vollständige Steuerung und Telemetrie für Tomons / Inateck Wallboxen (AC EV Charger). Live-Werte (V, A, W, kWh, Temp), Ladeleistung-Slider (6–32 A), Start/Stopp-Schalter und Energy Dashboard Integration. | [ha-tomons-charger](../ha-tomons-charger) |

---

## 📥 Wie binde ich eine Integration in Home Assistant ein?

Es gibt zwei einfache Wege, Integrationen aus diesem Repository in Home Assistant zu installieren:

### Methode 1: Direkte Installation via HACS (Benutzerdefiniertes Repository)

1. Öffne deine **Home Assistant** Oberfläche.
2. Navigiere zu **HACS** $\rightarrow$ **Integrationen**.
3. Klicke oben rechts auf das Drei-Punkte-Menü (**$\vdots$**) und wähle **Benutzerdefinierte Repositories** (*Custom repositories*).
4. Füge die GitHub-URL der gewünschten Integration ein:
   * **Repository-URL:** `https://github.com/Limo123123/ha-tomons-charger`
   * **Typ / Kategorie:** `Integration`
5. Klicke auf **Hinzufügen** (*Add*).
6. Die Integration erscheint nun in HACS. Klicke auf **Herunterladen** (*Download*) und starte Home Assistant neu.
7. Gehe anschließend auf **Einstellungen** $\rightarrow$ **Geräte & Dienste** $\rightarrow$ **Integration hinzufügen** und wähle die Integration aus.

### Methode 2: One-Click "My Home Assistant" Link
*(Ersetze `<DEIN_GITHUB_USERNAME>` durch deinen echten GitHub-Benutzernamen)*

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=Limo123123&repository=ha-tomons-charger&category=integration)

---

## 🔄 Wie funktionieren Updates in HACS?

HACS verfügt über ein integriertes Update-Management, das auf **GitHub Releases und Git-Tags** basiert:

1. **Versions-Tagging (Semantic Versioning):**
   * Sobald im jeweiligen Integrations-Repository (z. B. `ha-tomons-charger`) ein neues Release erstellt wird (z. B. Git-Tag `v1.0.1` oder `v1.1.0`), vergleicht HACS dieses Tag mit der Version in `manifest.json`.
2. **Automatische Benachrichtigung:**
   * Home Assistant und HACS prüfen periodisch im Hintergrund auf neue Releases.
   * Sobald ein neues Tag auf GitHub existiert, zeigt HACS automatisch einen blauen Benachrichtigungs-Badge **"Update verfügbar"** auf deiner HACS-Übersicht und in den Home Assistant Systemeinstellungen an.
3. **1-Klick Update:**
   * Der Nutzer klickt in Home Assistant einfach auf **Aktualisieren** (*Update*).
   * HACS lädt die neuen Dateien herunter, ersetzt den Ordner in `custom_components/` und bittet um einen kurzen Neustart von Home Assistant.
   * Keine manuelle Dateiverwaltung nötig!

---

## ➕ Weitere Integrationen hinzufügen

Um diesem Katalog weitere eigene Integrationen hinzuzufügen:
1. Erstelle ein neues Repository für deine Integration (z. B. `ha-meine-neue-integration`).
2. Füge eine `hacs.json` und den Ordner `custom_components/<domain>/` ein.
3. Ergänze die Tabelle in dieser `README.md` und die Liste in `repositories.json`.

---

## 📄 Lizenz
MIT License © 2026.
