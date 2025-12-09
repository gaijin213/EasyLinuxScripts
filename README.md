# EasyLinuxScripts

Hi — I'm glad you're here. I started on computers when CDs were a luxury, Windows was the everyday, and a mis-click could feel like a personal betrayal. Switching to Linux years later felt like finally getting the keys to a house I’d been visiting for decades: exciting, liberating, and — I’ll admit — occasionally confusing.

EasyLnuxScripts is my small, ongoing collection of scripts and helpers I wrote for myself (and my friends) during that transition. I add things here as I build them, tidy them up, and imagine how they could save someone else a late-night troubleshooting session. This repo is about empathy first: scripts that do a little heavy lifting while teaching you what they're doing.

---

## 🚀 Why I made this

When I moved from Windows to Linux I kept stumbling over the same tiny things: installing the right packages, setting up SSH keys, restoring bookmarks, or making a familiar app feel like home. I wrote little utilities to solve those friction points, and after helping a few friends get unstuck, it made sense to keep the scripts in a place others could find and contribute to.

This repo is for the person who wants to learn, not just automate blindly. Each script is a chance to understand why something works — and to gain confidence.

---

## A short personal note

I love hearing "Oh wow, that just worked" from someone who thought it would be difficult. I also remember the times I broke my setup because I ran a script without reading it. So, you'll find my scripts are conversational in style: clear comments, safe defaults, and an occasional aside like "this part confused me the first time too."

---

## What you’ll find here

- scripts/ — small, focused helpers (shell, Python) with comments and usage info
- examples/ — sample config files and tiny dotfile snippets
- docs/ — longer write-ups for tricky tasks and step-by-step walkthroughs
- LICENSE — usually MIT for simplicity and reuse
- CONTRIBUTING.md — how I prefer contributions (coming soon)

Typical scripts I add:
- Basic setup helpers: create a user, add SSH keys, install a set of packages
- Installer helpers: safely create a USB installer with clear checks
- Package helpers: small wrappers to install the same tool on Debian/Fedora/Arch
- Dotfiles backup and restore examples
- Small desktop tweaks to get keyboard shortcuts or default apps feeling familiar

---

## How I write scripts here (and why)

- Small, single-purpose scripts. One job, one file.
- Human-friendly comments — I explain why, not just what.
- Safety options: --help, --dry-run, --interactive when appropriate.
- POSIX-first, but pragmatic: sometimes Python helps readability.
- Tested on a VM or throwaway environment before I commit.

I want you to be able to read a script and understand the train of thought that produced it.

---

## Safety: please, please read first

I cannot stress this enough: scripts change systems. I add safety checks, but always:

1. Read the script top to bottom.
2. Run with --dry-run when available.
3. Test in a VM, Live USB, or a disposable machine if the script touches disks, partitions, or users.
4. Back up your data before running anything that alters files or system settings.

Example flow I use:
1. Inspect the script in my editor
2. Run `./scripts/some-script.sh --dry-run`
3. Run interactively: `./scripts/some-script.sh --interactive`

---

## How to use this repo

1. Clone:
   git clone https://github.com/<your-org>/EasyLnuxScripts.git
2. Inspect the script you want to run and read its header.
3. Make it executable and test with help/dry-run flags:
   chmod +x ./scripts/setup-basic.sh
   ./scripts/setup-basic.sh --help
4. Only use sudo when the script requires it, and review prompts.

---

## Want to contribute?

Yes — please. Things I appreciate:
- Small, focused PRs with a clear use-case and test steps.
- Scripts that explain themselves and include a --help section.
- Notes about which distros you tested on and what worked.
- If a script touches disks or networking, open an issue first so we can discuss safety.

If you're not comfortable creating a PR, open an issue describing the problem you want solved and I can sketch a script.

---

## Roadmap (personal wishlist)

- First trio: setup-basic.sh, install-common-packages.sh, create-usb-installer.sh
- CONTRIBUTING.md with clear safety checklist and style rules
- A "first 24 hours" walkthrough for people booting Linux for the first time
- Small collection of dotfiles for common setups (Neovim, zsh, GTK/Qt tweaks)

---

## License & attribution

Most things here use the MIT License. If you adapt a script, please keep the author header so we remember who helped. I’ll do the same when I use someone else’s work — credit matters.

---

Thanks for stopping by. If you’re migrating from Windows and feeling unsure, you’re not alone — drop an issue, tell me what caused you the most friction, and I’ll try to add a script or a doc that would have helped me when I started.

Welcome to tinkering, welcome to learning, and most of all: welcome to the open world. 🐧
