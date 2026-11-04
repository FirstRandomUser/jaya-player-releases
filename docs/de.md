# Jaya Player — Anleitung

Jaya Player ist ein IPTV-Player für Android TV, TV-Boxen und Smartphones.
Die App **stellt keine Fernsehsender oder Inhalte bereit**: Sie spielt nur Playlists ab, die der Nutzer selbst hinzufügt.

---

## 1. Installation

1. App herunterladen: **https://github.com/FirstRandomUser/jaya-player-releases/releases/latest/download/jaya-player.apk** (immer die neueste Version) oder über die Seite [Releases](https://github.com/FirstRandomUser/jaya-player-releases/releases/latest).
2. Auf einer TV-Box ist die App **Downloader** oder ein USB-Stick praktisch.
3. Bei der ersten Installation fragt Android, ob Installationen aus dieser Quelle erlaubt werden — erlauben.
4. Android 6.0 oder neuer ist erforderlich.

Weitere Updates lädt und installiert die App **selbst** (siehe Abschnitt 10).

---

## 2. Erster Start und Playlist

Beim ersten Start öffnen sich die **Einstellungen**.

1. **Playlists → Hinzufügen** drücken.
2. Typ wählen:
   - **M3U-Link** — Playlist-Adresse vom Anbieter;
   - **Xtream Codes** — Serveradresse, Login und Passwort;
   - **Datei** — `.m3u`-Playlist vom Gerät oder USB-Stick.
3. **EPG** (Programmführer) — XMLTV-Adresse. Meist ist sie bereits in der Playlist des Anbieters enthalten, das Feld kann leer bleiben. Fehlt der Programmführer, fragen Sie Ihren Anbieter nach der EPG-Adresse und tragen Sie sie hier ein.
4. **Aktualisieren alle … Std.** — wie oft Playlist und Programmführer aktualisiert werden.
5. **Speichern** drücken. Das Laden läuft im Hintergrund — Sie können sofort weiterschauen.

Mehrere Playlists sind möglich. Schlägt ein Update fehl (z. B. kein Internet), wiederholt die App es beim nächsten Start automatisch.

---

## 3. Fernbedienung

| Taste | Aktion |
|---|---|
| ▲ ▼ | vorheriger / nächster Sender |
| ◀ | Senderliste |
| ◀ ◀ (weiter links) | Gruppenliste |
| ▶ | Favoriten |
| ▶ ▶ (schnell zweimal) | Stream-Statistik (ein/aus) |
| OK | Infoleiste |
| OK erneut | Pause |
| OK in der Pause | fortsetzen |
| langes OK | Aktionsmenü (Ton, Untertitel, Format, Einstellungen) |
| Ziffern | Sender per Nummer wählen |
| 0 | vorheriger Sender |
| zweimal Zurück | Beenden |

**In der Senderliste:**
- ▶ — Programmführer des gewählten Senders;
- langes OK — Markiermodus: ◀ zu Favoriten hinzufügen/entfernen, ▶ Sender löschen (gelöschte lassen sich in der Gruppe „Gelöscht“ wiederherstellen).

**Auf dem Smartphone:** Tippen — Pause und Infoleiste; nach oben wischen — Infoleiste, nach unten — ausblenden; auf der linken Hälfte nach rechts wischen — Senderliste; auf der rechten Hälfte nach links — Favoriten; langes Tippen — Einstellungen.

---

## 4. Programmführer und Archiv

- Der Programmführer wird **24 Stunden zurück und 48 Stunden voraus** gespeichert.
- In der Senderliste ▶ drücken — der Programmführer öffnet sich. Vergangene Sendungen lassen sich im **Archiv** ansehen, wenn der Anbieter es unterstützt.
- Im Archiv: **OK** — Spulleiste, ◀ ▶ — Schritt (beim Halten schneller), **Zurück** — zurück zum Live-Programm.

---

## 5. Live-Pause (Timeshift)

**Einstellungen → Wiedergabe → Live-Pause mit Aufnahme.**

- **Aus:** Pause hält das Bild an; nach dem Fortsetzen läuft wieder live.
- **Ein:** Nach der Pause geht es **an derselben Stelle** weiter. Der Rückstand zum Live-Bild wird unten angezeigt; **Zurück** — zu live.

**Speicher für die Live-Pause:**
- **Interner Speicher** — die Aufnahme beginnt im Moment der Pause und wird beim Senderwechsel gelöscht.
- **Externes Laufwerk (USB)** — die Aufnahme läuft ständig, solange Sie einen Sender sehen, daher **spulen ◀ ▶ in der Pause zurück** (so weit der Platz reicht). Die App legt auf dem Laufwerk den Ordner `Timeshift` an und nutzt höchstens 80 % des freien Platzes; alte Aufnahmen werden automatisch gelöscht.

USB-Laufwerk: FAT32 oder exFAT (NTFS, falls Ihr Gerät es unterstützt).
DASH-Streams, verschlüsselte Streams und Streams mit separater Tonspur werden nicht unterstützt — dort funktioniert die Pause wie gewohnt.

---

## 6. Versteckte Gruppen (Kindersicherung)

