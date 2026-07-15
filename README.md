<div align="center">

<img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/banner.png" alt="ForwardX Banner" width="100%">

[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](#)
[![Made with Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](#)
[![Made with Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](#)
[![License](https://img.shields.io/badge/License-GPL-brightgreen?style=for-the-badge)](#)
[![Made with ❤️](https://img.shields.io/badge/Made%20with-❤️-white?style=for-the-badge)](#)
<br>

### Auto-forward your Telegram messages — 24/7, on autopilot.

**ForwardX** is an Android app that automatically **copies messages from one Telegram chat to another**, using your own account. Its Free, Automatic, Filterable and Always ON

</div>

<div align="center">

<a href="https://github.com/weebzone/ForwardX/releases/latest">
  <img src="https://raw.githubusercontent.com/weebzone/ForwardX/main/screenshots/downloadbanner.png" alt="Download ForwardX" width="200">
</a>

**Latest stable APK • Free • No Ads**

</div>



## 🧭 Quick Navigation

- 📲 [Install the app](#-1-install-which-apk-do-i-download)
- 🔑 [First-time setup](#-2-first-time-setup)
- 🧩 [The basics](#-3-the-basics)
- 🛠️ [Make your first rule](#-4-making-your-first-rule)
- 📋 [Every rule field explained](#-5-every-rule-field-explained)
- 🎬 [Content categories](#-6-auto-content-categories)
- ⏪ [Backfill old messages](#-7-backfill)
- ⚙️ [Settings explained](#-8-the-settings-page)
- 🔄 [Always-on: every situation](#-9-always-on-every-situation-explained)
- 🍱 [Ready-made recipes](#-10-ready-made-rule-recipes)
- 🆘 [Tips & troubleshooting](#-11-tips-safety--troubleshooting)

---

## 📸 Screenshots

<div align="center">

| Login | Home | PowerOn | Rules |
|:---:|:---:|:---:|:---:|
| <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/authscreen.jpg" width="150"> | <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/homescreen1.jpg" width="150"> | <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/homescreen2.jpg" width="150"> | <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/rulescreen.jpg" width="150"> |
| Rule editor | Logs | Settings | Stats |
| <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/rulesinscreen.jpg" width="150"> | <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/logscreen.jpg" width="150"> | <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/settingscreen.jpg" width="150"> | <img src="https://raw.githubusercontent.com/weebzone/ForwardX/refs/heads/main/screenshots/statscreen.jpg" width="150"> |

</div>

---

## 📲 1. Install: which APK do I download?

The app ships as a few different APK files — one per phone type. Pick **just one**:

| APK file | Pick this if… |
|---|---|
| `app-arm64-v8a-release.apk` | ✅ **You have a normal, modern phone (2017 or newer).** Best choice for 95% of people — smallest download. |
| `app-armeabi-v7a-release.apk` | You have an older / low-end 32-bit phone. |
| `app-x86_64-release.apk` | You're running an Android emulator on a PC. |
| `app-universal-release.apk` | Not sure which one you need? This works on **every** device (just a bit bigger). |

> 🤔 **Why so many files?** Each phone chip needs slightly different internal code. Shipping the exact one your phone needs keeps the download small. When in doubt, grab **`universal`** — it always works.

**To install:** download the APK → open it → allow *"Install from unknown sources"* if Android asks → tap **Install**. ✅

---

## 🔑 2. First-time setup

### Step 2.1 — Allow two quick permissions

- 🔔 **Notifications** — required so Android lets the background service keep running.
- 🔋 **Ignore battery optimization** — stops Android from killing the app to "save battery." This is essential for reliable, non-stop forwarding.

### Step 2.2 — Grab your Telegram API keys

ForwardX logs in as *you*, so Telegram needs your own personal API keys first.

1. On a browser, visit **[my.telegram.org](https://my.telegram.org)** and log in with your phone number.
2. Open **"API development tools."**
3. Fill in the short form (App title: `ForwardX`, short name: `forwardx`, platform: Android — anything works here).
4. You'll get an **`api_id`** (a number) and an **`api_hash`** (a long string of letters and numbers). Keep both handy.

### Step 2.3 — Open the app and sign in

1. Launch ForwardX → paste your **API ID** and **API Hash** → **Continue**.
2. Enter your **phone number** with country code (e.g. `+919876543210`) → **Send code**.
3. Telegram sends a login code to your Telegram app → type it in → **Verify**.
4. Have Two-Step Verification on? Enter your password → **Unlock**.

> 🔒 **Your privacy:** your credentials stay **only on your phone**. Nothing is ever uploaded anywhere.

---

## 🧩 3. The basics

Just three words to know:

- 📥 **Source** — the chat you copy messages **from** (a channel, group, or even a private chat).
- 📤 **Destination** — the chat you send messages **to**. One rule can send to **several** destinations at once.
- 📜 **Rule** — the recipe connecting them: *"from this source, forward messages matching these filters, to these destinations."*

**The main power switch:** on the **Home** screen there's a big toggle.
- **ON** → forwarding is live (a small notification shows the app is running).
- **OFF** → nothing gets forwarded.

> 💡 Tip: you can build rules while forwarding is off, then flip the switch on once you're ready.

---

## 🛠️ 4. Making your first rule

Let's forward everything from a channel called *"Movies HD"* into your own *"My Backup"* channel:

1. Go to the **Rules** tab → tap **➕**.
2. **Rule name:** give it something memorable, like `Movies backup`.
3. **From:** tap it, pick *Movies HD*.
4. **To:** tap it, pick *My Backup* (you can add more destinations here too).
5. Leave everything else as-is for now.
6. Tap **Save rule**.
7. Go to **Home** and flip the main toggle **ON**.

🎉 That's it! New posts in *Movies HD* now land in *My Backup* automatically.

> ⚠️ A rule only saves once it has a **name**, a **source**, and at least **one destination**.

Want to change it later? **Rules** tab → tap the rule. Want to try it safely first? Use the **Test 🧪** button on the rule — nothing gets sent.

---

## 📋 5. Every rule field explained

Fields are grouped into sections inside the rule editor. **You really only need the first three** (Name, From, To) — everything below is optional fine-tuning.

### 5.1 — Route (From / To)
- **From:** the source chat *(required)*.
- **To:** one or more destinations *(at least one required)*.

> 📝 **Example:** From = `Anime Uploads`, To = `My Anime` **and** `Backup Drive Channel` → every match goes to *both*.

### 5.2 — Priority & Exclusive stop
- **Priority** (`0`–`100`): when several rules watch the *same* source, higher numbers get checked **first**.
- **Exclusive stop**: if this rule matches, **stop** — don't let lower-priority rules also grab the message.

> 💡 A file can match multiple rules. Priority + Exclusive stop lets you send each message to exactly **one** place. See the [category routing example](#-65--routing-each-category-to-its-own-channel).

### 5.3 — Copy mode
- **Off** *(default)* — a normal Telegram **forward** (shows "Forwarded from…").
- **On** — re-sends as a fresh **copy**, no "Forwarded from" tag.

> ⚠️ Caption edits (Section 5.9) only work when Copy mode is **ON**, since cleaning a caption means re-sending the message.

### 5.4 — Message types (media filter)
Choose exactly what this rule should forward:
`ALL` · `TEXT ONLY` · `MEDIA ONLY` · `PHOTOS` · `VIDEOS` · `DOCUMENTS` · `AUDIO` · `VOICE`

> 📝 **Example:** set to **VIDEOS** to skip text chatter and photos, and forward only video posts.

### 5.5 — Content category (auto-detected)
Automatically detects each file's type and forwards only the categories you pick — full details in [Section 6](#-6-auto-content-categories). Leave everything off to allow any type.

- **Must match ALL selected:**
  - **ON** → the file must match *every* selected category (e.g. `Movie + Split` = only split movies).
  - **OFF** → the file can match *any one* of them (e.g. `Movie` **or** `Split`).

### 5.6 — Sender filter
Forward messages only from certain senders:
- **Any** *(default)*
- **Specific users** — only listed user IDs
- **Admins** — only chat admins
- **Anonymous admins** — messages posted "as the channel"
- **Verified** — only blue-tick verified accounts

> 📝 **Example:** in a busy group, set to **Admins** so only staff posts get forwarded.

### 5.7 — Keyword filters *(matched against caption/text)*
- **Only if contains** — forward *only* when the caption has one of these (comma = "any of").
  - 📝 `1080p, 2160p, 4k` → forwards posts mentioning any of those.
- **Skip if contains** — *block* the message if it contains any of these.
  - 📝 `sample, trailer, hdcam` → skips samples, trailers, hdcam.
- **Regex** toggle — treat the box as one regular expression (`|` for alternatives).
  - 📝 `S\d{2}E\d{2}` → only posts with an `S01E02`-style tag.
- **Case sensitive** / **Whole word only** — fine-tunes non-regex matching.

### 5.8 — File filters *(matched against the filename)*
- **Min MB / Max MB** — only forward files in a size range (e.g. Min `100` skips tiny junk/sample files).
- **Filename contains** (comma = any) — e.g. `1080p, x265`.
- **Ends with** (comma = any) — e.g. `.mkv, .mp4` → only those extensions.
- **Regex** (`|` = multiple) — e.g. `S\d{2}E\d{2}\.mkv$`.

> ℹ️ All filled-in file filters must pass **together** (AND). Empty ones are simply ignored.

### 5.9 — Caption edits *(needs Copy mode ON)*
Clean up messy captions before sending:

- ⭐ **Clean filename caption** — the smart one. Strips links, `@usernames`, `#hashtags`, emojis, and decorative symbols, then trims everything after the file extension (keeping a `.001` split suffix if present).
  - **Before:**
    ```
    🎬 Tuck Jagadish (2021) 1080p WEB-DL.mkv
    ━━━━━━━━━━━
    📥 via @SomeBot   🔗 https://t.me/somechannel
    #Bollywood #Movies
    ```
  - **After:** `Tuck Jagadish (2021) 1080p WEB-DL.mkv`
- **Remove links / @usernames / #hashtags / emojis** — individual strippers, if you don't want the full trim above.
- **Prepend / header** — text added at the top, e.g. `🎬 New upload:`.
- **Append / footer** — text added at the bottom, e.g. `Join @MyChannel`.
- **Find & replace** — custom text swaps, with optional regex / case-sensitivity per row.

### 5.10 — Schedule
Only forward within a chosen time window and set of days.
> 📝 **Example:** `22:00 → 06:00`, Mon–Fri → forwards only overnight on weekdays. (Overnight windows crossing midnight are supported.)

### 5.11 — Delivery & sync
- **Delay before forwarding** (`0`–`120s`) — wait before sending each match (adds to the global delay in Settings).
- **Max retries on failure** (`0`–`10`) — how many times to retry a failed send.
- **Sync edits** — if the original message is edited, update the forwarded copy too.
- **Sync deletes** — if the original is deleted, delete the forwarded copy too.

---

## 🎬 6. Auto content categories

ForwardX reads each file's **caption first, then its filename**, and auto-tags it — no manual keyword typing needed.

### 6.1 — Movie 🎬
A single film — detected by a release year or a standalone video/document with no episode markers.
```
Tuck Jagadish (2021) 1080p WEB-DL.mkv
Inception.2010.BluRay.x264.mkv
Interstellar 2014 2160p HDR.mkv
```

### 6.2 — TV Show 📺
Episodic content with an `S01E05`, `1x05`, or "Season + Episode" marker.
```
Loki S01E05 1080p.mkv
The Office 1x05.mkv
Breaking Bad Season 2 Episode 3.mkv
```

### 6.3 — Combined 📦
A multi-episode pack — episode ranges, or "complete / batch" whole-season packs.
```
Loki S01 E01-E06.mkv
One Piece Complete Season 1.mkv
Attack on Titan S04 Batch.zip
EP01 to EP12 720p
```

### 6.4 — Split ✂️
A multi-part upload — split file parts.
```
BigMovie.2021.1080p.mkv.001
Season.Pack.7z.002
film.part1.rar
Movie.cd2.avi
```

> 🔀 A file can be **several categories at once**. Example: `Loki S01 E01-E06.mkv.001` is *TV Show + Combined + Split*, all together.

### 6.5 — Routing each category to its own channel

Since one file can match multiple categories, combine **Priority + Exclusive stop** so each file lands in exactly one place. Recommended setup (highest priority first), all with **Exclusive stop ON** and **Must match ALL ON**:

| Priority | Rule (categories) | Destination |
|:---:|---|---|
| 60 | Combined **+** Split **+** TV Show | Combined-Split-Series channel |
| 50 | Combined **+** TV Show | Combined-Series channel |
| 40 | Split **+** TV Show | Split-Series channel |
| 30 | TV Show | Series channel |
| 20 | Split **+** Movie | Split-Movies channel |
| 10 | Movie | Movies channel |

This exact setup is available as a ready-to-import recipe — see [Section 10](#-10-ready-made-rule-recipes).

> 📝 **Worked example:** a post `Loki S01 E01-E06.mkv` is detected as *TV Show + Combined* → matches the priority-50 rule first (Exclusive stop) → goes **only** to the Combined-Series channel.

---

## ⏪ 7. Backfill

Normally ForwardX only forwards **new** messages. **Backfill** sends the messages that *already exist* in a channel's history — perfect for when you set up a rule *after* the content was posted.

**Open it:** **Rules** tab → **Backfill** (top right).

### 7.1 — How it works
It scans the source **once** and runs every historical message through **all** the rules for that source — so it obeys the exact same filters and category routing as live forwarding.

### 7.2 — Options

- **Source channel** — pick which source to import (only sources with at least one enabled rule are listed). A 🏷️ badge means that source routes by category.
- **Range** — how much history to import:
  - **All messages** — the entire history.
  - **Last N messages** — the newest N (slider, 50–5000).
  - **New messages only** — just the messages posted **since your last completed backfill** of this source. It's fast because it skips re-scanning the whole history — perfect for a quick "top up" after you've already imported once.
  - **Message range** — a precise slice using message links/numbers:
    - **From message** *(optional)* — start here (blank = oldest).
    - **To message** *(optional)* — stop here (blank = latest).
    - Get a message link: in Telegram, long-press a message → **Copy Link** (or just note its number).
    - 📝 From `.../1200`, To blank → message 1200 onward. From blank, To `.../5000` → everything up to 5000. Both filled → just that slice.
- **Order** — **Oldest first** *(recommended, keeps original order)* or **Newest first**.
- **Preview matches** — a dry run showing how many messages *would* forward vs. be skipped, **before** anything is sent.
- **Start backfill** — begins the run, with a live progress bar, **Forwarded / Skipped / Failed** counts, and an ETA. A notification keeps it going even if you leave the screen.

### 7.3 — Pause, Stop & Resume
- **Pause / Resume** — temporarily halt and continue.
- **Stop** — ends the run but **saves your place**.
- **Resume later** — reopen Backfill for the same source → a **"Resume available"** banner appears → tap **Resume** to continue exactly where you left off (or **Start over** to restart). Already-forwarded messages are auto-skipped, so nothing is ever sent twice.

> 🐢 Backfilling a huge channel sends a lot of messages, paced by the anti-flood setting (Section 8) to keep your account safe — big imports simply take a while.

### 7.4 — Catch up on messages missed while offline

Live forwarding only works while ForwardX is actually running. So if your phone was **switched off**, the app was **closed**, or you **lost internet**, any messages posted during that gap were never forwarded — they slip through the cracks. ForwardX can fill that gap for you in two ways:

- 🟢 **Automatically** — turn on **Auto catch-up on startup** in Settings. Every time the app reopens and reconnects, it checks how far behind it is and quietly forwards **just the messages you missed**, then carries on live. (It only runs when the main power switch is ON.)
- 👆 **Manually** — when auto catch-up is off, a **"Catch up on missed messages"** card appears on the **Home** screen whenever there's a gap. One tap forwards the missed messages. (The card hides itself while a catch-up or backfill is already running, so it never gets in the way.)

Behind the scenes this is simply a **"New messages only"** backfill (Section 7.2), so it's quick — and thanks to duplicate protection, it never re-sends anything you already have.

> 🔔 **You'll know when it's done:** whenever a backfill or catch-up finishes, ForwardX posts a notification with the result (e.g. *"1,240 forwarded · 88 skipped · 3 failed"*) — so you don't have to sit and watch a long import.

---

## ⚙️ 8. The Settings page

| Setting | What it does |
|---|---|
| 🔁 **Start on boot** | Automatically resumes forwarding after your phone **restarts** — you don't have to open the app. (Just opening the app also resumes forwarding on its own.) |
| 📥 **Auto catch-up on startup** | When the app starts and reconnects, automatically forwards anything posted in your sources **while it was offline**, then continues live (see Section 7.4). **Off by default.** Runs only when the main power switch is ON. |
| 🛡️ **Duplicate protection** | Never forwards the same message twice (survives restarts). Scope: **Per rule** *(default)* or **Per destination** (skip if it already reached that destination via *any* rule — great when several sources feed one channel). |
| 🐢 **Min send interval** | Minimum gap between two sends. **Higher = safer** from Telegram rate limits. Start around `1200 ms`, raise for big backfills. |
| ⏱️ **Global delay** | Extra pause added before every send, on top of each rule's own delay. |
| 🎨 **Theme** | System / Light / Dark. |
| 💾 **Export / Import rules** | Back up all rules to a JSON file, or load rules from a file — this is how you use the [recipes](#-10-ready-made-rule-recipes). |
| 🚪 **Log out** | Disconnects your Telegram session and returns to the login screen. |
| ℹ️ **About** | Credits and links to other projects. |

**Other screens:** 📄 **Logs** shows every forward/skip/failure with the reason. 📊 **Stats** shows per-rule totals.

> 🧠 **Why anti-flood matter:** Telegram limits how fast an account can send. Too fast triggers a temporary "FLOOD_WAIT," or worst case, a ban. ForwardX funnels **all** sends through one paced queue to stay under the limit — that's why sends are spaced out on purpose.

---

## 🔄 9. Always-on: every situation explained

Confused about what forwards, when, and why? It all comes down to **3 switches** and **2 ways a message gets delivered**.

### The 3 switches

| Switch | Where | What it does |
|---|---|---|
| 🔘 **Power button** | Home | The master ON/OFF. **Nothing forwards unless this is ON.** |
| 🔁 **Start on boot** | Settings | After the phone **restarts**, turns the power back on by itself. |
| 📥 **Auto catch-up** | Settings | After being **offline**, automatically forwards the messages that were missed. |

### The 2 ways a message reaches the destination

- ⚡ **Live** — forwarded the *instant* it's posted — but only while ForwardX's background worker is alive.
- ⏪ **Catch-up** — forwards messages missed *while the worker wasn't alive* (automatically, or by tapping the Home card).

> 🏆 **The one golden rule:** messages forward **only while the background worker is alive.** Everything else is just about (a) keeping it alive and (b) filling the gaps from when it wasn't. The worker **keeps running even when you swipe the app away** — it only dies when the **phone turns off** or **Android kills it** to save battery.

### Every situation — you post a file in the source

**When the Power button is ON:**

| Situation | Worker alive? | The file… | When you reopen the app |
|---|:---:|---|---|
| App open, you're using it | ✅ | forwarded **instantly** (live) | nothing to do |
| You swipe the app away | ✅ *(it survives)* | forwarded **instantly** (live) | nothing to do |
| Android killed it in the background | ❌ | **missed** during the dead time | forwarding resumes → Auto catch-up **ON**: sent automatically · **OFF**: tap the catch-up card |
| Phone powered off / restarted | ❌ | **missed** while off | see *"After a restart"* below |

**When the Power button is OFF:** nothing is forwarded at all, in any situation — and catch-up won't run either (it needs Power ON).

### After a phone restart

| Start on boot | What happens |
|---|---|
| **ON** | Forwarding turns itself back on automatically — no need to open the app. |
| **OFF** | Forwarding stays off until you **open the app** (opening it turns forwarding back on). |

Then, once forwarding is back on:

| Auto catch-up | The files missed while the phone was off… |
|---|---|
| **ON** | get forwarded **automatically**. |
| **OFF** | wait for you — the **catch-up card** appears on Home; tap it to send them. |

> ⚠️ **Start on boot only does something if the power was ON before the phone turned off.** If you'd already turned forwarding off, it stays off after a reboot.

### ✅ The simple recommendation

For truly hands-free, never-miss-anything forwarding, turn on all three:

> **Power ON  +  Start on boot ON  +  Auto catch-up ON**

That way, after *any* reboot or background-kill, ForwardX restarts itself, forwards anything it missed, and keeps going — you never have to touch it. And if you ever open the app and see **no catch-up card**, that means nothing was missed. 🎯

---

## 🍱 10. Ready-made rule recipes

Import these to get started fast: **Settings → Import rules** → paste the JSON (or load the file). After importing, **open each rule** and set its **From**/**To** — recipes ship with placeholders since only you know your channel IDs.

| Recipe | What it does |
|---|---|
| `simple-mirror.json` | Forwards **everything** from one chat to another. |
| `movies-clean-captions.json` | Forwards only **movies**, in copy mode, with fully cleaned captions. |
| `keyword-and-schedule.json` | Only `1080p`/`4k` videos over 100 MB, skips samples/ads, overnight only. |
| `media-routing-rules.json` | The full **6-category** routing set (Movies, Split Movies, TV, Split TV, Combined TV, Combined Split TV) with priority + exclusive-stop. |

> **Category values for JSON:** `"MOVIE"`, `"TV_SHOW"`, `"COMBINED"`, `"SPLIT"`
> **Media types:** `"ALL"`, `"TEXT_ONLY"`, `"MEDIA_ONLY"`, `"PHOTOS"`, `"VIDEOS"`, `"DOCUMENTS"`, `"AUDIO"`, `"VOICE"`
> File sizes are in **bytes** (100 MB = `104857600`). Schedule times are **minutes from midnight** (`1320` = 22:00). `scheduleDaysMask` is a bitmask (`127` = every day).

---

## 🆘 11. Tips, safety & troubleshooting

- ✅ **Keep forwarding reliable:** grant the battery-optimization exemption, enable **Start on boot**, and turn on **Auto catch-up on startup** so anything missed during downtime is forwarded automatically.
- 🚫 **Avoid bans:** don't set the send interval too low. For big backfills, raise **Min send interval** first.
- ♾️ **"Connecting…" won't go away?** Make sure you're logged in and online — a fresh login walks through phone → code → (password).
- 🔍 **Nothing is forwarding?** Check: the **Home** toggle is ON, the rule is **enabled**, the **source** matches where messages actually arrive, and filters aren't too strict. Use **Test** or **Preview** — the **Logs** screen shows the exact reason.
- ✂️ **Caption not cleaned?** Caption edits only apply in **Copy mode**.
- 🔒 **Protected ("no-save") channels:** messages Telegram blocks from saving can't be forwarded or copied, and are skipped automatically.
- 🗂️ **Your data:** everything (session, rules, credentials) stays **on your device** — nothing is uploaded anywhere.

---

<div align="center">

### Made with ❤️ by **Karan (Weebzone)**

</div>
