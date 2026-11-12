# Smoogi's Music Player

### 📥 Download

[![Download Latest Release](https://img.shields.io/badge/Download-Latest%20APK-2ea44f?style=for-the-badge&logo=android)](https://github.com/Smoogi/smoogi-releases/releases/latest)

Download the latest version from GitHub Releases.

## About


Smoogi's Music Player is a free, offline music player for Android that I originally made for myself because I couldn't find one that worked exactly how I wanted.


The main feature is Smart Shuffle, which lets you adjust how often favorites, newly added songs, and tracks you haven't listened to in a while show up. You can also reduce the chances of recently played or frequently skipped songs appearing.


Over time, I've added quite a few other features:




Playback: Multiple queues, gapless playback, volume normalization, equalizer, silence skipping, and more.


Library: Duplicate detection, metadata editing, batch lookup, and tools for organizing your music.


Playlists: Regular playlists and smart playlists that update automatically based on your rules.


Customization: Different UI skins, themes, and customizable controls.




Everything works locally, except optional metadata lookups that you start yourself.


No ads, no subscriptions, no accounts, and no locked features. Just a music player.



**Contents:** [Install and update](#install-and-update) · [Playing music](#playing-music) · [Queue](#queue) · [Shuffle](#shuffle) · [Sound](#sound) · [Library and browsing](#library-and-browsing) · [Playlists](#playlists) · [Song details and covers](#song-details-and-covers) · [Online lookup](#online-lookup-optional) · [Keeping the library tidy](#keeping-the-library-tidy) · [Statistics](#statistics) · [Looks](#looks) · [Backup and restore](#backup-and-restore) · [Privacy](#privacy) · [Known issues](#known-issues)

---

## Install and update

1. Open the newest release and download `smoogi-music-player-<version>.apk` (the `.sha256` file is only a checksum; you do not install it).
2. Open the downloaded file. Android may ask once to allow installs from your browser; allow it for this install.
3. Open **Smoogi**, choose your music folder(s) and allow access to music files.

Needs Android 10 or newer and a 64-bit ARM phone (almost every phone since 2017).

**Updating:** download the newer `.apk` and open it; it installs over the old version and keeps your library, playlists and settings. Or use **Settings > App updates > Check for updates**, which opens the release page for you. The app never checks by itself. Save a profile first (see [Backup and restore](#backup-and-restore)) to be safe.

---

## Playing music

- **Background playback** with a media notification, lock-screen controls, headset and Bluetooth buttons, and the cover of the playing song on the notification and the lock screen.
- **Now Playing screen:** large cover, seek bar, previous / play-pause / next, and a second row with Shuffle, Options and Repeat. Pull the page down to close it. A long press on the cover opens the same menu as a long press on a song.
- **Customisable controls:** put the Shuffle, Options and Repeat buttons in the order you like and show or hide their names (Settings > Now Playing Controls).
- **Time left:** tap the time at the right of the seek bar to switch between the song's length and the time that is left.
- **Playback options** (the Options button): sleep timer (15, 30, 45 or 60 minutes, with a fade-out at the end), **stop after this song**, playback speed from 0.5x to 2.0x with the pitch kept, and **A-B repeat** to loop a part of a song.
- **Repeat** off, all or one. Playback resumes where you left it after the app is closed.
- **Skip silent intros and outros:** two separate switches (off by default). The app listens to each song once, in the background, finds silence at the start or the end and skips it. It never skips more than 10 seconds at each end, never touches short songs, and leaves a song alone when it is not sure.
- **Fade between songs:** off, or 2 to 10 seconds. The end of a song fades out and the next fades in (a fade, not an overlapping crossfade).
- Songs play back to back without a gap where the files allow it.
- A song that cannot be played is skipped with a message; if nothing in the queue can be played, playback stops and says so.
- The system **back button** closes pages one by one and, at the top of a tab, leaves the app while the music keeps playing.

## Queue

- The **queue panel** under the player starts at the playing song. Reorder it, remove songs from it, and tap a song to jump to it.
- **Queue tabs**, like browser tabs: several queues at once, one of them playing. Tap a tab to play that queue where you left it, the plus opens a new empty queue, long-press a tab to rename it, clear it or close it. Each tab remembers its songs, order, shuffle, repeat, current song and position.
- **Play next** and **Add to queue** from any song menu.
- The queue (with the original order, so turning shuffle off restores it) is saved and comes back after a restart.

## Shuffle

- **Normal shuffle:** every song equally likely, a fresh random order each time.
- **Smart Shuffle** (Settings > Shuffle) with a switch for each idea, all adjustable:
  - **Prioritize favorites** with an intensity.
  - **Prioritize new songs:** one or several time windows (7, 15, 30 days or your own), each with its own boost. The smallest window a song fits in decides.
  - **Discovery:** songs you have not played for a long time (or ever) get a boost, in tiers you can add and edit.
  - **Cooldown:** songs you heard recently come up less often, with a strength and a "last N songs" memory.
  - **Skipped a lot:** songs you often press Next on within the first seconds are played less. It needs at least 5 plays or skips of a song before it judges, and it never excludes a song.
  - **Leave out long songs:** a limit in minutes, so that a 40-minute mix does not come up in the middle of a shuffle.
  - **Guarantee favorites up front:** a share of favorites among the first songs.
  - A **randomness cap** so that a strongly boosted song cannot take over, and so that a lowered song keeps a real chance.
  - **Presets:** save the current settings under a name, load them later, reset to the defaults.
  - A **live preview** that shows how the settings would change 200 simulated shuffles.
- Shuffle buttons on the library, albums, artists, playlists and favorites start from the shuffled order. On a smart playlist you can choose Normal or Smart for a single press without changing your setting.
- Turning shuffle on or off while a song plays does not interrupt it.
- Hidden and missing songs are never part of a shuffle.

## Sound

- **Equalizer:** on/off, ten presets (Flat, Rock, Pop, Jazz, Classical, Bass boost, Treble boost, Vocal, Dance, Loudness), your own curve with one slider per band of the phone, and a loudness boost.
- **Dynamic volume ("Even out the volume"):** every song gets a gain so that songs sit at the same loudness. Match the first song you start with, or use a fixed level. Optionally turn quiet songs up too. Loudness is measured once per song (the standard EBU R128 / LUFS measurement), kept on the phone, and the page shows the progress, an estimate of the time left, and lets you stop and continue.

## Library and browsing

- **You choose the folders** (Settings > Folders & Scanning). Add folders, exclude sub-folders, and the app scans only those. Nothing else on the phone is scanned.
- The library is on screen as soon as the first scan has listed the files; the rest (recognising files, reading tags and covers) goes on in the background.
- **Optional deep scan** for folders that Android does not list (for example with a `.nomedia` file).
- **Rescan** from the button, at start and when you come back to the app, so a song downloaded by another app shows up without doing anything.
- **Moved or renamed files** are recognised by their audio, so favorites, counts and playlists follow them.
- **Songs, Browse (Artists and Albums), Playlists, Misc, Settings:** five tabs you can put in your own order. Artists show a fan of their album covers.
- **Search** by song, artist, album and genre, fast also in big libraries and with Japanese and other scripts.
- **Favorites** and **Hidden songs** (hide a song from the library without deleting it; hidden songs keep their place in playlists and can be shown again).
- **When a file name has no "Artist - Title":** choose whether the folder name or "Unknown Artist" is used.
- **Song menu** (long press): play next, add to queue, add to playlist, favorite, edit details, hide, **details** (format, bit rate, size, folder, dates, counts), **share** the audio file, **set as ringtone**, and **delete from device** (with Android's own confirmation).
- Built and tested for libraries of a few thousand songs.

## Playlists

- Create, rename, delete and reorder playlists. Adding skips duplicates.
- **Smart playlists** built from rules that update by themselves:
  - on the song's details (artist, album, album artist, genre, title, composer, year, track and disc number), the file name, the folder, the length, when it was added, how often and when it was last played, and whether it is in Japanese script;
  - groups of "match all" or "match any", and a NOT on any rule or group;
  - a live "N songs match" count, suggestions from your own library while you type, and ready-made starting points (songs by an artist, songs of a genre, from the 1980s, Japanese and non-Japanese).
- **M3U import and export** for one playlist at a time, matching songs by file name and folder or by title and artist.

## Song details and covers

- **Edit** title, artist, album, album artist, genre, composer, year, track and disc number, and the cover. Your edits are kept in the app and always win; **your music files are never changed.**
- **Paste details:** paste text copied from anywhere (lines like "Title: ...", a list, a table or JSON) and the editor fills the fields it understands.
- **Genre** is read from the file (old numeric genres and several genres in one tag are understood), can be edited, and can be used in smart playlists.
- **Covers** from the tags are shown everywhere (lists, artists, albums, notification). Choose a picture of your own for a song, or take the cover from an online match.
- **Copy these details to other songs** (for example the album of one song to the rest of the album).

## Online lookup (optional)

Nothing here runs by itself: every request is one you pressed.

- **Search a song online** (MusicBrainz and the Cover Art Archive): the best match is ranked by title, artist and the song's own length (so the studio recording comes before concert versions), artists credited in another script are found, and you choose which details and which cover to take. Nothing is applied without your tick; details that would replace something real are not ticked and ask you first.
- **Batch lookup** for up to 100 songs at once, one search at a time and at the pace the service allows. Every result is saved per song, so a stop, a lost connection or a closed app loses nothing: Resume, Retry failed, and "Select next 100". A pause the service asks for is waited out. You review the matches and apply the ones you tick. **It keeps going while the phone is locked,** with a notification that shows the progress and a Stop button.
- Library Health can hand the songs it found (for example "missing details") straight to the lookup.
- **Other sources you switch on yourself** (Settings > Online sources): Wikidata, Last.fm, Discogs and TheAudioDB add genres, a year or an artist's name in its own script to a match. Last.fm and Discogs need your own free key, which stays on your phone and is not part of backups.

## Keeping the library tidy

- **Library Health** (Misc): possible duplicates (with their formats and bit rates, so you can see which copy is better), songs with missing details, songs with no cover, songs that could not be read, missing files and hidden songs. Hide or delete from there; nothing is ticked or removed for you.
- **Same artist or album?** (Misc): finds artists and albums written in more than one way ("Linkin Park" and "Linkin-Park", an album in two folders) and shows them together in Browse. Nothing is changed in your songs, you confirm every group, you can say "not the same", pick groups by hand, ungroup and undo.

## Statistics

- **Misc > Statistics** for all time, this year or the last 30 days: listening time, plays, songs played, most played, recently played, never played, forgotten favorites, often cut short, top artists.
- A page for each song: counts, listening time, average share heard, first and last played, rank, and plays per month for the last year.
- A play counts after about 30 seconds of real listening (or half of a short song); seeking forward cannot count as a play.

## Looks

- **Skins:** Material (default), **Cyberpunk** (a yellow HUD look with a dial that shows the song's progress) and **Frutiger Aero** (glass panes, a glossy play button with a progress ring, glass icon tiles).
- **Material look:** system, light or dark, an accent colour (swatches or your own), how strong the colours are (soft, vibrant, expressive, mono), pure black for OLED screens, and ready-made looks (True black, Ocean, Forest, Sunset, Rose, Violet, Neon, Graphite).
- Reorder the bottom tabs and the Now Playing buttons.
- Large system fonts are supported.

## Backup and restore

**Settings > Backup & Restore** saves one file, wherever you choose, with the parts you tick:

- settings (looks, equalizer, shuffle and its presets, playback options, tab order),
- playlists, smart playlists, favorites and hidden songs,
- play history and counts,
- your metadata edits and lookup results (optionally with the cover pictures),
- loudness measurements,
- your same-artist and same-album groups.

It holds no music. Songs are recognised again on another phone, or after a reinstall, by their audio, file name or title and artist; load it after the first scan has finished. Nothing is wiped when you load a profile: it is added to what is there. A big file (hundreds of megabytes with covers) loads without trouble.

Before an update changes how the app stores its data, the app also copies its own database on the phone, and Backup & Restore offers to put that copy back if the update broke something. It stays on the phone, so save a profile somewhere else too.

**Not included:** your music files and the details inside them, the music folders you chose, the play queue, and your online-source keys.

## Privacy

- No account, no cloud, no analytics, no ads, no background network use. The app does not check for updates, look anything up or send anything on its own.
- The internet permission is used only when you press something: a lookup (sends the title, artist and album of the song you look up), "Ask other sources" or Test on a source you turned on (sends the artist and title and, for Last.fm and Discogs, your own key), or Check for updates (asks GitHub for the newest release; nothing about you).
- Other permissions: music files (to play them), notifications and a foreground service (the playback notification, and a running batch lookup), and "modify system settings" (only for Set as ringtone).
- Your music files are only read. Everything the app adds (edits, lookups, covers, playlists, counts) is in the app's own storage, which Android removes when you uninstall.

## Known issues

- Cover art on a car's display over Bluetooth depends on the phone's Bluetooth stack; on at least one recent Samsung update it does not show for any player, not only this one. A recorder under Settings > Diagnostics > Media session log shows what the app hands to Android.
- This is a test version: expect rough edges.

## Problems and ideas

Open an issue on this page (the Issues tab) with what you did, what you expected and what happened, your phone model and the version under Settings > App updates. Song titles are not needed.
