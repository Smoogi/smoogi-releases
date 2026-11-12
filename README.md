# Smoogi's Music Player

### 📥 Download

[![Download Latest Release](https://img.shields.io/badge/Download-Latest%20APK-2ea44f?style=for-the-badge&logo=android)](https://github.com/Smoogi/smoogi-releases/releases/latest)

Download the latest version from GitHub Releases.


A free music player for Android that works fully offline. It plays the music files that are on your phone, in the folders you choose, and keeps everything it learns about them on the phone.

This page holds the **test releases**. The newest one is under **Releases** on the right.

## Install

1. Open the newest release and download `smoogi-music-player-<version>.apk` (the `.sha256` file is only a checksum, you do not install it).
2. Open the downloaded file. Android may ask once to allow installs from your browser; allow it for this install.
3. Open **Smoogi**, choose your music folder(s) and allow access to music files.

Needs Android 10 or newer and a 64-bit ARM phone (almost every phone since 2017).

## Update

Download the newer `.apk` from Releases and open it: it installs over the old version and keeps your library, playlists and settings. Or, in the app: **Settings > App updates > Check for updates**, which opens the release page for you. The app never checks by itself.

## What it does

- Library by songs, artists and albums, search, favorites, hidden songs, play counts and statistics.
- Playlists, smart playlists with rules (including genre, year, play counts), M3U import and export.
- Smart Shuffle with adjustable weights, a play queue with tabs, fades, dynamic volume, equalizer, skip-silence, playback speed.
- Metadata editing (title, artist, album, genre, cover...), with a paste-from-clipboard helper, kept in the app only: your music files are never modified.
- Optional online lookup of a song's details and cover (MusicBrainz and the Cover Art Archive), one search per press; a batch lookup for up to 100 songs that keeps going while the phone is locked.
- Optional extra sources you switch on yourself (Wikidata, Last.fm, Discogs, TheAudioDB; the last two need your own free key).
- Library Health, same-artist and same-album grouping (nothing is merged without your say), Backup & Restore.
- Skins (Material, Cyberpunk, Frutiger Aero).

## Privacy

- No account, no cloud, no analytics, no ads, no background network use. The app does not check for updates, look anything up or send anything on its own.
- The internet permission is used only when you press something: a lookup (sends the title, artist and album of the song you are looking up), "Ask other sources" or Test on a source you turned on (sends the artist and title of that song, and your own key), or "Check for updates" (asks GitHub for the newest release, nothing about you).
- Keys you paste for Last.fm or Discogs stay on your phone and are not included in backups.
- Other permissions: music files (to play them), notifications and a foreground service (the playback notification, and a running batch lookup), "modify system settings" (only for Set as ringtone).
- Your music files are only read. Everything the app adds (edits, lookups, covers, playlists, counts) is in the app's own storage.

## Backup & Restore

Settings > Backup & Restore saves one file, wherever you choose, with your settings, playlists, smart playlists, favorites, hidden songs, play history and counts, and your metadata edits and lookup results (optionally the cover pictures). It holds no music. Songs are recognised again on another phone, or after a reinstall, by their audio, file name or title and artist.

The same-artist and same-album groups you made are included too. Not included: your music files and the details stored inside them, the music folders you chose, the play queue and your online-source keys.

Before an update changes how the app stores its data, the app also copies its database on the phone itself; if an update breaks something, Backup & Restore offers to put that copy back. It stays on the phone, so save a profile somewhere else before updating, to be safe.

## Known issues

- Cover art on a car's display over Bluetooth depends on the phone's Bluetooth.
- This is a test version: please expect rough edges and tell me about them.

## Problems and ideas

Open an issue on this page (the Issues tab) with what you did, what you expected and what happened, your phone model and the version under Settings > App updates. Song titles are not needed. If it is about covers on a car or the lock screen, Settings > Diagnostics > Media session log can record what the app hands to Android; turn it on, reproduce the problem, press Copy all and paste it into the issue (it contains song titles).
