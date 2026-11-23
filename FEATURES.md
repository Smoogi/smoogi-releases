# Feature guide

Everything Smoogi's Music Player can do. Back to the [front page](README.md) for the download, installing and privacy.

**Contents:** [Playing music](#playing-music) · [Queue](#queue) · [Shuffle](#shuffle) · [Sound](#sound) · [Library and browsing](#library-and-browsing) · [Playlists](#playlists) · [Song details and covers](#song-details-and-covers) · [Lyrics](#lyrics) · [Online lookup](#online-lookup-optional) · [Keeping the library tidy](#keeping-the-library-tidy) · [Statistics](#statistics) · [Looks](#looks) · [Backup and restore](#backup-and-restore)

---

## Playing music

- **Background playback** with a media notification, lock-screen controls, headset and Bluetooth buttons, and the cover of the playing song on the notification and the lock screen.
- **Now Playing screen:** large cover, seek bar, previous / play-pause / next, and a second row with Shuffle, Options and Repeat. Pull the page down to close it. A long press on the cover opens the same menu as a long press on a song.
- **Customisable controls:** put the Shuffle, Options and Repeat buttons in the order you like and show or hide their names (Settings > Now Playing Controls).
- **Time left:** tap the time at the right of the seek bar to switch between the song's length and the time that is left.
- **Playback options** (the Options button): sleep timer (15, 30, 45 or 60 minutes, with a fade-out at the end), **stop after this song**, playback speed from 0.5x to 2.0x with the pitch kept, and **A-B repeat** to loop a part of a song.
- **Repeat** off, all or one. Playback resumes where you left it after the app is closed.
- **Skip silent intros and outros:** two switches (off by default). The app listens to each song once, in the background, and skips clear silence at the start or the end (never more than 10 seconds, never on short songs).
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
- **Songs, Browse (Artists, Albums, Genres, Years and Folders), Playlists, Misc, Settings:** five tabs you can put in your own order. Artists show a fan of their album covers.
- **Search** by song, artist, album and genre, fast also in big libraries and with Japanese and other scripts.
- **Favorites** and **Hidden songs** (hide a song from the library without deleting it; hidden songs keep their place in playlists and can be shown again).
- **When a file name has no "Artist - Title":** choose whether the folder name or "Unknown Artist" is used.
- **Song menu** (long press): play next, add to queue, add to playlist, favorite, edit details, hide, **details** (format, bit rate, size, folder, dates, counts), **share** the audio file, **set as ringtone**, and **delete from device** (with Android's own confirmation).
- Built and tested for libraries of a few thousand songs.

## Playlists

- Create, rename, delete and reorder playlists. Adding skips duplicates.
- **Add many songs at once:** the + on a playlist opens a picker with search, an **All** button that selects or clears everything listed, and a **Filter** by artist, album, genre or year. A new playlist opens straight away so you can fill it.
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

## Lyrics

- **Lyrics that follow the song:** on the player, swipe the cover sideways to see the lyrics; the line being sung is highlighted and kept in view, and it follows seeking, pausing and skipping. Two small marks under the cover show that there is a lyrics page. Songs without lyrics simply have no second page.
- **From a `.lrc` file next to the song** (same name, ending in `.lrc`, in a folder you added): found by itself, read only, and understood in the common encodings, including Shift-JIS and UTF-16.
- **Add lyrics** (the menu of a song, long-press): pick any `.lrc` or text file, whatever it is called or wherever it is. The app keeps its own copy for that song; your files are not changed. **Remove imported lyrics** is in the same menu.
- **Word by word:** if the file has word times (enhanced LRC), the line being sung lights up word by word; lines without word times use the normal highlight.
- **Full screen:** double tap the lyrics to read them large, a few lines at a time. Double tap again, Back or the close button leaves. One tap shows previous / play-pause / next, the title and the text size. The screen stays on only while it is open.

## Online lookup (optional)

Nothing here runs by itself: every request is one you pressed.

- **Search a song online** (MusicBrainz and the Cover Art Archive): the best match is ranked by title, artist and the song's own length (so the studio recording comes before concert versions), artists credited in another script are found, and you choose which details and which cover to take. Nothing is applied without your tick; details that would replace something real are not ticked and ask you first.
- **Batch lookup** for up to 100 songs at once, one search at a time and at the pace the service allows. Every result is saved per song, so a stop, a lost connection or a closed app loses nothing: Resume, Retry failed, and "Select next 100". A **Missing metadata** switch lists only songs that lack the details you choose (title, artist, album, genre, year, track and disc number, album artist, cover); songs that were already checked stay in the list, and **Recheck checked** selects them again on purpose. A pause the service asks for is waited out. You review the matches and apply the ones you tick. **It keeps going while the phone is locked,** with a notification that shows the progress and a Stop button.
- **Find lyrics online** (Misc, LRCLIB): off until you switch it on on that page. A press of Search sends the title, artist and the album you typed to lrclib.net; you read the answers, and only **Use these lyrics** keeps one for the playing song (and asks first if the song already has lyrics). Lyrics are often protected by copyright; use them for yourself.
- Library Health can hand the songs it found (for example "missing details") straight to the lookup.
- **Other sources you switch on yourself** (Settings > Online sources): Wikidata, Last.fm, Discogs and TheAudioDB add genres, a year or an artist's name in its own script to a match. Last.fm and Discogs need your own free key, which stays on your phone and is not part of backups.

## Keeping the library tidy

- **Library Health** (Misc): possible duplicates (with their formats and bit rates, so you can see which copy is better), songs with missing details, songs with no cover, songs that could not be read, missing files and hidden songs. Hide or delete from there; nothing is ticked or removed for you.
- **Same artist or album?** (Misc): finds artists and albums written in more than one way ("Linkin Park" and "Linkin-Park", an album in two folders) and shows them together in Browse. A grouped artist also counts as one in Statistics, in playlist rules and in the duplicate check. Nothing is changed in your songs, you confirm every group, you can say "not the same", pick groups by hand, ungroup and undo.

## Statistics

- **Misc > Statistics** for all time, this year or the last 30 days: listening time, plays, songs played, most played, recently played, never played, forgotten favorites, often cut short, top artists.
- **Library** (next to Listening): how your songs divide over genres, artists and albums, in a chart and a list. Tap a genre to see its artists, an artist to see its albums, an album to open its songs; a song with several genres is split between them.
- A page for each song: counts, listening time, average share heard, first and last played, rank, and plays per month for the last year.
- A play counts after about 30 seconds of real listening (or half of a short song); seeking forward cannot count as a play.

## Looks

- **Skins:** four looks to choose from in Settings > Appearance.
  - **Material** (default): the standard look, in your colours.
  - **Cyberpunk:** a yellow HUD on a night city, with a dial that shows the song's progress.
  - **Frutiger Aero:** glass panes, bubbles, a glossy play button with a progress ring.
  - **PC-94:** an old Japanese desktop: dot-matrix lettering, bevelled windows and keys on a night sky with cherry blossoms. The player's menu bar opens real screens. Options: Japanese labels for the tab names and menu, a fine dither texture on surfaces (Off, Subtle, Strong), and an artwork filter (Soft, PC-94, Extreme) that shows covers with few colours and dithered pixels. Your pictures are never changed.
- **Material look:** system, light or dark, an accent colour (swatches or your own), how strong the colours are (soft, vibrant, expressive, mono), pure black for OLED screens, and ready-made looks (True black, Ocean, Forest, Sunset, Rose, Violet, Neon, Graphite).
- **Your own wallpaper:** in Settings > Appearance, Cyberpunk, Frutiger Aero and PC-94 can show a picture of your own behind the skin instead of the one they come with. The picture is copied into the app; your original is not changed.
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

**Automatic backups:** choose a folder (your Google Drive folder, an SD card, any folder a sync app watches), how often (every day, 3 days, week or month) and how many to keep. When you open the app and a backup is due, it saves everything above into that folder, and removes the oldest ones it made. It only runs while the app is open, uses no internet, and **Back up now** does it on the spot. A backup with covers is saved in pieces, so it works however big it gets.

Before an update changes how the app stores its data, the app also copies its own database on the phone, and Backup & Restore offers to put that copy back if the update broke something. It stays on the phone, so save a profile somewhere else too.

**Not included:** your music files and the details inside them, the music folders you chose, the play queue, and your online-source keys.
