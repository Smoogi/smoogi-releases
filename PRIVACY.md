# Privacy policy: Smoogi's Music Player

Last updated: 12 November 2026

**In short:** the app does not collect, send or share any data about you. It works offline. It uses the internet only when you press a button that needs it, and then it sends only what is listed below.

## What the app stores, and where

Everything the app learns or you create lives in the app's own storage on your phone and is removed when you uninstall the app:

- the list of your songs and what it read from them (titles, artists, albums, covers, lengths),
- your playlists, favorites, hidden songs, play history and counts,
- your edits to song details, covers you chose, and results of lookups you applied,
- your settings, and the keys you pasted for optional sources (see below).

Your music files are only read. The app never changes them. The developer cannot see any of this: there is no account, no server, no analytics, no crash reporting and no advertising in the app.

## What the app asks Android for

- **Access to music files**, to find and play the songs in the folders you chose. It scans only those folders.
- **Notifications and a foreground service**, for the playback notification and for a batch lookup that keeps running while the phone is locked.
- **Internet**, only for the features below.
- **Modify system settings**, only if you use Set as ringtone.

## When the app uses the internet

Only when you press the button for it. Nothing is sent in the background or at start-up.

| What you press | Where the request goes | What is sent |
|---|---|---|
| Search online / Batch lookup | musicbrainz.org, and coverartarchive.org for covers | the title, artist and album of the song(s) you look up |
| Ask other sources, or Test, on a source you switched on | query.wikidata.org (Wikidata), ws.audioscrobbler.com (Last.fm), api.discogs.com (Discogs), www.theaudiodb.com (TheAudioDB) | the artist and title of the song (for Wikidata, the MusicBrainz ids of the match); for Last.fm, Discogs and optionally TheAudioDB, the key you pasted |
| Check for updates | api.github.com | a request for the newest release of the app's releases page; nothing about you |

Those services have their own privacy policies and may log the request as any web service does (for example your IP address). The developer does not receive or see these requests.

Keys you paste for Last.fm, Discogs or TheAudioDB stay on your phone and are not included in backups.

## Backups

Backup & Restore writes a file where you choose; it is yours and is not uploaded anywhere. The app also keeps a copy of its own database on the phone before an update that changes how data is stored.

## Children

The app has no accounts, no social features and collects nothing, so it collects no data from children either.

## Changes and contact

If this changes, the new text is published here with a new date. Questions: open an issue on this page (the Issues tab).
