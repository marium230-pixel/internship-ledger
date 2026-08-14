# 📓 The Internship Ledger

A single-page task tracker built to manage multiple concurrent internships at once.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![No Build Step](https://img.shields.io/badge/Build%20Step-None-6E4B3A?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Live-4E8B5C?style=for-the-badge)

**🔗 Live app:** https://internship-ledger.netlify.app/
**🔗 GitHub Pages:** https://marium230-pixel.github.io/internship-ledger/

---

## 💭 The Story

At one point I was juggling four concurrent internships — FlyRank AI Fluency, Excelerate Flutter Dev, Swiftly Seva UI/UX, and HeyJivu QA — each with its own deadlines, its own cadence, its own idea of what "done" even means. A weekly assignment isn't the same shape of work as a bug severity, which isn't the same shape as a design deliverable. I tried tracking all of it in my head, then in one generic to-do list, and both fell apart the same way: everything blurred into one undifferentiated pile, and I kept losing track of what actually needed me *today*.

This app started as a way to solve that for myself, not as a portfolio exercise. It's built on one real belief: if you're managing several unrelated workstreams at once, your tool should know they're unrelated — not force them into the same shape just because they're all technically "tasks."

## ⚙️ Features

- 🏷️ **Per-internship custom fields** — each internship tracks whatever actually matters to it (Week #, Severity, Deliverable type, etc.), not a generic label
- ➕ **Manage internships live** — add or remove internships without touching code; removing one archives its tasks instead of deleting them
- 🔁 **Recurring tasks** — mark a task to repeat weekly; checking it off auto-schedules the next occurrence
- ⏰ **Snooze** — +1 day / +1 week buttons to reschedule without opening an edit form
- 🔍 **Search** — full-text search across every internship and every task at once
- 🗄️ **Archive, not delete** — nothing is destroyed permanently; everything removed lands in an Archived tab and can be restored
- 📊 **Weekly digest** — a quick per-internship breakdown of what's overdue, due this week, and done
- ✅ **"Completed" internship state** — wind down an internship once it ends without losing its history or cluttering active filters
- 🌤️ **Today view** — a stripped-down, single-glance view of just what's due today
- 🎙️ **Voice-to-task** — add a task by speaking instead of typing (requires HTTPS hosting; works on the deployed link)
- 📤 **Export / import backup** — move data between devices as a JSON file

## 🧱 Tech

Single self-contained `index.html` file — vanilla HTML, CSS, and JavaScript, no build step, no framework, no backend. Data is stored in the browser's `localStorage`, so it's private to whoever opens it, per device.

## 🎨 Design

Editorial "daily broadsheet" aesthetic — Playfair Display and Cormorant Garamond for headers, Jost for body text, on a dark mahogany / rose gold / muted copper / blush pink palette. Verified for WCAG AA text contrast and 44×44px minimum touch targets throughout.

## 🔄 Using this for your own internships

This isn't locked to my four internships — it's built to be reused as-is, no code changes needed:

1. Open the [live app](https://internship-ledger.netlify.app/)
2. Tap **"Manage internships"**
3. Remove the ones that aren't yours (✕ next to each — this archives their sample tasks rather than deleting anything, so nothing is lost if you change your mind)
4. Add your own — give it a name, a short monogram (e.g. "AC" for Acme Co.), and whatever custom field actually matters for that work (Week #, Severity, Sprint, Deliverable, Client, etc.)

Your data lives in your browser's local storage, so it's private to your device — if someone else opens the same link, they get their own blank slate, not yours.

## 🚀 Running locally

Just open `index.html` in a browser. Note: voice input requires a secure (`https://`) origin, so it won't work from a local file — it works on the deployed link above.

## ☁️ Deployment

Currently hosted via Netlify Drop. To redeploy after changes, drag the updated `index.html` onto [Netlify Drop](https://app.netlify.com/drop) or push to this repo with GitHub Pages enabled.
