# Jaya Player — user guide

Jaya Player is an IPTV player for Android TV, TV boxes and smartphones.
The app **does not provide any TV channels or content**: it only plays playlists that the user adds.

---

## 1. Installation

1. Download the app: **https://github.com/FirstRandomUser/jaya-player-releases/releases/latest/download/jaya-player.apk** (always the latest version) or from the [Releases](https://github.com/FirstRandomUser/jaya-player-releases/releases/latest) page.
2. On a TV box, the **Downloader** app or a USB stick is convenient.
3. On first install Android asks to allow installs from this source — allow it.
4. Android 6.0 or newer is required.

After that, the app downloads and installs updates **by itself** (see section 10).

---

## 2. First launch and playlist

**Settings** open on first launch.

1. Press **Playlists → Add**.
2. Choose the type:
   - **M3U link** — the playlist address from your provider;
   - **Xtream Codes** — server address, login and password;
   - **file** — an `.m3u` playlist from the device or a USB stick.
3. **EPG** (TV guide) — an XMLTV address. Usually it is already included in the provider's playlist, so the field can stay empty. If there is no TV guide, ask your provider for the EPG address and enter it here.
4. **Update every … h** — how often to update the playlist and the TV guide.
5. Press **Save**. Loading runs in the background — you can go back to watching right away.

You can add several playlists. If an update fails (for example, no internet), the app retries automatically on the next launch.

---

## 3. Remote control

| Button | Action |
|---|---|
| ▲ ▼ | previous / next channel |
| ◀ | channel list |
| ◀ ◀ (further left) | group list |
| ▶ | Favourites |
| ▶ ▶ (double press) | stream statistics (on/off) |
| OK | info panel |
| OK again | pause |
| OK while paused | resume |
| long OK | action menu (audio, subtitles, aspect, settings) |
| digits | go to channel by number |
| 0 | previous channel |
| Back twice | exit |

**In the channel list:**
- ▶ — TV guide of the selected channel;
- long OK — marking mode: ◀ add/remove from Favourites, ▶ delete the channel (deleted channels can be restored from the "Deleted" group).

**On a smartphone:** tap — pause and info panel; swipe up — info panel, down — hide it; swipe right on the left half — channel list; swipe left on the right half — Favourites; long tap — settings.

---

## 4. TV guide and archive

- The TV guide is kept for **24 hours back and 48 hours ahead**.
- Press ▶ in the channel list to open the TV guide. Past programmes can be watched from the **archive** if your provider supports it.
- In the archive: **OK** — seek bar, ◀ ▶ — step (speeds up when held), **Back** — return to live.

---

## 5. Live pause (Timeshift)

**Settings → Playback → Live pause with recording.**

- **Off:** pause stops the picture; after resuming you are back to live.
- **On:** after a pause, watching continues **from the same moment**. The delay behind live is shown at the bottom; **Back** — return to live.

**Live pause storage:**
- **Internal memory** — recording starts at the moment of pause and is deleted when you switch channels.
- **External drive (USB)** — recording runs all the time while you watch a channel, so **while paused ◀ ▶ rewind** (as far as space allows). The app creates a `Timeshift` folder on the drive and uses at most 80 % of free space; old recordings are deleted automatically.

USB drive: FAT32 or exFAT (NTFS if your device supports it).
DASH streams, encrypted streams and streams with a separate audio track are not supported — pause works the normal way on them.

---

## 6. Hidden groups (parental control)

1. Open the group list (◀ ◀), select a group and **hold OK** — group selection turns on.
2. Mark groups with OK and press **Back**.
3. Enter the password with the arrows and press OK. The default password is **▶ ▶ ▶ ▶**.
4. After the first hiding, the app offers to create your own arrow password (e.g. ▲ ▲ ◀ ▶) — remember it.

To show hidden groups again, **press ◀ three times quickly** in the group list and enter the password. Groups are hidden again when the app is minimised.

---

## 7. Picture-in-picture and background (smartphone)

- **Picture-in-picture:** when you go to the home screen, video continues in a small window.
- **Background audio:** audio continues when the screen is locked; controls are in the notification shade.

---

## 8. Settings

- **Screen:** automatic frame rate, 120 Hz, info panel duration, list scrolling, **OLED screen** (burn-in protection: element shifting, hidden clock, pause screensaver, menu dimming).
- **Clock:** position on screen.
- **Playback:** picture-in-picture, background audio, volume levelling, statistics, live pause, preloading of neighbouring channels, buffer, User-Agent.
- **Themes** (separate "Themes" button in settings): ready-made themes (Classic, OLED black, Ocean, Warm, Glass) or your own colours of panels, selection, text, info panel, clock and transparency.
- **Administration:** password and locking of settings items (locked items are hidden).

**User-Agent** is how the player "introduces itself" to the provider's server. If the playlist loads but channels do not open, try **VLC**.

---

## 9. Backup

**Settings → About → Export** saves playlists, Favourites, hidden groups and settings to a file. **Import** restores them — for example, on a new device.

---

## 10. Updates

- The app checks, downloads and installs updates by itself (can be turned off in **About**).
- The signature is verified before installing — an update cannot be forged.
- If the app could not check for updates for **90 days**, a restricted mode turns on (no TV guide or archive, 5 Favourites channels). Just connect to the internet — everything comes back.

---

## 11. Pro version

Right now all features are **free**. When Pro arrives, everyone gets another **3 months** of full access.

| | Free | Pro |
|---|---|---|
| Quality | up to 1080p (4K/HDR — 3 minutes) | 4K, HDR |
| Favourites | 20 channels | unlimited |
| Hidden groups | 1 | unlimited |
| Archive | last 3 hours | as much as the provider offers |
| Volume levelling, automatic frame rate, 120 Hz, AC3/DTS to receiver | — | ✓ |
| Live pause with recording, themes | — | ✓ |
| Picture-in-picture and background audio (smartphone) | — | ✓ |

---

## 12. Troubleshooting

- **A channel does not open** — change the User-Agent (VLC); check the playlist on another device.
- **No TV guide** — check the EPG address in the playlist; open **Playlists** — the loading error is shown there.
- **Crackling audio on a smartphone with volume levelling** — turn levelling off.
- **4K stutters on a weak TV box** — choose the "Large" buffer or watch in HD.

---

## 13. Connecting devices and quality

- **Connect devices** (Settings → Connect devices): pair a phone with the TV by code — the code appears on the TV automatically. Send playlists and settings, add a playlist from a browser via QR code, cast from the phone to the TV (📺 button, the phone becomes a remote) and take playback back. Connected devices can be renamed and removed.
- **Quality** (info panel): “Auto” lowers quality on a slow network (if the channel offers several); “Best” always uses the highest. Remembered per channel.
- **“Auto” buffer**: the buffer grows automatically on frequent rebuffering.

---

## 14. Convenience

- **Reminders:** in the TV guide press OK on a future programme — it is marked ◉, and a “Switch” window appears a minute before it starts.
- **Favourites:** long OK — marking mode; ▲▼ reorder channels, OK renames a channel.
- **Programme on screen** (Settings → Screen): current programme title over the video, with position, size, background and colour.
- **Interface size:** normal, large, extra large. **Autostart** with the device (Settings → Playback).
- **Themes:** new “Neon” theme; settings in a strict metallic style.

---

© 2026 Ruslan G. All rights reserved.
