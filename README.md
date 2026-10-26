# Local AI

**A private AI assistant that runs on your own Windows PC.** Your chats, memories and files stay on your computer.
It only goes online when it needs to: to look something up for you, to download the AI model you choose, or to use a
cloud AI you linked yourself.

- 💬 Chat, write, translate, explain, summarize: answered by an AI model running on your PC, in short, plain answers
- 🌦️ Live weather, sports scores, news and web answers with sources; it searches by itself when a question needs today's facts
- 🧮 Sums, tips, unit conversions, dates and "days until" worked out exactly, not guessed
- 📄 Ask about your documents (PDF, Word, text, even scans) and search your own files; it changes a file only after you click **Save**
- 🧠 Remembers what you tell it (your name, family, allergies…), and you can see and edit everything it remembers
- ⏰ Reminders, timers, repeating reminders and daily briefings, said in your own words
- 📅 A calendar for appointments, birthdays, bills and plans, with Google, Outlook and Apple calendars connected
- 🗣️ Talk to it and hear answers read aloud, even hands-free (optional voice add-on, runs on your PC)
- 🎮 **Workshop**: describe a game or an app and Local AI builds it, play-tests it and lets you use it right away
- 🖱️ **Do it for me**: it can use apps like Notepad, Calculator and File Explorer for you, with your OK
- 🎮 **Game mode**: when you start a game, the AI steps aside so your game gets the whole graphics card
- 🔌 **Connections**: link folders and services (GitHub, Home Assistant and more) and ask about them in normal words
- 🖼️ Create and edit pictures on your PC (optional add-on)
- 📱 Use it from your phone at home or anywhere, and give family members their own private sign-in
- ☁️ Optional: link your own Claude, ChatGPT or Gemini account for chats where you want it

> Local AI is a preview. Answers can be wrong: check anything important.

<p align="center">
  <img src="docs/images/1-start.png" alt="Local AI start screen with shortcut cards" width="49%">
  <img src="docs/images/2-chat-cards.png" alt="A chat with a weather forecast card and a sports scoreboard card" width="49%">
</p>
<p align="center">
  <img src="docs/images/3-phone.png" alt="Local AI on a phone, with a weather card and a reminder" width="38%">
  <img src="docs/images/4-family.png" alt="Family settings with private sign-ins, kids mode and quiet hours" width="49%">
</p>

---

## Download and install

