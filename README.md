# NEXUS — Investor & Entrepreneur Platform

A multi-page web platform connecting investors and entrepreneurs. Built with **pure HTML, CSS, and JavaScript** — no frameworks, no npm, no build step required.

> 🌐 **Live Demo:** [nexus-iota-five.vercel.app](https://nexus-iota-five.vercel.app)

---

## 📸 Pages Overview

| Page | Description |
|------|-------------|
| `dashboard.html` | Main hub — links to all modules with guided walkthrough tour |
| `calendar.html` | Meeting scheduler — book, accept, decline investor meetings |
| `video-call.html` | Video calling — camera, mic, screen share, in-call chat |
| `documents.html` | Document chamber — upload, e-sign, track contracts & NDAs |
| `payments.html` | Payments — send/receive funds, transaction history |
| `security.html` | Security center — 2FA, password strength, sessions, roles |

---

## 🗂️ Project Structure

```
nexus-website/
├── index.html            → Redirects to dashboard
├── dashboard.html        → Week 3: Main hub + guided tour
├── calendar.html         → Week 1: Meeting calendar
├── video-call.html       → Week 2: Video calling UI
├── documents.html        → Week 2: Document chamber
├── payments.html         → Week 3: Payments & transactions
└── security.html         → Week 3: Security & 2FA
```

---

## ✨ Features

### 📅 Meeting Calendar
- Monthly calendar grid with meeting markers
- Schedule, accept, and decline investor meetings
- Availability slot management
- Meetings list with filter tabs (All / Pending / Confirmed / Declined)

### 🎥 Video Call
- Lobby with scheduled & live call cards
- Real camera & microphone via `getUserMedia`
- Screen sharing via `getDisplayMedia`
- Draggable picture-in-picture local video tile
- In-call chat drawer with simulated replies
- Mute, camera off, fullscreen controls
- End-call summary modal with duration stats

### 📁 Document Chamber
- Table-based file manager with search & filter
- Upload via drag-and-drop or file browser
- Create documents from 6 templates (NDA, Term Sheet, Investment Contract, etc.)
- E-signature pad (draw with mouse or touch)
- Status workflow: Draft → In Review → Signed
- Slide-in preview drawer for each document

### 💳 Payments
- Wallet balance display with monthly change %
- Send money with recipient picker
- Transaction history grouped by date (filterable)
- Deposit, Withdraw, Transfer modals
- Fund a Deal — direct investor → entrepreneur transfer
- Mini bar chart for income trend
- Success confirmation with reference number

### 🔐 Security Center
- Security score ring (0–100) that updates live
- Password strength meter (4 levels + 6 real-time requirement checks)
- Two-factor authentication setup (Authenticator App / SMS / Email)
- OTP 6-digit input for 2FA verification
- Active sessions list with revoke controls
- Role-based permissions viewer (Entrepreneur vs Investor)
- 7-day security activity log

### 🏠 Dashboard
- Time-aware greeting (morning / afternoon / evening)
- Module cards with live stats and notification badges
- 6-step guided walkthrough with spotlight tooltip system
- Recent activity timeline (filterable by category)
- Quick actions grid
- Week progress bars

---

## 🎨 Design System

Each page has a **distinct visual identity** while sharing a unified top navigation bar.

| Page | Theme | Font |
|------|-------|------|
| Dashboard | Warm editorial, serif | Fraunces + DM Sans |
| Calendar | Dark navy + blue accent | DM Serif Display + DM Sans |
| Video Call | Cinematic black + cyan | Syne + Inter |
| Documents | Parchment paper, light | Playfair Display + IBM Plex Sans |
| Payments | Dark fintech terminal | Space Grotesk + Space Mono |
| Security | Clinical white + blue | Outfit + JetBrains Mono |

**Shared nav:** All pages include a fixed black top navbar (`NEXUS` brand + page links + user info) that highlights the active page in green.

---

## 🛠️ Tech Stack

| Layer | Choice |
|-------|--------|
| Markup | Vanilla HTML5 |
| Styling | Vanilla CSS3 (CSS variables, Grid, Flexbox) |
| Logic | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts |
| Camera/Mic | WebRTC (`getUserMedia`, `getDisplayMedia`) |
| Signature | HTML5 Canvas API |
| Framework | **None** |
| Build tool | **None** |
| Dependencies | **None** |

---

## 📅 Development Weeks

| Week | Tasks | Status |
|------|-------|--------|
| Week 1 | Meeting Calendar (schedule, accept/decline, availability) | ✅ Done |
| Week 2 | Video Call UI + Document Chamber with e-signature | ✅ Done |
| Week 3 | Payments, Security Center, Dashboard + guided tour | ✅ Done |

---

## 📁 How Pages Are Connected

Every page has a shared fixed topnav that links to all other pages via plain `<a href="...">` tags. The active page is highlighted. Clicking Dashboard module cards also navigates to the respective page.

```
index.html → dashboard.html
dashboard.html → calendar.html, video-call.html, documents.html, payments.html, security.html
(and back from every page via topnav)
```

---

## 🖥️ Browser Support

| Browser | Support |
|---------|---------|
| Chrome / Edge | ✅ Full (including camera/screen share) |
| Firefox | ✅ Full |
| Safari | ✅ Full (camera works, screen share limited by OS) |
| Mobile Chrome | ✅ Responsive |
| Mobile Safari | ✅ Responsive |

> **Note:** Camera and microphone features require HTTPS or localhost. They will not work on `file://` URLs.

---

## 📄 License

This project was built as part of a frontend internship. All code is original and open for educational use.

---

<div align="center">
  Built with ❤️ using pure HTML · CSS · JavaScript — no frameworks needed
</div>
