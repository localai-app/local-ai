# Local AI

**A private AI assistant that runs on your own Windows PC.** Your chats, memories and files stay on your computer.
It only goes online when it needs to: to look something up for you, to download the AI model you choose, or to use a
cloud AI you linked yourself.

- 💬 Chat, write, translate, explain, summarize: answered by an AI model running on your PC
- 🌦️ Live weather, sports scores and schedules, news and web answers with sources
- 📄 Read and search your own files; it creates or changes a file only after you click **Save**
- 🧠 Remembers what you tell it (your name, preferences, allergies…), and you can see and edit everything it remembers
- ⏰ Reminders, timers and alarms with Windows notifications
- 🖼️ Create and edit pictures on your PC (optional add-on)
- 📱 Use it from your phone or tablet on your home Wi-Fi, and give family members their own private sign-in
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
   Every download is checked against a fixed checksum.

The installer isn't code-signed yet, so Windows may say **"Windows protected your PC"**. Choose **More info**, then
**Run anyway**. Each release lists the installer's SHA-256 checksum, so you can verify the file first.

## What you need

| | Minimum | Recommended |
|---|---|---|
| Windows | Windows 10 or 11, 64-bit | Windows 11 |
| Memory | 8 GB | 16 GB or more |
| Graphics | Not required (runs on the processor, slowly) | A graphics card with 8 GB or more |
| Disk space | About 5 GB | 10–25 GB, depending on the model and add-ons |

Local AI uses Vulkan, so it works with AMD, NVIDIA and Intel graphics.

**More than one graphics card?** The AI spreads across all of them. **Gaming laptop?** It uses the separate graphics
card and skips the slower built-in graphics. **AMD Strix Halo (Ryzen AI Max)?** It uses the large shared memory, so
bigger models fit. You can choose which card to use in **Settings → Speed & answers**.

### AI models offered during setup

Setup recommends one for your PC. You can switch later, or use your own `.gguf` file.

| Model | Download | Good for |
|---|---|---|
| Qwen3.5 4B | about 3.4 GB | Smaller graphics cards, built-in graphics, or the processor |
| Qwen3.5 9B (balanced) | about 6.6 GB | Graphics cards with 8–12 GB |
| Qwen3.5 9B (best quality) | about 8.4 GB | Graphics cards with 12 GB or more |
| Qwen3.5 27B | about 17.7 GB | 24 GB graphics cards |
| Qwen3.5 35B-A3B | about 22.9 GB | Two graphics cards, or AMD Strix Halo |

The models come from Alibaba's Qwen family (Apache-2.0 licence). Sizes include the file that lets the AI look at pictures.

---

## What it can do

### Chat and everyday help
- Ask anything: explanations, writing and email drafts, translations, maths, conversions, ideas.
- Attach a picture (**+**, paste or drag in) and ask about it.
- **Try again** and **Edit** work on a copy, so the original chat is kept.
- Pin chats, put them in projects, search all your chats, and export a chat as a file.
- Light or dark theme, or **Match Windows**, with a choice of accent colour and text size.

### Live answers from the web
- **Weather**: "What's the weather tomorrow?" uses the city you saved in Settings, or name any city. You get a forecast
  card, with a day-by-day strip for the week.
- **Sports**: "When do the Louisville Cardinals play next?" or "Did the Steelers win?" gives a scoreboard card with the
  next game, time and TV channel.
- **Links**: paste a link and say "summarize this page".
- **Current facts and news**: Local AI searches, reads the pages and shows its sources. If it can't verify something, it
  says so instead of guessing.
- **Latest versions** of common software (Python, Node.js, Go, Rust, VS Code and more), taken from each project's
  official release feed.

### Your files
- Find, read and search files in the folders you allow; summarize a document or ask questions about it, including PDFs.
- Ask it to create or change a text file: it shows you the exact text first and saves only when you click **Save**.
  The original is backed up.
- Folders with passwords, keys and browser data are always off-limits, and you can block any folder.