1. Download **`LocalAI-Setup-<version>.exe`** from the [latest release](https://github.com/localai-app/local-ai/releases/latest).
2. Run it. Installing doesn't need administrator rights.
3. Follow the setup screens. Local AI checks your PC, recommends an AI model that fits, and downloads it for you.
   Every download is checked against a fixed checksum. Setup can also take your city and favourite teams and set up a
   morning briefing, so it's useful from day one.

The installer isn't code-signed yet, so Windows may say **"Windows protected your PC"**. Choose **More info**, then
**Run anyway**. Each release lists the installer's SHA-256 checksum, so you can verify the file first.

**Updates:** when a new version is out, choose **Update now**. Local AI downloads it, checks it against the published
fingerprint, updates itself and reopens. Your chats, memories and settings are kept.

## What you need

| | Minimum | Recommended |
|---|---|---|
| Windows | Windows 10 or 11, 64-bit | Windows 11 |
| Memory | 8 GB | 16 GB or more |
| Graphics | Not required (runs on the processor, slowly) | A graphics card with 8 GB or more |
| Disk space | About 4 GB | 10–25 GB, depending on the model and add-ons |

Local AI uses Vulkan, so it works with AMD, NVIDIA and Intel graphics.

**More than one graphics card?** The AI spreads across all of them. **Gaming laptop?** It uses the separate graphics
card and skips the slower built-in graphics. **AMD Strix Halo (Ryzen AI Max)?** It uses the large shared memory, so
bigger models fit. You can choose which card to use in **Settings → Speed & answers**.

After the AI loads, Local AI checks that it really fits on the graphics card. If part of it spilled into slower shared
memory, it moves picture reading (and, for some models, a few layers) to the processor and quietly reloads. It checks again every 15 minutes in case
something pushes it out later.

**Tune it for your PC**: **Settings → Speed & answers → Show fine-tune options** lets you choose how long the AI stays
loaded (up to always), see and adjust the graphics card fit, set processor threads, pick an answer style (Precise,
Balanced or Creative) and run a speed test. Chats can be as long as your model supports (up to 128k tokens).

### AI models offered during setup

Setup recommends one for your PC. You can switch later, or use your own `.gguf` file.

| Model | Download | Good for |
|---|---|---|
| Qwen3.5 4B (light) | about 3.4 GB | Smaller graphics cards, built-in graphics, or the processor |
| Qwen3.5 9B (balanced) | about 6.6 GB | Graphics cards with 8–12 GB |
| Qwen3.5 9B (great quality) | about 8.4 GB | Graphics cards with 12 GB or more |
| Gemma 4 26B (best quality) | about 15.4 GB | 16 GB graphics cards or more: smartest at this size, and quick |
| Qwen3.5 27B (large) | about 17.7 GB | 24 GB graphics cards |
| Qwen3.5 35B-A3B (large, fast) | about 22.9 GB | Two graphics cards, or AMD Strix Halo |

Qwen models are Apache-2.0; Gemma models carry Google's Gemma licence. Sizes include the file that lets the AI look at pictures.

---

## What it can do

### Chat and everyday help
- Answers Local AI works out itself show as tidy cards: sums and conversions, weather, sports, Steam prices,
  playtime, your PC's performance, your reminders and schedule, what it knows about you, stocks, crypto and news.
  Your phone shows the same cards. The ⓘ under any answer says in plain words what it used: saved memories, earlier
  chats and web sources.
- Ask anything: explanations, writing and email drafts, translations, ideas. Answers are as short as the question:
  a fact in a sentence or two, steps as a short list.
- Say things your own way, typos and all: "don't let me forget to call Mum at 5", "it's too bright in here",
  "make the text bigger", "google it". If it gets one wrong, reply "no, I meant …" and it learns your wording.
- **Talk to it like a person.** Follow-ups just work: "shorter", "and tomorrow?", "in feet?", "the second one",
  "that's old", "are you sure?", even "?". Tell it how you like replies ("keep your answers short", "be more
  sarcastic", "stop using emojis") and it keeps doing that in every chat. It gives a real pick when you ask for
  one, re-checks before agreeing when you say it's wrong, and never claims it can't do something it can.
- **The same for everyone**: family sign-ins and Discord guests get the same understanding and voice (within their own
- **Small things that add up**: Undo after forgetting a memory, the monthly "Still true?" check on phones, Every day / Weekdays buttons on reminders, and Sources that also show the pages Local AI skipped and why.
- **Better sources, and phones catch up**: questions about who runs or owns something are checked against Wikipedia or a news site; phones get repeat buttons on reminders, family members get repeating reminders, Undo and Sources; Discord guests get clearer answers and fewer repeated quotes.
- **Smarter answers, taught by example**: live prices for gold, oil, currencies and crypto, exact world times and bill splits, more questions looked up instead of guessed, weather questions in everyday words, and plainer web answers.
- **More answers you can count on**: exact holiday dates, fractions and number patterns, live prices for any company's stock, better web lookups on big pages, and requests that always get a real answer.
- **Straight answers about the world and about Local AI**: current officeholders looked up, live sports results, official Chrome and Firefox versions, and plain answers to "is my data safe?" and "what can you do offline?".
- **Better at knowing when to look things up**: local events this weekend, current officials and company leaders, betting favorites, tomorrow-morning forecasts, the newest Chrome and Edge versions, and real answers to everyday advice questions.
- **Understands more ways of asking**: when a question needs up-to-date facts in words it doesn't recognize, it checks and looks it up; casual web questions are searched in plain words; plus everyday wordings for prices, markets, weather, time zones, places and bill splits.
- **Morning brief**: the first time you open Local AI each day, one card (and a phone notification) with your weather, reminders and birthdays, yesterday's games, your watchlist, your teams, headlines, game deals and anything on your PC that needs attention. Family members get their own.
- **Brief cards and teams**: the brief is a clean stack of cards, one per section, and you manage the teams it follows in a list that checks each team when you add it (college teams too).
- **Your assistant**: 👎 under a wrong answer and Local AI tries again (also on phones and in Discord), follow topics for news in your morning brief, one-tap shortcuts for questions you ask often, and overnight prep that tidies up while your PC is idle.
- **Calendar**: a Calendar button on the left bar. Say "dentist next Tuesday at 3" or "Mom's birthday is March 3", ask "what's on my calendar this week?" or "am I free Friday?", and upcoming events show in your morning brief (birthdays a week ahead, the rest three days ahead, and on the day) with a notification 30 minutes before. Warns about overlaps, connects Google, Outlook or Apple calendars read-only, exports .ics, and has a shared family calendar on everyone's phone. Each event has **Add to my calendar** for your phone's own calendar or Outlook.
- **Phone menu and staying signed in**: one-tap tiles for Today, Calendar, Memories, Workshop and Settings in the phone's left menu, icons on every section, and a fix for iPhones signing you out of the Home Screen app.
- **Phone calendar, charts and chat settings**: the phone's Calendar shows the whole month (tap a day for its events), Today shows your watchlist with 30-day charts like the PC, and **This chat** explains each setting for the chat you have open.
- **Phone, markets and clips**: phone menu sections as clean cards with Snooze and Cancel on reminders, sector alerts, a market close summary and watchlist export, "clip that" by voice and sharing clips to Discord, plus better answers about frost, snow, other cities' weekend weather, spot prices, world news and local events.
- **Better answers, add to calendar, accessibility, smaller install**: the latest iOS, Android, macOS and Windows 11 versions straight from Apple, Google and Microsoft; "who runs <company>?" from the encyclopedia with the real title; "Add to my calendar" on each event (your phone's own calendar, or a file for Outlook/Windows/Apple on the PC); every control named for screen readers; and a smaller installer (about 120 MB) now that Local AI no longer carries a second copy of .NET.
- **Places near you**: "nearest gas station", "what's to eat around here?", "how long to get home?", "will I make my 3:00?", "where am I?". Cards with logos or photos, open now, distance and drive time, Directions and Website; follow-ups like "more", "open late" and "directions to the second one". Uses your phone's location (it asks first) or Windows' location on the PC; free maps, no account needed.
- **Folders, shows and file names**: just ask "organize the TV shows in D:\Downloads" or "clean up the file names in D:\Docs". Tidy cards with tap questions, a live example, show posters, before → after and Undo (or Finish it, if the PC closed mid-tidy); keep a folder tidy automatically, "what episodes am I missing?", "free up space" (to the Recycle Bin, after you check), photos by date, music by artist and album, and matching file names (dots, underscores and odd symbols gone, numbered files lined up).
- **Job finder**: a Jobs button on the left bar (and in the phone menu). Add the roles you want, a pay range, remote or a city and the sites to check; get one list with pay, a match score, scam warnings, drive time and a note on old listings. Tailor your resume and cover letter to any job (it never invents anything), see what changed, save as Word or PDF, get interview prep with a practice interview in chat, a company snapshot, follow-up drafts, a resume check and the skills these jobs ask for. Track applications, save searches for morning alerts, interviews go on your calendar. It never applies for you.
  limits). Long chats keep a short summary of their start, so a 60-message chat still knows what you decided early on.
  Once a month a "Still true?" card offers memories over a month old to keep or forget; "review my memories" does the
  same in chat. Ask "how do you search?" and it tells you plainly.
- **Sums done exactly**: percentages, tips, discounts and tax, splitting a bill, unit conversions (miles, kg, cups,
  ounces…), temperatures, "how many days until Christmas", and the date and time, all worked out by the app.
- Attach a picture (**+**, paste or drag in) and ask about it. **Ctrl+Alt+S** takes a picture of the window you're
  looking at so you can ask "what does this error mean?". **Ctrl+Alt+A** opens Local AI from anywhere.
- **Helpers** for a chat: Homework helper (hints, not answers), Recipe chef, Tech support, Writing coach, or your own.
- **Try again** and **Edit** work on a copy, so the original chat is kept. Pin chats, put them in projects, search all
  your chats, and export a chat as a file.
- Light or dark theme, or **Match Windows**, with a choice of accent colour and text size.

### Live answers from the web
- **It knows when to look things up.** Anything recent or upcoming (release dates, "the latest", results, who holds a job
  now, prices, store hours, outages, news) goes to the web instead of the AI's older built-in knowledge. If an answer
  gives away that it's out of date, Local AI searches instead, and "that's old" makes it search again.
- **Follow-ups keep the subject**: "when is the next Bengals game?" then "what channel is it on?".
- **Weather**: forecast cards with a week-by-day strip, for the city you saved or any city you name.
- **Sports**: scoreboard cards with the next game, time and TV channel.
- **Near me**: "where's the nearest …" uses your home location.
- **Links**: paste a link and say "summarize this page".
- Answers show their sources by site name. If it can't verify something, it says so instead of guessing.

### Your documents and files
- Drop a PDF, Word or text file on the message box and ask about it ("summarize this", "what does it say about
  refunds?"). Scanned documents and photos of paperwork are read too. Everything is read on your PC.
- Find, read and search files in the folders you allow.
- Ask it to create or change a text file: it shows you the exact text first and saves only when you click **Save**.
  The original is backed up.
- **Folder jobs**: "sort the files in my downloads folder" or "tidy up my pictures", tap **Tidy a folder** on the
  start screen, or drag a folder onto the chat. You see every step first (before → after grouped by show, with the
  changed part highlighted, and how the folders will look), and **Undo** puts it all back. Nothing is ever deleted or
  overwritten. If Local AI closes in the middle, the card offers **Finish it** or **Undo**.
- **TV shows and movies**: "organize the TV shows in D:\Downloads\TV" names them the way Emby, Plex and Jellyfin expect
  (Show\Season 01\Show - S01E01.mkv, subtitles alongside). It checks the folder first, asks a few tap questions (where
  the library goes, which copy to keep: the better picture wins), shows each show with its poster and missing episodes
  (optional TVmaze lookups), and can refresh your media server. Daily shows and anime numbering are understood, and
  episodes numbered only by their folder ("Season 1 Episode (8)\Jaynestown.mp4") are filed too, checked against the
  episode titles. You choose whether to move the files (nothing left behind) or copy them and keep the originals.
  Download-site names ("www.site.org - ") are dropped, the same show in differently named folders ends up in one
  folder with a folder per season, and old download folders left with only .nfo, .txt or .url files are cleared too.
- **Keep it tidy**: after a tidy, choose "Keep it tidy" (or ask "keep my downloads tidy"): new files get a card to check,
  or are filed without asking if you prefer.
- **Clean up file names**: "clean up the file names in D:\Docs" gives tidy, matching names without moving anything:
  dots, underscores, odd symbols and download tags go, and numbered files match (Chapter 1, chapter_02 → Chapter 01,
  Chapter 02). "Fix the episode names so all seasons match" renames shows to Show - S01E01, with episode titles if you
  like. Folders with programs or code are never touched.
- **Photos and music**: "organize my photos by date" (Year\Month folders by the date taken, exact copies set aside) and
  "sort my music" (Artist\Album - Title from the songs' details).
- **Free up space**: "what's taking up space?" shows your drives, the biggest folders and things that are usually safe
  to clear (old installers, zips you've unpacked, big files you haven't opened in months). Tick, confirm, and they go to
  the Recycle Bin.
- Folders with passwords, keys and browser data are always off-limits, and you can block any folder.

### Memory
- Tell it things like "Remember that my dog is called Biscuit" or "I'm allergic to peanuts". Ask "am I allergic to
  anything?" or "what's my wife's name?" and it answers from what you told it, never by guessing.
- Saved facts are used when they matter. For example, food suggestions leave out what you're allergic to.
- Open **Memories** to see, edit or delete everything it remembers, and **Undo** any new memory with one click.
- Optional "search model" (0.6 GB) finds memories and earlier chats by meaning, not just exact words, and helps it
  understand everyday wording.
- "What did we talk about yesterday?" looks back through your chats, and "did we ever discuss car engines?" finds the
  chats about a subject. You can turn memory off for a single chat.

### Reminders, timers and briefings
- Say it naturally: "remind me at quarter to 5 to leave", "the day after tomorrow", "on the 25th", "end of the month",
  "10 minute timer", "wake me up at 7".
- Change one just as easily: "snooze it", "make it 6 instead", "an hour earlier", "move it to Monday".
- **Repeating reminders**: "remind me every day at 9 to take my pills".
- **Briefings**: "every morning at 7, give me the weather and my team's next game" runs on schedule in its own chat,
  with a notification.
- **Watches**: "let me know when the new schedule is announced" checks every few hours and only speaks up when something
  changes.
- Windows notifications with **Snooze** buttons, and phone notifications too. Local AI needs to be running for them to
  go off.

### Job finder
- **Jobs** on the left bar: add one or more roles (it suggests similar titles), a pay range per year or hour, remote,
  hybrid or on-site with a city and distance, how recent, job type, level and words to leave out, then tick the sites.
  Remotive, RemoteOK, We Work Remotely, Jobicy, Arbeitnow and the companies you name are read directly; Indeed,
  LinkedIn, Glassdoor, ZipRecruiter, Monster, Dice and USAJobs get their own searches with your filters filled in.
- One list: a job found on several sites shows once with every link, its pay (marked when it's above or below the usual
  for your search), a match score with reasons, the drive time from your town, a scam warning when something looks off,
  and a note when a listing has been up for weeks.
- Add your resume (PDF, Word or text, from the PC or your phone; it stays on your PC). It gets a screening-software
  check and a chart of the skills your searches ask for. **Tailor my resume** reads the posting, looks the company up,
  then rewrites your resume and a cover letter using only what's in it: see exactly what changed, edit it, change the
  letter's tone, save as Word or PDF.
- **Interview prep** (likely questions, answers from your real experience, questions to ask, and **Practice in chat**),
  **About the company** (what it does, size, news, anything worth knowing), and follow-up, thank-you and recruiter
  drafts you copy and send yourself.
- Track applications (follow-up reminders), add an interview time to put it on your calendar, and save a search to hear
  about new jobs each morning (PC, phone, Discord). The morning brief gets a Job search line.
- In chat: "find remote data analyst jobs over 70k", "how are my applications going?". Family members get their own
  Jobs page on their phones; Discord guests can ask for the top five jobs. Local AI never applies for you.

### Places near you
- Ask about what's around you: "nearest grocery", "what's to eat around here?", "any pharmacies open now near me",
  "tacos near downtown Louisville". Each answer is a card: the place's logo or photo, open now or closed, distance and
  drive time, address, and Directions, Website and Call buttons. Then "more", "which ones are open late?",
  "directions to the second one" or "just Mexican".
- Malls and stores too: "what malls are near me?", "dollar stores nearby", "what stores are near me, like Walmart?"
  (the store you name comes first).
- "How long to get home?", "how far is the airport from here?" and "will I make my 3:00?" (for calendar events with a
  place: it says when to leave). "Where am I?" names the street and town.
- Away from home, "will it rain tomorrow?" and the morning brief use the town you're in.
- Your phone shares its location only for questions that need it (it asks you first); on the PC Local AI asks Windows
  (**Settings → Places & maps**, where you can add your home address for exact travel times). Positions are rounded to
  about a city block and never saved. Free services only: OpenStreetMap, Wikimedia and OSRM.

### Stocks and crypto
- "watch bitcoin and NVDA", "tell me if ETH drops below 2,000", "tell me if Tesla stock moves 5%", "how's my watchlist?",
  "what's trending in crypto?". Prices only; nothing about what you own.
- Big moves, your own price targets and new 30-day highs or lows become a notification on your PC and phone, a line in
  the Markets chat and, if you connect one, a post in your Discord channel. Alerts wait while you're gaming or overnight.
- Ask in your own words: "how are my stocks looking?", "market update", "stock news", "NVDA news" (headlines with links).
  Answers show as a card with each price, today's move and a 30-day chart.
- **More → Markets** opens your watchlist page: a card for every coin and stock with today's move, a 30-day chart, its
  alerts and a Remove button, plus Add and Refresh, Export (a CSV for Excel or Google Sheets) and a switch for a market
  close summary. "Every morning at 7, my markets summary" works too.
- Whole sectors and indexes: "watch the tech sector", "tell me if the energy sector drops 3%", "alert me if the S&P
  falls 2%". "Send me a daily market wrap" turns on a short summary after the US close on weekdays (the S&P 500,
  Nasdaq and Dow, plus your best and worst); "export my watchlist" saves it as a spreadsheet.
- **Settings → Markets** holds the watchlist, how sensitive alerts are, Discord alerts and an optional free Finnhub key.
- Only the names or tickers are sent to CoinGecko and Yahoo Finance. Local AI never suggests buying or selling and can't
  trade.

### Talk to it (optional voice add-on)
- **Ctrl+Alt+V** from any app starts hands-free talking.
- Speak your question with the microphone and hear answers read aloud with a natural voice that runs on your PC.
- **Talk hands-free**: just speak, pause, and Local AI answers out loud, then listens again.

### Workshop: make games and apps
- Describe a game or a handy app in your own words. Local AI plans it, builds it, play-tests it, and you can use it
  right away, on your PC or your phone.
- Ask for changes, use **Point and change** to pick the exact part of an app, **Undo** any change, and **Share** it as
  one file anyone can open.
- Web games and apps by default, and 2D or 3D games with a real game engine when you want one.
- Choose Quick, Best quality (an optional bigger builder download) or Claude, if you link it.

### Game mode
- When you start a game from Steam, Epic, EA, Riot, GOG, Ubisoft, Battle.net or Xbox (or any program you add to
  `games.txt`), Local AI steps aside: the AI model is unloaded so your game gets the whole graphics card, and background
  work waits.
- Reminders, sums, dates and your phone keep working. Ask something on the PC and the AI wakes up for the answer, then
  steps aside again a few minutes later. Family phones and Discord guests are asked to try again after the game.
- When the game closes, the AI is ready again within about half a minute. Turn it on or off in **Settings → Gaming**.
- **Playtime**: ask "how long have I played today?", "this week?" or "how long have I played Elden Ring?". An optional
  break reminder nudges you every 2 hours of play (**Settings → Gaming**).
- **Performance helper**: "why is my game stuttering?" or "what's using my RAM?" takes a quick reading of the processor,
  memory and graphics card, then gives plain advice.
- **Steam prices**: "is Hades on sale?" gets the price, any discount and a link, and you can watch a game for a sale.
  Only the game's name is sent to Steam. Discord guests and family phones can ask too.
- **Game clips** (optional, early): after a one-time add-on download, **Ctrl+Alt+C** or "clip that" saves the last
  15 seconds to 2 minutes of your game, with sound, to `Videos\Local AI Clips`. It uses your graphics card's video
  encoder only (tested once in **Settings → Gaming**), never the processor. Optionally say "clip that" out loud while
  you play (Windows' own offline speech recognizer, listening for a few phrases only while a game runs), and share a
  clip to your Discord channel with **Share to Discord** on the notification or "share that clip" (clips over 10 MB
  are copied at 720p first).

### Do it for me (computer use)
- "Open Notepad and write a shopping list", "in Calculator, work out 15% of 240", "in File Explorer, make a folder
  called Taxes".
- You approve the task once; risky steps (deleting, closing without saving) ask every time. An orange border shows where
  Local AI is working, and pressing **Esc** stops it at once. Before saying it's done, it checks the result is really there.
- Works best in Notepad, Calculator and File Explorer; other apps may work but are less tested.

### Connections
- Link Local AI to folders and services from **Settings → Files & web → Connections** (or just say "add a connection"):
  files in a folder, GitHub, Home Assistant, a ready-made setup written for Claude Desktop, or a web address. Services
  that sign in through the browser work too.
- Then ask in normal words, like "what's on the shopping list in My Files?". Anything that changes something shows a
  card with the exact action first: **Allow for this task**, **Always allow**, or **Don't**. Deleting, moving or paying
  asks every time.
- Access keys and sign-ins are stored encrypted, and anything a service sends back is treated as information, never as
  instructions.

### Pictures (optional add-on)
- "Draw me a red kite over a meadow" makes a picture on your PC in about half a minute on a good graphics card. You can
  then say "add a rainbow".
- The image add-on is a separate download (about 6.7 GB, plus 5.3 GB for editing).
- **Pictures** in the left bar shows everything you've made or added.
- With two graphics cards, pictures can be made on one while chat stays ready on the other.

### Phone, tablet and family
- **At home**: chat from your phone's browser on your home Wi-Fi. Scan a QR code, sign in, then use **Add to Home
  Screen**. It has the same look, cards and notifications as on the PC, plus a **Today** screen with your reminders,
  scheduled checks, watchlist and playtime. The left menu has one-tap tiles for Today, Calendar, Memories, Workshop and
  Settings, a month calendar, and the phone stays signed in even when an iPhone drops its saved sign-in.
- **From anywhere**: **Settings → Phone & sharing → Use from anywhere** lets your phone reach Local AI on any Wi-Fi or
  mobile data, with no router changes. Your phone signs in to Local AI with your own password, and repeated wrong
  passwords lock sign-in for longer and longer. Forgot the phone password? **Reset phone password** signs every phone out and lets you choose a new one.
- **Family**: in **Settings → Phone & sharing → Family**, give each person their own sign-in. They get private chats,
  memories, reminders and pictures. They can't see yours, your files, or each other's.
  - Kids mode gives age-appropriate answers and screens picture requests.
  - Per-person switches cover pictures, web and their own cloud AI account. You can also set quiet hours, pause someone
    instantly, or remove them.
  - Family sign-ins work only on your home Wi-Fi.
- Everyone shares the AI on your PC, which must be on with Local AI running. If two people ask at once, one waits a
  few seconds.

### Optional cloud AI
- Link your own **Claude**, **ChatGPT** or **Gemini** account with an API key, then pick it for a chat from the model
  button beside Send, or tap **Ask … too** under an answer for a second opinion.
- You're asked once before anything is sent. Only that chat's text is sent: never your files, web results or pictures,
  and memories only if you turn that on.
- Keys are encrypted on your PC. Cloud chats are billed by that company to your own account, and you can switch back
  at any time.

### Discord (optional)
- Connect your own Discord bot so people in your server can ask Local AI questions, with web answers, exact sums and
  today's date.
- Guests get a separate, limited assistant with no access to your chats, memories or files.
- Server commands: **/gamenight** (a reminder before it starts), **/lfg** (who's in? then a ping when it's time),
  **/patchnotes** (a weekly summary), **/plans**, **/price** and **/movers** (answered as cards with today's move in
  green or red and the 30-day range).

### Safety and housekeeping
- **Backups**: back up and restore everything in one file, optionally encrypted with a passphrase, or turn on daily
  automatic backups.
- **Updates**: Local AI checks this page once a day and offers **Update now**. Nothing installs without you, and
  **What's new** shows each release's notes afterwards.
- **Help**: the **?** in the left bar explains every feature and keyboard shortcut; each setting has a **What is this?**
  button and says whether it applies right away.
- **Your data folder** has a README.txt explaining what each file is.
- **System health**: a plain "at a glance" view of the model, graphics, phone access, backups and more.
- **Diagnostics**: Help → Save diagnostics makes a file for bug reports. It never includes your chats, memories or files.

### For tinkerers
Local AI starts in a simple mode. Turn on **Show all features** in **Settings → App** for:
- Teaching skills by example.
- Background research on topics you ask about, with a notebook of sources.
- Longer multi-step tasks over approved files.
- Coding help in an approved project folder (on a separate copy).

Answers to fix, topics you follow, shortcuts and overnight prep are under **Settings → Your assistant**. The older learning tools (idle practice, self-improvement) are under **Experimental features**, which is off unless you turn it on.

---

## Privacy

- **Stays on your PC:** your chats, memories, files, documents, pictures, reminders and settings. Chats and memories are
  stored encrypted for your Windows account. Voice, picture creation and the Workshop run on your PC too.
- **Goes online only when needed:**

  | When | Where |
  |---|---|
  | Downloading models or the add-ons you choose | Hugging Face |
  | Checking for and downloading updates | GitHub |
  | Looking things up | DuckDuckGo or Wikipedia (or Brave Search, if you add your own key), then the pages it reads |
  | Weather | Open-Meteo |
  | Sports | ESPN's public data |
  | Software versions | The projects' own release feeds |

- Only the search words and page addresses leave your PC. Your memories, files and chat history are never sent with them.
- **Only if you turn them on:** your own cloud AI account, Connections you add, your Discord bot, and phone, family or
  anywhere access.
- No accounts with us, no analytics, no ads.

## Known limitations

- Windows only. The installer isn't code-signed yet.
- Your PC must be on with Local AI running for phone, family, reminders and briefings to work.
- Speed depends on your graphics card. Without one, answers are slow.
- Do it for me is tested most in Notepad, Calculator and File Explorer.
- The AI can be wrong. Live answers show their sources, so you can check them.

## Licences

Local AI is built on open-source components, including:
- [llama.cpp](https://github.com/ggml-org/llama.cpp) and stable-diffusion.cpp (MIT)
- .NET (MIT)
- Markdig (BSD-2-Clause)
- PdfPig (Apache-2.0)
- SkiaSharp, Discord.Net and QRCoder (MIT)
- Microsoft Edge WebView2
- The Anthropic C# SDK (MIT)

Models are downloaded only when you choose them and carry their own licences (Qwen: Apache-2.0; Gemma: the Gemma
Terms of Use). Full notices are included with the program under **Help → Licences and credits**.
