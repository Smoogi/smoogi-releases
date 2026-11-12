# Privacy policy: Smoogi's Music Player

Last updated: 12 November 2026

**In short:** the app has no accounts, no analytics, no crash reporting, no advertising and no trackers, and the developer receives nothing from it. Playing music and managing your library work fully offline. The app uses the internet only for features you start yourself, and then it sends only what is listed below.

## What the app stores, and where

Everything the app learns or you create is stored in the app's own private storage on your phone:

- the list of your songs and what it read from them (titles, artists, albums, covers, lengths),
- your playlists, favorites, hidden songs, play history and counts,
- your edits to song details, covers you chose or downloaded, and results of lookups you applied,
- your settings, and the keys you pasted for optional sources (see below).

Your music files are only read during playing, scanning and lookups. Edits to song details are kept in the app's own storage; the app does not write them into your audio files. The one exception to "only read" is deleting: if you choose **Delete** on a song, the app asks Android to delete that file, and Android asks you to confirm.

The app turns off Android's automatic backup and device-to-device transfer for its data. Its data is not uploaded to Google or any other cloud by the app.

## What stays when you uninstall

Uninstalling removes the app's private storage: the library, playlists, play history, settings, downloaded covers and pasted keys. It does not remove:

- your music files,
- backup files you saved with **Backup & Restore**, including the automatic backups in the folder you chose,
- playlist files you exported (.m3u8),
- anything else you saved or copied outside the app.

Delete those yourself if you no longer want them.

## What the app asks Android for

- **Access to music files** (`READ_MEDIA_AUDIO`; on Android 12 and older, storage read access), to find and play the songs in the folders you chose. It scans only those folders. If you choose a folder for automatic backups, the app can read and write in that folder only.
- **Notifications and foreground services**, for the playback notification, and for a batch lookup or applying its results while the phone is locked. These show a visible notification with a Stop button. The app also holds a wake lock so playback and those tasks are not cut off.
- **Internet**, only for the features below.
- **Modify system settings**, only if you use Set as ringtone.

While a song plays, Android shares its title, artist and cover with the lock screen, the notification and any connected device such as a car or Bluetooth headphones.

## When the app uses the internet

Only when you start it: by pressing a button, or by starting a batch lookup. The one exception is the optional **Check once a day** in Settings > App updates, which is off until you switch it on. Nothing else is sent at start-up, and the app makes no requests while it is closed.

| What you start | Where the request goes | What is sent |
|---|---|---|
| Search online / Batch lookup | musicbrainz.org, and coverartarchive.org for covers (which may forward the picture request to the Internet Archive, archive.org) | the title, artist and album of the song(s) you look up; for covers, the id of the matched release |
| Ask other sources, or Test, on a source you switched on | query.wikidata.org (Wikidata), ws.audioscrobbler.com (Last.fm), api.discogs.com (Discogs), www.theaudiodb.com (TheAudioDB) | the artist and title of the song (for Wikidata, the MusicBrainz ids of the match); for Last.fm and Discogs the key you pasted, and for TheAudioDB your key if you pasted one, otherwise its public test key |
| Check for updates (button), or Check once a day if you switched it on (at most once every 24 hours, only while the app is open) | api.github.com | a request for the newest release of the app's releases page; nothing about you |
| Support the app, Privacy policy | ko-fi.com or github.com, in your browser | nothing from the app: it only opens the page, and that site's own policy applies there |

A **batch lookup** searches up to 100 songs one after another. If you lock the phone or switch to another app while it runs, it keeps going, with its notification showing, until it finishes, you tap Stop, or you leave its screen. Applying the matches you ticked (which can download covers) also continues in the background until it is done.

Like any web request, these reach the service together with technical information such as your IP address and the app's name in the request header, and the service may log them under its own privacy policy. The app does not collect or store those addresses, and the developer does not receive or see these requests.

Keys you paste for Last.fm, Discogs or TheAudioDB are stored as plain text in the app's private storage (the app does not encrypt them; Android keeps that storage private to the app). They are not included in Backup & Restore files, and the app does not write them to its logs.

## Backups

**Backup & Restore** writes a file where you choose (or, with **Automatic backups**, into the folder you chose, when the app is open and a backup is due). The file is yours and the app does not upload it anywhere. It holds your playlists, favorites, play history, edits and settings, and cover pictures if you include them; it does not hold your music files or your pasted keys. Before an update that changes how data is stored, the app also keeps a copy of its own database in its private storage. That copy includes your pasted keys and is removed on uninstall.

## Children

The app has no accounts, no social features and collects no data, so it collects no data from children either.

## Changes and contact

If this changes, the new text is published here with a new date. Questions or problems: open an issue at https://github.com/Smoogi/smoogi-releases/issues (the Issues tab of this page). Please do not post personal information or keys there.
