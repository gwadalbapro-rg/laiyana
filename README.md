<p align="center">
  <img src="icon-256.png" width="128" alt="Laïyana logo: a baby with headphones">
</p>

<h1 align="center">laïyana</h1>

<p align="center">
  A bit-perfect music player for Windows, made for people who collect music.<br>
  Your library, handled a little more like records.
</p>

<p align="center">
  <a href="https://laiyana.app"><b>laiyana.app</b></a> · <a href="#download">Download</a> · <a href="https://github.com/gwadalbapro-rg/laiyana/issues">Report a bug</a>
</p>

<p align="center">
  <img src="docs/boucles/affiches/en-lecture.jpg" width="820" alt="Now Playing: the cover, the spinning record and synced lyrics">
</p>

## Why

I've been collecting music since middle school, and I've tried pretty much every player out there. Most of them felt incomplete, inconsistent, too expensive, or just not that nice to look at. I also collect vinyl, and I've always missed that feeling with digital files: pulling out a record, looking at the sleeve, reading the booklet.

So I built the player I wanted: the features I actually use, and an experience that feels a little more like handling records.

It's named after my little niece, Laïyana, who has been my biggest inspiration. That's why the logo is a baby with headphones.

## Features

### Sound

- **Bit-perfect playback** through WASAPI exclusive mode or ASIO. Nothing touches the signal unless you ask for it.
- **DSD** (DSF and DFF) over DoP, or converted to PCM when your DAC can't take it.
- **Signal path you can trust**: the player bar says *Bit-perfect* only when it's true. One click shows every step, from the file to your DAC, and tells you exactly what changed the signal, if anything (volume, resampling, ReplayGain).
- **Resampling only when needed**, if your device refuses a sample rate in exclusive mode, with high-quality linear-phase filtering and a single TPDF dither.
- **Formats**: FLAC, ALAC, WavPack, APE, WAV, AIFF, CAF, MP3, AAC, Vorbis, DSF, DFF.

### Your collection

- **Jump to a letter**: click a letter and your shelf jumps there. Every other album dims, and a glint sweeps across the first cover, like a light on the record bin.
- **Flow**: your whole collection as a full-screen wall of covers. Flip a cover to see its tracklist.
- **Sleeve**: open any cover full size, turn it over to see the back, and leaf through the booklet scans from the album folder.
- **Now Playing**: a big cover with a record that slides out and spins while it plays, synced lyrics, and a listening mode where everything else fades away.
- **Tidy**: rename and organize your files and folders from their tags, with a preview and undo.
- **Artist pages** with photo, biography and your listening history. Click the photo and their albums **bloom** around it, by year.
- **Hi-Res overview**: how much of your library goes beyond CD quality, and which albums.
- **Favorites** and **New arrivals**: your latest loves and additions, each with its own page.
- **Playlists** with their own handmade sleeve, cut from the covers of the albums inside.
- **Credits** from MusicBrainz (producers, featured artists, songwriters, samples), right next to the lyrics.
- **Synced lyrics for your whole collection**, fetched in the background, one track at a time.
- **Last.fm scrobbling**, if you connect your account: your plays from the last 14 days are sent too, and plays wait offline until the network is back.
- Tag editor, ReplayGain analysis, a smart shuffle that spreads artists and albums evenly, playlists (M3U8 import and export), a mini player, folder watching.

### Taking care of your library

- **Duplicates**: when an album is in your library twice, Laïyana shows it once, with the best version of each track. The extra copies are listed in one place: send all the MP3 copies of your FLACs to the Recycle Bin in one click, and look at the doubtful cases one by one.
- **Booklets**: scans found in the album folder (and its image subfolders) become a booklet you can leaf through; pick the back cover or add pages yourself.
- **Removed tracks**: everything you took out of the library, by album, to put back or send to the Recycle Bin.
- **Backup and restore**: plays, playlists and favorites in one small file, to move to a new PC.

### On Windows

- **Opens your files**: double-click a FLAC or MP3 in File Explorer and it plays, even if Laïyana is already open. Audio files get their own icon.
- **Media keys** and the Windows media overlay, playback buttons under the taskbar preview, an optional tray icon and start with Windows.
- English and French, following your Windows language.

## Screenshots

<p align="center">
  <img src="docs/boucles/affiches/sleeve-scene.jpg" width="400" alt="Sleeve: a cover full size">
  <img src="docs/boucles/affiches/chemin-du-signal-schema.jpg" width="400" alt="The signal path, from the file to the DAC: Bit-perfect">
</p>
<p align="center">
  <img src="docs/captures/qualite.jpg" width="810" alt="The quality check: an 88.2 kHz album whose music stops at 20.8 kHz, next to a genuine Hi-Res file">
</p>
<p align="center">
  <img src="docs/boucles/affiches/eclosion.jpg" width="400" alt="An artist's albums around their photo">
  <img src="docs/captures/doublons.jpg" width="400" alt="Duplicates: 330 albums of lossy copies to send to the Recycle Bin">
</p>

More, with short videos, on [laiyana.app](https://laiyana.app).

## Privacy

Everything stays on your computer. Laïyana has no account, no tracking and no analytics.

Online lookups are optional and can be turned off in Settings. When they're on, only artist names, album titles and track titles are sent, to free and open services:

- [MusicBrainz](https://musicbrainz.org), [Wikidata](https://www.wikidata.org), [Wikimedia Commons](https://commons.wikimedia.org) and [Cover Art Archive](https://coverartarchive.org) for credits, artist photos and missing covers
- [Wikipedia](https://www.wikipedia.org) for biographies
- [LRCLIB](https://lrclib.net) for synced lyrics, with [lyrics.ovh](https://lyrics.ovh) as a fallback
- [Last.fm](https://www.last.fm), only if you connect your account: artist, title, album, length and time of each play

Results are kept locally, so they work offline afterwards. Full details: [privacy](https://laiyana.app/privacy.html).

## Download
<a id="download"></a>

Windows 10 (1809 or later) or Windows 11, 64-bit.

- **Microsoft Store** (signed by Microsoft, automatic updates): link coming at release
- **Installer**: from the [Releases](https://github.com/gwadalbapro-rg/laiyana/releases) of this repository

Mac: not yet, a Mac version is being considered.

<!-- Until the installer is code-signed: -->
The installer isn't code-signed yet, so Windows SmartScreen may warn you the first time: click **More info**, then **Run anyway**.

## Feedback

Laïyana is free, with no account and no ads. The app is closed source; the audio output part may be released later as a free Rust library. If paid extras ever come (a *Pro* with headphone correction is planned), everything shown here stays free.

Bug reports, ideas and constructive criticism are very welcome: open an issue. If something sounds wrong, press **Ctrl + Shift + R** in the app: it copies a report (playback, output, errors) you can paste into the issue.

---

© 2026 Cédric Vilmen · [Legal notice](https://laiyana.app/legal.html) · [Privacy](https://laiyana.app/privacy.html)