### Memory
- Tell it things like "Remember that my dog is called Biscuit" or "I'm allergic to peanuts". It also picks up lasting
  facts from normal conversation.
- Saved facts are used when they matter. For example, food suggestions leave out what you're allergic to.
- Open **Memories** to see, edit or delete everything it remembers, and **Undo** any new memory with one click.
- Optional "search model" (0.6 GB) finds memories and earlier chats by meaning, not just exact words.
- You can turn memory off for a single chat.

### Reminders and timers
- "Remind me tomorrow at 9 to call the dentist", "Set a timer for 10 minutes", "What reminders do I have?".
- You get a Windows notification, a sound and a reminder card in the chat, with **Snooze**. Timers count down live.
- Local AI needs to be running for reminders to go off.

### Pictures (optional add-on)
- "Generate an image of a red kite over a meadow" makes a picture on your PC in about half a minute on a good graphics
  card. You can then say "Edit this image: add a rainbow".
- The image add-on is a separate download (about 6.7 GB, plus 5.3 GB for editing).
- **Pictures** in the left bar shows everything you've made or added.
- With two graphics cards, pictures can be made on one while chat stays ready on the other.

### Phone, tablet and family
- **Your phone**: chat from your phone's browser on your home Wi-Fi. Scan a QR code, sign in, then use **Add to Home
  Screen**. It has the same look and the same cards as on the PC.
- **Family**: in **Settings → Phone & sharing → Family**, give each person their own sign-in. They get private chats,
  memories, reminders and pictures. They can't see yours, your files, or each other's.
  - Kids mode gives age-appropriate answers and screens picture requests.
  - Per-person switches cover pictures, web and their own cloud AI account. You can also set quiet hours, pause someone
    instantly, or remove them.
  - Family sign-ins work only on your home Wi-Fi.
- Optional home certificate: install it once on a phone or tablet to stop the browser's "not private" warning.
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
- Connect your own Discord bot so people in your server can ask Local AI questions.
- Guests get a separate, limited assistant with no access to your chats, memories or files.

### Safety and housekeeping
- **Backups**: back up and restore everything in one file, optionally encrypted with a passphrase, or turn on daily
  automatic backups.
- **Updates**: Local AI checks this page once a day and shows **Update available**. Nothing installs without you.
- **System health**: a plain "at a glance" view of the model, graphics, phone access, backups and more.
- **Diagnostics**: Help → Save diagnostics makes a file for bug reports. It never includes your chats, memories or files.

### For tinkerers
Turn on **Show all features** in Settings for:
- Teaching skills by example.
- Background research on topics you ask about, with a notebook of sources.
- Longer multi-step tasks over approved files.
- Coding help in an approved project folder (on a separate copy).

Idle practice and self-improvement are under **Experimental features**, which is off unless you turn it on.

---

## Privacy

- **Stays on your PC:** your chats, memories, files, pictures, reminders and settings. Chats and memories are stored
  encrypted for your Windows account.
- **Goes online only when needed:**

  | When | Where |
  |---|---|
  | Downloading models or the image add-on you choose | Hugging Face |
  | Checking for updates | GitHub |
  | Looking things up | DuckDuckGo or Wikipedia (or Brave Search, if you add your own key), then the pages it reads |
  | Weather | Open-Meteo |
  | Sports | ESPN's public data |
  | Software versions | The projects' own release feeds |

- Only the search words and page addresses leave your PC. Your memories, files and chat history are never sent with them.
- **Only if you turn them on:** your own cloud AI account, your Discord bot, and phone or family access on your home
  network.
- No accounts with us, no analytics, no ads.

## Known limitations

- Windows only. The installer isn't code-signed yet.
- Your PC must be on with Local AI running for phone, family and reminders to work. Reminders appear on a phone only
  while the Local AI page is open.
- Speed depends on your graphics card. Without one, answers are slow.
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

Models are downloaded only when you choose them and carry their own licences (Qwen: Apache-2.0). Full notices are
included with the program under **Help → Licences and credits**.
