# USJ Group — Business Planning

Context for continuing this work. Read this first.

---

## Who / what

- **Bhanu** — software engineer at **USJ Group**, Dehradun, India.
- Everything here is being prepared for **Uday sir** (director) for approval.
- Bhanu is **not** an MBA. That must be said openly in the scope deck.

## Standing rules — do not break these

1. **Plain simple English.** Short points. Write as if talking. No long paragraphs, no corporate English.
2. **Never put AI names or co-author lines in git commit messages.** Author is `Bhanu <bhanu@usjtechnologies.com>`.
3. Everything is a **proposal for approval**, not a description of an existing business. Use "we would…", "if approved…".
4. In the service sections: **no money, no numbers.** All costs and investment go into one separate "What is needed" section.

## Design system used everywhere

```
--cream:#F0EEE6   --ink:#191919    --ink2:#5A5852   --ink3:#8C8985
--line:#E2DFD5    --clay:#CC785C   --kraft:#D4A27F  --manilla:#EBDBBC
--navy:#3F5A7D    --moss:#5C7052   --plum:#7A5C7D   --sand:#8A7350
```

Serif headings (`ui-serif, Georgia`), sans body. Minimal, no charts, tables + cards only.
Mobile must look **identical to desktop** — no responsive trimming on the PDF-style docs
(done with `<meta name="viewport" content="width=1024">` + `min-width:1024px`).

---

## The three businesses

| Business | What |
|---|---|
| **ChaloKumbh** | Online Pooja, Vedanz, Doon Travellers, USJ Stays |
| **USJ Electronics** | Retail, bulk supply |
| **USJ Technologies** | IT services, software & apps, GeM & tenders |

### Where things actually stand today

- **Doon Travellers** — running. Real cabs, real bookings. This is the proof.
- **ChaloKumbh website** — built and online.
- **Social** — ChaloKumbh has Instagram, Facebook, X, YouTube. Posting only on Instagram + Facebook
  (AI-generated daily Hindu calendar posts, AI reels about temples). USJ Group has LinkedIn.
- **Online Pooja / Vedanz / USJ Stays** — not started.
- **Electronics & Technologies social** — not created.

### Key positioning points already established

- **Online Pooja** — every competitor (including Sri Mandir) sends a **recorded** video afterwards.
  Nobody streams the ghat pooja **live**. Verified. That is the gap.
  Marketing idea: stream Ganga Aarti from Har Ki Pauri free every evening, sell the pooja.
- **Vedanz** — two products: Ganga Jal (couriered anywhere) and packaged drinking water (sold at the ghats).
  Three ways to do the water: (1) someone else's plant + our label, (2) our own plant + BIS/FSSAI licences,
  (3) pure trading. **Recommendation: start with Way 1.** Bhanu still has to confirm this.
- **Doon Travellers** — we do not own vehicles, we partner with operators. Biggest growth lever is
  Google Maps / Google Business Profile.
- **USJ Stays** — we do not own hotels. Hotels list with us, we bring customers, we take a share.
  OYO/Goibibo model but **only for Kumbh regions**. Timing matters: tie up hotels before the Ardh Kumbh rush.
- **The joining idea** — one customer, five earnings. Cab → room → pooja → water → Ganga Jal → repeat pooja.
  Spend on marketing once, earn many times. Nobody else covers the whole journey.
- **Ardh Kumbh Mela 2027** is the target event.
- Every one of the four services needs **a person on the ground in Haridwar**. Nothing moves without that.

### Per-service template (use this for every service, in this order)

1. What it is
2. How it works
3. What we need
4. Why we can do it (USP)
5. How we get customers

---

## The three options for sir (still to be written into the deck)

Bhanu's exact position, in his words:

> Sir wants me to manage the business and get profits. I should first say what I know, what is
> possible in my sense, and what experience I have — that I am a software engineer, not an MBA guy.
> **In any option I will put 100% effort and 100% manage everything if wanted, but 0% blame and
> 0% responsibility taken.** That must be declared clearly.

The three options to present:

1. **Bhanu runs overall business management** — but then the asked investment must be provided
   (hiring, marketing, tools).
2. **Sir decides everything**, Bhanu only executes the software side of his own domain.
3. **Bhanu takes it on** — but with 0% blame for outcomes, including software.

---

## Still to do

- [ ] **USJ Electronics** section — same five-part template
- [ ] **USJ Technologies** section — same five-part template
- [ ] **"What is needed"** section — people, marketing, tools. All money lives here only.
- [ ] **"The three options"** section — must be explained clearly in the deck
- [ ] Short summary PDF (6–7 pages) with the actual ask, once the site is complete

### Waiting on Bhanu

- Salary numbers for the hiring roles
- Whether anyone is already in Haridwar
- Pandit / hotel / taxi contacts
- Vedanz route decision — Way 1 (someone else's plant, our label) vs Way 2 (own plant)
- Which wording to use for the responsibility line

---

## Folders

| Folder | What |
|---|---|
| `01-business-setup/` | Domain + email + social costs. **Approved-style doc.** ₹8,098/yr, ₹675/mo (approx). Google Workspace **Base** ₹99/user/mo × 3. |
| `02-whats-next/` | The 8-step plan + 3 hiring roles, for after sir approves the setup |
| `03-explainer-video/` | The 108s explainer video, its HTML source, the teleprompter, and the narration script |
| `04-business-scope-site/` | **The main active work.** The scope website. |
| `assets/` | USJ logo, full-res and web-sized |
| `archive/` | Earlier drafts. Reference only. |

## Git

The **whole** Business Planning folder is one repo. Branch `main`.

```
https://github.com/USJ-Technologies/USJ-Business-Planning   (private)
```

Author is `Bhanu <bhanu@usjtechnologies.com>`, set locally on the repo. Keep it that way.

The scope site used to be its own repo inside `04-business-scope-site/`. Its 5 commits were
kept — `git log --follow` still tracks files across the move.

**Keep this repo private.** It holds internal strategy, and the salary / role /
responsibility sections are still to be added.

## The scope website (`04-business-scope-site/`)

Single self-contained `index.html`. No build step, no dependencies. Open it in a browser.

Two modes, toggled top-right:
- **Read** — sidebar nav, scroll through
- **Present** — full-screen slides, `←` `→` to move, `Esc` to go back, `P` to enter

23 slides today: Cover → The group → Where we are today → ChaloKumbh (idea, Online Pooja ×4,
Vedanz ×4, Doon Travellers ×4, USJ Stays ×4, One customer five earnings, What ChaloKumbh needs)
→ Coming next.

New sections go in as `<section class="sl" id="s-...">` inside `.wrap`, and get a matching
link in `<nav class="nav">`. Nothing else needs changing — the JS picks up slides automatically.

### Hosting

Deployed to Vercel under the existing account (team `harrys-projects-93f08a21`), project `usj-group`.
`vercel.json` sets `X-Robots-Tag: noindex, nofollow, noarchive` and `robots.txt` disallows everything —
this is an internal document and must stay out of search results.

**Note:** the first deploy went out missing `index.html`. Redeploy from here:

```bash
cd "04-business-scope-site"
npx vercel --prod
```

Or connect the GitHub repo to the Vercel project so it deploys on every push.

> Before this URL is shared beyond sir: it holds internal strategy, and the salary /
> role / responsibility sections are still to be added. Worth deciding who can see it.
