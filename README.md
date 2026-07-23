# ContextCruncher

**ContextCruncher** ist ein kleines Windows-Programm, das dir beim Kopieren, Ordnen
und Verkleinern von Text und Screenshots hilft — praktisch, wenn du oft mit
ChatGPT, Claude & Co. arbeitest. Es läuft **komplett auf deinem PC**: **keine
Cloud, keine Anmeldung, keine Administrator-Rechte**, und ohne Internet werden
keine Daten verschickt.

---

## ⬇️ Programm herunterladen

Immer die **neueste Version** gibt es hier — ein Klick, kein Konto nötig:

### 👉 **[ContextCruncher.exe herunterladen](https://github.com/n-sig/ContextCruncher/releases/latest/download/ContextCruncher.exe)**

> 💡 **Tipp:** Speichere diesen Link als Lesezeichen. Er zeigt **immer** auf die
> aktuellste Version — du musst nichts weiter suchen. Wenn eine neue Version da
> ist, lädst du über denselben Link einfach die neue `ContextCruncher.exe` herunter
> und ersetzt damit die alte.

Es gibt **nichts zu installieren**: Die heruntergeladene `ContextCruncher.exe`
kannst du direkt starten (z. B. per Doppelklick). Am besten legst du sie in einen
eigenen Ordner, z. B. `C:\ContextCruncher\`.

---

## ⚠️ Beim ersten Start: die blaue Windows-Warnung

Weil das Programm (noch) nicht kostenpflichtig digital signiert ist, zeigt Windows
beim ersten Start eine blaue Warnung namens **„Der Computer wurde durch Windows
geschützt"** (SmartScreen). Das ist **normal** bei kleinen Programmen und bedeutet
nur, dass Windows den Herausgeber nicht kennt — **kein Virus**.

So startest du es trotzdem (nur **einmal pro Version** nötig):

1. Im blauen Fenster auf **„Weitere Informationen"** klicken.
2. Dann erscheint unten der Knopf **„Trotzdem ausführen"** — darauf klicken.

Danach startet ContextCruncher ganz normal. Beim nächsten Start derselben Version
kommt die Warnung nicht mehr.

> Falls dein Virenscanner oder Browser den Download blockiert: Es handelt sich um
> einen **Fehlalarm** (unsignierte kleine Programme lösen den öfter aus). Du kannst
> den Download in deinem Browser bzw. Virenscanner als Ausnahme erlauben.

---

## 🚀 Erste Schritte

Nach dem Start läuft ContextCruncher **im Hintergrund**. Es öffnet kein Fenster,
sondern legt ein **kleines rotes Symbol unten rechts in der Taskleiste** ab (neben
der Uhr, evtl. unter dem kleinen Pfeil „^"). Ein **Rechtsklick** auf dieses Symbol
öffnet das Menü mit allen Funktionen und den Einstellungen.

Die wichtigsten Tastenkürzel (funktionieren überall in Windows):

| Tastenkombination | Funktion |
|---|---|
| **Strg + Umschalt + F11** | Bildausschnitt aufnehmen (Screenshot eines Bereichs) |
| **Strg + Umschalt + F10** | Aktives Fenster als Bild aufnehmen |
| **Strg + Umschalt + F9** | Text vom ganzen Bildschirm einlesen (OCR) |
| **Strg + Umschalt + Einfg** | Text aus einem markierten Bereich einlesen (OCR) |
| **Strg + Umschalt + F7** | Zwischenablage-Text für die KI verkleinern |
| **Strg + Umschalt + L** | Verlauf durchsuchen |
| **Strg + Umschalt + H** | Token-/Kosten-Übersicht anzeigen |

> „Umschalt" ist die **Shift**-Taste. Alle Kürzel lassen sich im Menü unter
> **Einstellungen** ändern, und eine komplette **Kurzübersicht** findest du im
> Taskleisten-Menü unter **„Hotkey Cheat-Sheet"**.

Beim allerersten Start bietet dir ein kleines Willkommensfenster an, die
**Druck-Taste (Druck / PrtScn)** für schnelle Screenshots zu verwenden — praktisch,
weil diese Taste sonst kaum gebraucht wird.

Zum **Beenden**: Rechtsklick auf das Taskleisten-Symbol → **Beenden**.

---

## 🌐 Optional: Browser-Erweiterung

Im Release liegt zusätzlich eine **`browser_extension.zip`**. Damit kannst du in
Chrome/Edge ganze Webseiten als Bild aufnehmen und Text direkt im Browser
verkleinern. Sie ist **optional** — für die normale Nutzung brauchst du nur die
`.exe`.

> ⚠️ **Browser können ZIP-Dateien nicht direkt laden** — du musst sie zuerst
> entpacken. Eine `INSTALL.txt` mit derselben Anleitung liegt in der ZIP.

**So installierst du sie (Chrome / Edge / Brave):**

1. `browser_extension.zip` **entpacken** (Rechtsklick → „Alle extrahieren…").
   Du bekommst einen Ordner `browser_extension`, in dem `manifest.json` liegt.
2. In die Adresszeile `chrome://extensions` eingeben (bei Edge: `edge://extensions`).
3. Oben rechts **„Entwicklermodus"** einschalten.
4. Auf **„Entpackte Erweiterung laden"** klicken.
5. Den Ordner **`browser_extension`** auswählen — also den, in dem `manifest.json`
   **direkt** liegt (nicht den übergeordneten Entpack-Ordner).

**Tipp:** Lege den entpackten Ordner `browser_extension` am besten **direkt neben
die `ContextCruncher.exe`**. Dann findet das Programm ihn automatisch und der
Knopf „AddOn-Ordner öffnen" in den Einstellungen funktioniert:

```
Dein Ordner\
   ├── ContextCruncher.exe
   └── browser_extension\
       └── manifest.json
```

**Firefox** lädt unsignierte Erweiterungen nur vorübergehend: Adresszeile
`about:debugging#/runtime/this-firefox` → „Temporäres Add-on laden…" → die
`manifest.json` auswählen. Das muss nach jedem Firefox-Neustart wiederholt werden.

---

## 🔒 Hinweis zum Quellcode

Hier gibt es **nur das fertige Programm** zum Herunterladen. Der Quellcode ist
privat und wird nicht veröffentlicht.
