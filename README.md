# ChronosGG — Free Gaming Zone & Cyber Café Management Software (Windows, LAN, Offline)

**ChronosGG** is free, self-hosted **gaming zone management software** for running a
**cyber café**, **net café**, or **esports lounge** on pay-per-time gaming PCs. One operator
**Hub** runs the dashboard and billing; a lightweight **Agent** runs on every gaming PC to
track time, show countdown alerts, and lock the machine when a session ends. Everything runs
over your local network — fully **offline**, no cloud, no subscriptions, no internet
required.

---

## What it is

A **cyber café billing software** / **game center management** system built for real gaming
zones: bill customers by the hour, with prepaid time, or with named packages; watch every PC
live from one dashboard; lock a PC automatically the moment paid time runs out; and generate
daily and monthly revenue reports without any cloud service in the loop. Built for
**gaming café Pakistan** operators first — pricing is in **PKR**, rounded to the nearest ten —
but works for any LAN gaming center regardless of currency conventions.

---

## Key features

- **Bill by the hour, prepaid, or packages** — flexible per-time-tracking billing with
  per-PC rate overrides and package overage handled automatically.
- **Lock PCs automatically when time's up** — a full-screen lock overlay appears the moment
  a session expires, with threshold voice alerts at 10 and 5 minutes remaining.
- **Manage every PC from your phone on the same Wi-Fi** — an embedded web companion lets
  you open the Hub's IP address in any browser on the LAN and control sessions remotely.
- **Daily & monthly revenue reports as PDF/CSV** — colorful branded PDF reports plus raw
  CSV export, broken down by day, month, PC, and session.
- **Works fully offline on your LAN** — no internet connection needed to run the zone;
  your session and revenue data stays on your own Hub PC.
- **Bilingual English + Urdu announcements** — spoken alerts in English and Urdu with
  selectable voice language. Both languages ship with audio today (the Urdu clips are
  auto-generated placeholders that can be upgraded to studio recordings).
- **PC lock & lockdown on Windows** — keyboard-hook based lockdown blocks Alt+Tab and Task
  Manager while a PC is locked, with autostart and single-instance protection. This
  lockdown layer is in validation and pending final verification on real Windows hardware
  before it should be treated as fully hardened.
- **Offline admin bypass** — staff can unlock any PC with a shared admin credential even if
  the Hub server is down, cached locally on each Agent.
- **MAC-based PC identity** — a PC keeps its assigned number and rate even if its IP address
  changes.
- **Self-hosted and open-source** — no accounts, no telemetry, no per-seat fees; run it on
  your own hardware and keep your data.

---

## Screenshots

*(Images are added at release time — placeholders below.)*

- Desktop Hub dashboard — live PC grid, session controls: `docs/screenshots/hub-dashboard.png`
- Web companion (mobile view) — remote session control from a phone: `docs/screenshots/web-companion.png`
- Sample PDF revenue report: `docs/screenshots/report-pdf.png`

---

## Download & Install

1. Go to the **[Releases](../../releases)** page of this repository.
2. Download **`ChronosGG-Hub-Setup.exe`** and **`ChronosGG-Agent-Setup.exe`** (both Windows).
3. Run **`ChronosGG-Hub-Setup.exe`** on the counter / operator PC — this installs the Hub to
   Program Files with a Start Menu shortcut and an uninstaller. It offers an optional
   "start on Windows" checkbox.
4. Run **`ChronosGG-Agent-Setup.exe`** on every gaming PC you want to manage. Setup asks for
   the **Zone Secret** shown on the Hub's Settings screen (you can leave it blank and set it
   later) — the Agent then auto-starts automatically on every Windows boot.
5. Agents auto-discover the Hub on the LAN — no manual IP entry needed in most setups.

Both apps currently target **Windows**. Portable `ChronosGG-Hub.exe` / `ChronosGG-Agent.exe`
builds (no installation, no shortcuts) are also attached to each release for advanced users.

---

## Quick start

1. Start the Hub on your counter PC; open its dashboard.
2. Start the Agent on a gaming PC — it will appear as **Unregistered** in the Hub.
3. Assign it a PC number from the Hub's dashboard.
4. Start a session (rate, prepaid, or package) on that PC tile — the Agent shows the
   countdown HUD immediately.
5. Open `http://<hub-ip>:<port>` from your phone on the same Wi-Fi to manage sessions
   remotely, logging in with your admin credential.

---

## FAQ

**Does it need internet?**
No. ChronosGG runs entirely over your local network (LAN). There's no cloud dependency.

**What does it cost?**
It's free.

**Which OS does it run on?**
Windows, for both the Hub and the Agent.

**Can I use it on my phone?**
Yes — the Hub includes a built-in web companion. Open the Hub's IP address from any phone
or tablet browser on the same Wi-Fi network and log in with your admin credential.

**Is my data private?**
Yes. Everything is stored locally on the Hub PC (SQLite); nothing is sent to any external
server.

---

## Who is this for

Owners and operators of **gaming zones**, **cyber cafés**, **internet cafés**, **net cafés**,
**esports lounges**, and **gaming lounges** who need practical **PC timer** / **time-tracking**
and **pay-per-time** billing without buying into an expensive commercial **café management
system**. If you're searching for **cyber cafe billing software**, an **open-source cyber
cafe software** option, or a **game center management** tool that runs fully **self-hosted**
and **offline** with no per-seat license fees, ChronosGG is built for that use case —
including **gaming café Pakistan** operators billing in PKR.

---

**Keywords:** gaming zone management software, cyber café management, internet café software,
net café software, esports lounge management, gaming lounge PC management, LAN gaming center,
pay-per-time billing, time-tracking software, PC timer, prepaid billing, package billing,
cyber cafe billing software, PC lock software, session control, café management system,
gaming café Pakistan, PKR billing, self-hosted software, offline software, no-cloud software,
open-source cyber cafe software, game center management.

---

**Author:** Faisal Malik