1. Gruppenliste öffnen (◀ ◀), eine Gruppe wählen und **OK gedrückt halten** — die Gruppenauswahl startet.
2. Gruppen mit OK markieren und **Zurück** drücken.
3. Passwort mit den Pfeiltasten eingeben und OK drücken. Standardpasswort: **▶ ▶ ▶ ▶**.
4. Nach dem ersten Ausblenden bietet die App an, ein eigenes Pfeil-Passwort festzulegen (z. B. ▲ ▲ ◀ ▶) — merken Sie es sich.

Um versteckte Gruppen wieder anzuzeigen, in der Gruppenliste **dreimal schnell ◀ drücken** und das Passwort eingeben. Beim Minimieren der App werden die Gruppen wieder versteckt.

---

## 7. Bild-in-Bild und Hintergrund (Smartphone)

- **Bild-in-Bild:** Beim Wechsel zum Startbildschirm läuft das Video in einem kleinen Fenster weiter.
- **Ton im Hintergrund:** Der Ton läuft bei gesperrtem Bildschirm weiter; Steuerung über die Benachrichtigungsleiste.

---

## 8. Einstellungen

- **Bildschirm:** automatische Bildrate, 120 Hz, Anzeigedauer der Infoleiste, Listen-Scrollen, **OLED-Bildschirm** (Einbrennschutz: Verschieben von Elementen, Ausblenden der Uhr, Bildschirmschoner in der Pause, Abdunkeln der Menüs).
- **Uhr:** Position auf dem Bildschirm.
- **Wiedergabe:** Bild-in-Bild, Ton im Hintergrund, Lautstärkeausgleich, Statistik, Live-Pause, Vorladen benachbarter Sender, Puffer, User-Agent.
- **Designs** (eigene Schaltfläche „Designs“ in den Einstellungen): fertige Designs (Klassisch, OLED-Schwarz, Ozean, Warm, Glas) oder eigene Farben für Panels, Auswahl, Text, Infoleiste, Uhr sowie Transparenz.
- **Verwaltung:** Passwort und Sperren von Einstellungen (gesperrte Punkte werden ausgeblendet).

**User-Agent** ist, wie sich der Player beim Server des Anbieters „vorstellt“. Lädt die Playlist, aber Sender öffnen sich nicht, probieren Sie **VLC**.

---

## 9. Sicherung

**Einstellungen → Über die App → Export** speichert Playlists, Favoriten, versteckte Gruppen und Einstellungen in einer Datei. **Import** stellt sie wieder her — z. B. auf einem neuen Gerät.

---

## 10. Updates

- Die App prüft, lädt und installiert Updates selbst (abschaltbar unter **Über die App**).
- Vor der Installation wird die Signatur geprüft — ein Update kann nicht gefälscht werden.
- Konnte die App **90 Tage** lang nicht nach Updates suchen, wird ein eingeschränkter Modus aktiv (kein Programmführer und Archiv, 5 Favoriten). Einfach mit dem Internet verbinden — alles kommt zurück.

---

## 11. Pro-Version

Derzeit sind alle Funktionen **kostenlos**. Wenn Pro erscheint, erhält jeder weitere **3 Monate** vollen Zugriff.

| | Kostenlos | Pro |
|---|---|---|
| Qualität | bis 1080p (4K/HDR — 3 Minuten) | 4K, HDR |
| Favoriten | 20 Sender | unbegrenzt |
| Versteckte Gruppen | 1 | unbegrenzt |
| Archiv | letzte 3 Stunden | so viel der Anbieter bietet |
| Lautstärkeausgleich, automatische Bildrate, 120 Hz, AC3/DTS an Receiver | — | ✓ |
| Live-Pause mit Aufnahme, Designs | — | ✓ |
| Bild-in-Bild und Ton im Hintergrund (Smartphone) | — | ✓ |

---

## 12. Fehlerbehebung

- **Sender öffnet sich nicht** — User-Agent wechseln (VLC); Playlist auf einem anderen Gerät prüfen.
- **Kein Programmführer** — EPG-Adresse in der Playlist prüfen; **Playlists** öffnen — dort steht der Ladefehler.
- **Knackender Ton auf dem Smartphone mit Lautstärkeausgleich** — Ausgleich ausschalten.
- **4K ruckelt auf einer schwachen TV-Box** — Puffer „Groß“ wählen oder in HD schauen.

---

## 13. Geräte verbinden und Qualität

- **Geräte verbinden** (Einstellungen → Geräte verbinden): Handy per Code mit dem Fernseher koppeln — der Code erscheint automatisch auf dem TV. Playlists und Einstellungen senden, Playlist per QR-Code im Browser hinzufügen, vom Handy auf den TV übertragen (📺, das Handy wird zur Fernbedienung) und zurückholen.
- **Qualität** (Infoleiste): „Auto“ senkt die Qualität bei langsamem Netz; „Beste“ nutzt immer die höchste. Pro Sender gespeichert.
- **Puffer „Auto“**: wächst bei häufigem Nachladen automatisch.

---

## 14. Komfort

- **Erinnerungen:** im Programmführer OK auf einer künftigen Sendung — Markierung ◉, eine Minute vor Beginn erscheint „Umschalten“.
- **Favoriten:** langes OK — ▲▼ sortieren, OK benennt um.
- **Sendung auf dem Bildschirm**, **Oberflächengröße**, **Autostart**, neues Design **„Neon“**.

---

© 2026 Ruslan G. Alle Rechte vorbehalten.
