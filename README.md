# ChronosGG — Free Gaming Zone & Cyber Café Management Software (Windows, LAN, Offline)

**ChronosGG** is free, self-hosted **gaming zone management software** for running a
**cyber café**, **net café**, or **esports lounge** on pay-per-time gaming PCs. It comes as
**two apps**:

| App | Install it on… | What it does |
|-----|----------------|--------------|
| 🖥️ **ChronosGG Server** | Your **counter / reception PC** (one per café) | The operator dashboard — start/stop sessions, billing, packages, reports, and a web companion. |
| 🎮 **ChronosGG Client** | **Every gaming PC** you want to meter | Shows the countdown, plays time-up voice alerts, and locks the PC when paid time runs out. |

> **Rule of thumb:** the **Server** runs where *you* sit; a **Client** runs on every PC a
> *customer* plays on. You install the Server **once**, and the Client on **each** gaming PC.

Everything runs over your local network — fully **offline**, no cloud, no subscriptions, no
internet required.

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

- **Bill by the hour, prepaid, or packages** — flexible per-time billing with per-PC rate
  overrides and package overage handled automatically.
- **Lock PCs automatically when time's up** — a full-screen lock overlay appears the moment
  a session expires, with threshold voice alerts at 10 and 5 minutes remaining.
- **Manage every PC from your phone on the same Wi-Fi** — an embedded web companion lets
  you open the **Server's** IP address in any browser on the LAN and control sessions remotely.
- **Daily & monthly revenue reports as PDF/CSV** — colorful branded PDF reports plus raw
  CSV export, broken down by day, month, PC, and session.
- **Works fully offline on your LAN** — no internet connection needed to run the zone;
  your session and revenue data stays on your own **Server** PC.
- **Bilingual English + Urdu announcements** — spoken alerts in English and Urdu with a
  selectable voice language. (Urdu clips currently ship as auto-generated placeholders that
  can be upgraded to studio recordings.)
- **PC lock & lockdown on Windows** — keyboard-hook lockdown blocks Alt+Tab and Task Manager
  while a PC is locked, with autostart and single-instance protection.
- **Offline admin bypass** — staff can unlock any PC with a shared admin credential even if
  the Server is down, cached locally on each Client.
- **MAC-based PC identity** — a PC keeps its assigned number and rate even if its IP changes.
- **Self-hosted and open-source** — no accounts, no telemetry, no per-seat fees; run it on
  your own hardware and keep your data.

---

## Download & Install

Go to the **[Releases](../../releases)** page and download the two installers:

### 1. On the counter / reception PC → install the **Server**
Run **`ChronosGG-Server-Setup.exe`**. It installs the operator dashboard to Program Files with a
Start Menu shortcut and an uninstaller, and offers an optional "start on Windows" checkbox.
That's the whole Server setup — nothing to configure.

### 2. On every gaming PC → install the **Client**
Run **`ChronosGG-Client-Setup.exe`** on each PC you want to meter. **No secret, no IP, nothing
to enter** — the Client auto-starts on every Windows boot, **auto-discovers the Server on the
LAN**, locks the PC, and shows up on the dashboard ready to bill. Install and it just works.

Both apps target **Windows**. Portable `ChronosGG-Server.exe` / `ChronosGG-Client.exe` builds
(no installation, no shortcuts) are also attached to each release for advanced users. Both apps
**update themselves automatically** after install.

---

## Quick start

1. Install and open the **Server** on your counter PC.
2. Install the **Client** on a gaming PC — it appears as **Unregistered** on the Server's dashboard.
3. Assign it a PC number from the dashboard.
4. Start a session (rate, prepaid, or package) on that PC tile — the Client shows the countdown
   immediately.
5. Open `http://<server-ip>:<port>` from your phone on the same Wi-Fi to manage sessions
   remotely, logging in with your admin credential.

---

## FAQ

**Which app do I install where?**
The **Server** goes on your one counter/reception PC (the operator dashboard). A **Client** goes
on every gaming PC you want to charge for. See the table at the top.

**Does it need internet?**
No. ChronosGG runs entirely over your local network (LAN). There's no cloud dependency.

**What does it cost?**
It's free.

**Which OS does it run on?**
Windows, for both the Server and the Client.

**Can I use it on my phone?**
Yes — the Server includes a built-in web companion. Open the Server's IP address from any phone
or tablet browser on the same Wi-Fi network and log in with your admin credential.

**Is my data private?**
Yes. Everything is stored locally on the Server PC (SQLite); nothing is sent to any external
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

## Platforms

ChronosGG runs on **Windows** and **Linux** (x86_64), and they interoperate — a Linux
Server happily runs Windows Clients and vice versa.

| Download | Use it for |
|---|---|
| `ChronosGG-Server-Setup.exe` | Windows counter PC |
| `ChronosGG-Client-Setup.exe` | Windows gaming PC |
| `ChronosGG-Server-linux-x86_64.tar.gz` | Linux counter PC — extract, run `./ChronosGG-Server` |
| `ChronosGG-Client-linux-x86_64.tar.gz` | Linux gaming PC — extract, run `./ChronosGG-Client` |

> ⚠️ **The Linux Client is not a hardened kiosk.** Wayland forbids global keyboard grabs
> and nothing in userland can block `Ctrl+Alt+F<n>` VT switching, so the lock overlay
> appears but keyboard shortcuts are not blocked. It deters casual use; it does not stop
> someone who knows Linux. **Run gaming PCs on Windows**, or harden the Linux session
> itself. The Linux **Server** has no such limitation.

---

Built by **[zylio](https://zylio.net)** — an independent software studio building fast, honest
tools for power users and gamers.

**Product page:** [zylio.net/software/chronosgg](https://zylio.net/software/chronosgg)

© 2026 zylio. All rights reserved.
