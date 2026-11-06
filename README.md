SONG PLAYER — SETUP GUIDE
=========================

What's in this folder
---------------------
- index.html, sw.js, manifest.webmanifest, icons  → the app itself. You won't need to touch these.
- playlist.txt  → the name at the top of the app, your folders, and the songs in each, in order.
- songs  → one folder per group of songs: Worship, Devotional and Other Songs. Each holds your
  MP3s, plus one lyrics file (.txt) for each song.


1. Add your songs (easiest on a computer)
-----------------------------------------
1. Copy your MP3s from Suno into the right folder: songs/Worship, songs/Devotional or
   songs/Other Songs. (You can add more folders later the same way.)
2. Each song needs a lyrics file with the SAME name, ending in .txt instead of .mp3:
       songs/Worship/Ordinary Ground.mp3
       songs/Worship/Ordinary Ground.txt
   Two lyrics files are already in the Worship folder to start from. Copy one for each new song.
3. Open each .txt file (Notepad is fine), and paste the lyrics from the song's page in Suno
   under the notes. Keep the Title: and Scripture: lines at the top.
4. Open playlist.txt. Change the Title, Subtitle and Artist lines if you like. Then, under each
   folder name in square brackets, list that folder's songs, one per line, in playing order:
       [Worship]
       Ordinary Ground
       Think on These Things

       [Devotional]
       (devotional song names here)

       [Other Songs]
       (other song names here)

Each folder shows as its own tab in the app, with its own Play all and Shuffle. A tab appears
once at least one song is listed under it, and the tabs follow the order in playlist.txt.
Empty folders don't upload to GitHub, so that's fine — they show up once they have songs.
Names must match exactly, including capital letters and spaces: [Worship] goes with the
songs/Worship folder, and "Ordinary Ground" with Ordinary Ground.mp3 and Ordinary Ground.txt.


2. Put it on GitHub
-------------------
1. Sign in at github.com. Click the + at the top right, then "New repository".
2. Name it something short, like  songs . Choose Public. Click "Create repository".
3. On the new page, click the link "uploading an existing file".
4. On your computer, open the song-player folder, select everything INSIDE it
   (not the folder itself), and drag it onto the GitHub page. The icons and songs folders come along.
5. Click "Commit changes" and wait for the upload to finish.
6. Click Settings (top of the repository) → Pages (left side).
   Under "Build and deployment": Source = Deploy from a branch, Branch = main, folder = / (root). Click Save.
7. Wait a minute or two and refresh. Your address appears at the top of that page, like:
       https://YOUR-GITHUB-NAME.github.io/songs/


3. Share it
-----------
Open your address on your phone and tap Share at the top. Send it by text or email.
The Share button shares the tab you're on, so the link opens straight to that folder
(for example, just your worship songs).
Friends and family just tap the link. To keep it on their home screen:
- Android: tap "Install app" in the app (or the browser menu → Add to Home screen).
- iPhone: tap the Share button in Safari → Add to Home Screen.
The Share button on the lyrics screen sends a link straight to that one song.


4. Your editor link (for timing the lyrics)
-------------------------------------------
Add ?edit to the end of your address and bookmark it for yourself:
       https://YOUR-GITHUB-NAME.github.io/songs/?edit

In the editor view:
- Under each song you'll see whether the audio and lyrics files were found, and what name
  the app is looking for if one is missing.
- Open a song and tap "Time the lyrics". Tap Start, and every time a new line begins, tap the
  big button. Missed one? Tap Undo and the song backs up a few seconds.
- When it's done, tap "Copy text". On GitHub, open the song's .txt file (the app shows its full path),
  tap the pencil (Edit), select all, paste over it, and tap "Commit changes".
- "Preview on this phone" lets you watch the result before you upload it.

Without timing, the lyrics still show and drift slowly up the screen as the song plays.
With timing, each line lights up as it's sung, and anyone can tap a line to jump to it.


Adding a song later (works from your phone too)
-----------------------------------------------
1. On GitHub, open the songs folder, then the right folder (like Worship) → Add file → Upload files
   → pick the MP3 and its .txt → Commit changes.
2. Open playlist.txt → pencil (Edit) → add the song name on its own line under its folder → Commit changes.

To start a new folder from the GitHub website, drag the folder from your computer into the songs
folder's upload page. (GitHub can't hold an empty folder, so it needs at least one file in it.)
The site updates within a few minutes.


Extras for a lyrics file
------------------------
These go at the top of a song's .txt file, each on its own line:
    Title: Ordinary Ground
    Scripture: Isaiah 40:28-31
    Note: A sentence or two about the song. It shows above the lyrics.
    Cover: Ordinary Ground.jpg      (song artwork saved in the songs folder; shows in the list and on the lock screen)

In the lyrics:
- [Verse 1], [Chorus], [Bridge] and similar tags show as small labels.
- A line in (parentheses) shows in italics — good for whispered or background parts.
- Lines starting with # are notes to yourself and never show.


Good to know
------------
- Free GitHub Pages sites are public. The link isn't listed anywhere, but anyone who has it can listen.
  Tabs keep your music organized, but anyone with any link can tap over to every tab. For songs
  meant only for certain people, make a second repository with its own link.
- GitHub's website accepts files up to 25 MB each. Suno MP3s are well under that.
- To change the name under the home-screen icon, edit "name" and "short_name" in manifest.webmanifest.
- Playback keeps going with the screen off. The song shows on the lock screen, and Bluetooth
  headphones and car stereos can play, pause and skip. While the lyrics screen is open and a
  song is playing, the phone's screen stays on.
