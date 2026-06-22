# Organization Asset Library for PowerPoint Templates

> A single-page, interactive guide for SharePoint admins.
> It makes corporate PowerPoint templates show up for **every user** in the tenant, under **File then New**.

**Live page:** https://eriic-builds.github.io/oal-live-guide/

The whole guide is **one self-contained HTML file**.

- No build step.
- No dependencies.
- Open it in a browser, or host it as a static page.

---

## What you get

> You finish with branded `.potx` templates in a tab named after your organization, inside **PowerPoint on desktop and web**.

- Every user sees the **same** templates.
- They click one and start an on-brand deck.
- You get there in **nine short steps**.
- The PowerShell commands fill in your own **tenant**, **site**, and **library** names as you type.

---

## The job this does for you

You came here to make progress on **one thing**:

> Push approved templates to everyone, and have them appear the same way for each person.

### The problem today

The official Microsoft docs are spread across **four pages**.

| Page | Covers |
| --- | --- |
| 1 | The library |
| 2 | The PowerShell |
| 3 | Saving a `.potx` |
| 4 | How users open the gallery |

None of them walk the **full path** end to end.
None of them warn you about the parts where it breaks.

### What you fire when you adopt this

- Searching four doc pages and stitching them together yourself.
- Running the command, hitting a cryptic error, and starting over.
- Guessing whether **templates**, **images**, or **Brand Kits** is the right feature.

You read **one page**, top to bottom, and you are done.

---

## Why this guide is different

The value here is the part the official docs **do not say**.

These were learned by running the setup, hitting the real errors, and correcting course:

| The trap | What works |
| --- | --- |
| Read permission on the **site** | It must go on the **document library**. Path: Settings, then Site permissions, then Share site, set to **Read**. |
| Uploading a `.pptx` | Templates must be `.potx`. A `.pptx` does not appear in the gallery. |
| The CDN prompt | Answer **Y**. It is the default and the right choice. It ships with your SharePoint Online subscription. |
| `-CopilotSearchable` on templates | The server **rejects** it. It does not work on a template library. |
| OAL vs Brand Kit | **OAL** powers the File then New gallery. A **Brand Kit** applies your theme to Copilot content. Different features, run in parallel. |

> If you removed everything the Microsoft docs already cover, the table above is what remains.
> This is the reason to keep this page.

---

## What is inside

| Step | Section |
| --- | --- |
| Intro | Why this guide exists, and OAL vs Brand Kit |
| 01 | Prerequisites. Licensing, app versions, roles, limits |
| 02 | Build the SharePoint site and library from scratch |
| 02 C | Set permissions, with the exact click path |
| 03 | Build, save, and upload your `.potx` templates |
| 04 | Install the SharePoint Online Management Shell |
| 05 | Connect to SharePoint |
| 06 | Register the library with one command |
| 07 | How users find the templates on Windows, Mac, web |
| 08 | Manage and update commands |
| 09 | Gotchas checklist |

---

## Built-in features

- **Personalize bar.** Type your tenant, site, and library once. Every URL and command updates as you type.
- **Three reading modes.** Light, Dark, and a **dyslexia-friendly Reading mode** with a warm background, a readable font, and looser spacing.
- **Side rail.** Tracks your place as you scroll. Lets you jump between sections.
- **Per-command copy buttons.** Take one command at a time.

---

## Who this is for

- SharePoint Administrators.
- Microsoft 365 admins.
- The people who own brand templates for an organization.

> You do not need to be a developer.
> You need admin access and a few minutes.

---

## How to use it

1. Open the HTML file in a browser.
2. Type your **tenant**, **site**, and **library** into the personalize bar at the top.
3. Follow the **nine steps** in order.
4. Copy each command as you reach it.

**To host it as a public page:** rename the file to `index.html` and serve it from any static host, such as GitHub Pages.

---

## Grounding and disclaimer

Built and grounded on **official Microsoft documentation**, plus hands-on testing against a live tenant.

> **Unofficial community resource. Not affiliated with Microsoft.**

**Sources**

- Microsoft Learn, Create an organization assets library.
- Add-SPOOrgAssetsLibrary cmdlet reference.
- Microsoft Support, Use your organization's templates in PowerPoint.
- Microsoft Support, Create and save a PowerPoint template.

---

## Why I built this

Three reasons.

**1. Learn the process.**

- The OAL setup was new to me.
- The best way to learn a thing is to do it and write it down.
- Building the guide forced me to understand every step.

**2. Use AI to build something useful to me.**

- Not a generic doc.
- A guide shaped to how I read and how I work.
- I directed it, tested it, and corrected it until it fit.

**3. Learn to host it.**

- GitHub Pages, git, commits, branches.
- Publishing a page was a skill I did not hold.
- So I made a real page worth publishing, and learned hosting by shipping it.

---

### How this came together

I built it in a **loop**, not in one pass.

- **Caught the wrong source.** The first doc covered brand images, not templates. I switched before building.
- **Found real bugs.** The side rail vanished at one width. The scroll tracking lit the wrong section. I fixed both.
- **Ran the real PowerShell.** I hit a permission error, a CDN prompt, and a Copilot rejection. Each fix went back into the guide.
- **Rewrote it in my own voice.** So it did not read like generated filler.

> I kept testing it against reality, not against my assumptions.

---
