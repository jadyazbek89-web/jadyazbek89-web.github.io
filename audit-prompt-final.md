# Final Recruiter Audit Prompt — Jad Yazbeck Portfolio

Paste everything below this line into a new Claude Code session when you're ready to run the final review.

---

You are a senior agency recruiter in the GCC/MENA region reviewing my portfolio for a Senior Marketing Strategist role. I am Jad Yazbeck. The portfolio is at `C:\Users\User\JadYazbeckPortfolio\index.html` (live at jadyazbek89-web.github.io).

**Goal:** do a final, ruthlessly critical review so I can send this to recruiters with confidence. The objective is to impress recruiters and land interviews.

## How to review

1. Read the full `index.html`. Don't skim.
2. Audit from the perspective of a recruiter who scans portfolios for ~60 seconds before deciding to read or close. Be brutal. Do NOT be nice. I do not need reassurance, I need a job.
3. Flag EVERYTHING that is:
   - Inconsistent (same brand named two different ways, repeated phrases, etc.)
   - Vague or unverifiable (claims a recruiter would mentally challenge)
   - Weak (a "result" that isn't really a result, filler copy, dense paragraphs)
   - Off-tone (defensive, try-hard, or self-congratulatory)
   - Stale or broken (dead JS, missing scrollspy IDs, mismatched alt text, etc.)
4. Group findings as: **CRITICAL** (recruiter red flags) / **MEDIUM** (polish) / **LOW** (optional).
5. For each finding, give: the issue, why it hurts the pitch, and the exact fix (the replacement copy or change). No vague advice.
6. If a section is perfect, say so explicitly. Do not invent improvements.
7. If the entire portfolio is perfect and nothing needs to change, say `PORTFOLIO IS RECRUITER-READY. SHIP IT.` and stop there.

## Rules

- NO em dashes anywhere, including in proposed copy. Use commas, colons, pipes, or middle dots.
- NEVER rotate images. Use `object-position` only.
- Do NOT change anything yet. Present the list first and wait for my approval on each item before editing.
- Preserve facts: I did NOT do paid media on Visit Qatar; "15+" is team size, not brand count; "Multi-year" is not used anywhere.

## Pre-identified findings (start from this baseline, then expand)

These are findings already surfaced in a prior pass. Verify each is still present, refine the proposed fix if you have a better one, then go beyond this list.

### CRITICAL (recruiter red flags)

1. **"Qatar Tourism" vs "Visit Qatar" inconsistency in the hero hook.** Hero hook says "Qatar Tourism's 100M+ reach" but result cards and showcase header use "Visit Qatar." Pick one (recommend Visit Qatar throughout).
2. **Case Study result card #3 is weak.** It just says "Visit Qatar" with label "Account Leadership", which is a brand name, not a result. A real number/duration would land harder (e.g. "Always-on", number of major activations, months on account).
3. **"Engineered, not lucky" and "Engineered, not accidental" appear in two different sections** (Known For card 02 + first YouTube card). Same copywriter tic showing twice. One should change.
4. **Industry Firsts card 03, "YouTube-Recognized Red Carpet Concept" is vague.** A recruiter will think "recognized how?" Either tighten ("Featured by YouTube as a regional initiative") or drop the card.
5. **Industry Firsts card 02 attribution: "Rahma Riad's Account"** reads small/personal next to the other two cards (which cite song titles). Reframe as the campaign/moment, not the account.
6. **Collab proof has 4 photos but project memory only lists 2.** George Wassouf and Rahma Riad photos appear added since memory was written. Confirm they are intended, the files exist on disk, and the crops show faces.

### MEDIUM (polish)

7. **Hero hook is 4 claims chained with commas.** Last claim wins, first 2 blur. Consider a 2-line split, or front-load the strongest claim.
8. **Known For card 03 lists 7 brand names** (FIFA, PSG, UFC, LEGO, ITTF, Meta & YouTube, Charlotte Tilbury). Recruiter brain caps at ~4. Cut to the 3 strongest.
9. **Spotify EQUAL banner: "Managed Rahma Riad's digital presence... to the level where Spotify selected her..."** — "to the level where" is awkward. Replace with a cleaner cause/effect sentence.
10. **Min Awel Dekika YT card subtitle "602M+ Views · International Reach"** — "International Reach" is filler. Either drop or replace with platforms ("Meta · TikTok · Snapchat · YouTube"), which is already in the description.
11. **Case Study Strategy block** uses bold-labeled phrases inside a dense paragraph. Convert to 3 short bullets so a 60-second scanner can absorb it.
12. **Approach card 02: "earned judgment"** is slightly opaque. "Trained instinct" or "experienced calls" reads cleaner.
13. **Avail chip says "Open to Full-Time Opportunities"** but no notice/start date. A recruiter who wants to move fast benefits from a hint ("Available from [month]" or "Immediate").

### LOW (optional / future)

14. **OG image = headshot** (`Jad.jpeg`). For LinkedIn link previews, a composed image with overlay text gets higher click-through. Future enhancement.
15. **Certifications feel light** — 1 Meta Blueprint + 2 LinkedIn Learning. If Google Ads or GAIQ certs exist, list them. If not, leave as is.
16. **`navSections` in JS doesn't include `philosophy`, `known`, `brands`** — scrollspy "active" state doesn't track those sections. Minor bug.
17. **Dead JS: `tlToggle()` function** still exists but the timeline section was removed. Safe to delete.
18. **Form validation uses `alert()`** — works but feels dated. Inline error states are cleaner. Low priority.
19. **PUBG Mobile logo has `.hl` class** (slightly more visible than others). Intentional or leftover? Confirm.
20. **`og:description` vs `twitter:description`** wording differs slightly. Could be unified.

## Deliverable

A numbered, prioritized list with proposed fixes. After I approve item by item (or "all CRITICAL", "all CRITICAL + MEDIUM", etc.), make the edits and push to GitHub.
