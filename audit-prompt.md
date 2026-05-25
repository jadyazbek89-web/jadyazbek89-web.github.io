# Final Portfolio Audit Prompt

> Copy-paste the block below into a fresh Claude Code session when you're ready for the full finalization pass.
> Recommended model: Claude Opus 4.7.

---

You are picking up work on the Jad Yazbeck Portfolio project at C:\Users\User\JadYazbeckPortfolio\.

STEP 0 — LOAD CONTEXT BEFORE DOING ANYTHING
1. Read CLAUDE.md in full (all session logs, master pending list, decisions made).
2. Read the memory index at ~/.claude/projects/C--Users-User-JadYazbeckPortfolio/memory/MEMORY.md and every memory file it points to.
3. Confirm back to me, in 3-4 lines, what you understand about the project status, the design system, and the standing rules (no em dashes, no image rotation, do the work independently, end-routine logging).

THE MISSION
I am job-hunting. My target employers are MARKETING AGENCIES in the GCC (Dubai, Abu Dhabi, Riyadh, Doha, Kuwait) and in Lebanon (Beirut). Not in-house brand teams — agencies. This distinction matters because agencies hire differently: they care about creative range, breadth of clients, executional depth, and whether you can walk into a pitch room. Calibrate the entire audit to that audience.

The goal of this session is to FINALIZE THIS PORTFOLIO ONCE AND FOR ALL so that the moment an agency recruiter or creative director opens it, they immediately want to interview me.

STEP 1 — FULL CRITICAL AUDIT (BE BRUTAL)
Put yourself in the chair of an agency Head of Talent or Creative Director in Dubai or Beirut who opens 40 portfolios a week. They will spend 30-60 seconds on the first scan. They are looking for reasons to CLOSE THE TAB. Your job is to find those reasons before they do.

Audit across these dimensions and write findings to a temp file you can reference (you can delete it at the end):

A. ABOVE-THE-FOLD IMPACT (first 5 seconds)
   - Does the hook punch hard enough?
   - Is the headline scannable in one breath?
   - Does the photo + name + title combo feel senior, or junior?
   - CTAs: are they where the eye lands?

B. COPY & LANGUAGE
   - Every line: is it specific or generic? Kill anything generic.
   - Tone: confident without being arrogant. Agency-appropriate.
   - Typos, awkward phrasing, redundancy, weak verbs.
   - No em dashes anywhere (project rule).
   - No "Arab music industry" framing in body prose (project rule).
   - "And" stranding at line ends — check on desktop + mobile.

C. STRUCTURE & FLOW
   - Section order: does it tell a story? Hook → proof → depth → personality → contact?
   - Section count: is anything dead weight? If a section doesn't earn its place, cut or merge it.
   - Length: a recruiter scroll-fatigues fast. If the portfolio is too long, CONDENSE — but preserve the strongest proof points. Density of signal must go UP, not down.

D. PROOF & CREDIBILITY
   - Brands strip: ordered for max impact?
   - Industry Firsts: framed as undeniable claims?
   - Case study (Visit Qatar): does Challenge → Strategy → Execution → Results actually land, or does it read like filler?
   - Showcase grids: are the strongest cards in the strongest positions?

E. VISUAL EXECUTION
   - Run Playwright (the MCP is installed) and screenshot:
     * Desktop 1440px — full page + every section
     * Tablet 768px — full page + every section
     * Mobile 375px — full page + every section
   - Check: thumbnail crops, alignment, hover states (where you can), button spacing, type hierarchy, color contrast, padding/rhythm.
   - Confirm no layout breaks, no overlap, no orphan words, no broken images, no lazy-load surprises.

F. INTERACTION & POLISH
   - Custom cursor still working on desktop?
   - Rotating headline cadence still feels right?
   - Scroll reveals firing in the right order?
   - Counters animating cleanly?
   - Loader timing?

G. AGENCY-SPECIFIC SIGNALS
   - Does the portfolio show CREATIVE EXECUTION, not just strategy slides?
   - Is there enough VISUAL CRAFT for a creative director to respect it?
   - Are big-name brands and recognizable IP front and center? (PUBG, FIFA, PSG, Visit Qatar, Charlotte Tilbury)
   - Is the "I can walk into a pitch room tomorrow" energy coming through?

H. TECHNICAL / META
   - <title>, meta description, OG image, Twitter card — all clean and recruiter-friendly?
   - Mobile tap targets ≥ 44px?
   - Resume link works (Jad Yazbeck Resume.pdf with the space — keep download attr).
   - Email/phone tap-to-call works.
   - No console errors when the page loads.

I. THE "WHAT'S MISSING" CHECK
   - Is there anything an agency hiring manager would WANT to see that isn't there?
   - Examples to consider (not prescriptions): a one-line value prop near the top, a "selected clients" list with logos if logos are clean enough, a "what I do in a 90-day onboard" line, a clearer separation between Strategy work and Creative work, language fluency (English/Arabic/French) made visible somewhere.

STEP 2 — PRESENT FINDINGS, THEN EXECUTE
After the audit:
1. Show me a short, prioritized punch list: CRITICAL → HIGH → MEDIUM → POLISH.
2. Show me any proposed CONDENSING moves with before/after line counts or section counts, and confirm what's being preserved.
3. DO THE WORK. Don't ask me for permission on items inside the audit scope — per the "do the work" rule, take initiative. The only things to surface for my decision are:
   - Anything that changes positioning (e.g., adding/removing a section)
   - Anything that requires content I haven't given you (numbers, quotes, brand names not already in the file)
   - Anything where two strong options exist and a coin flip would decide

STEP 3 — CONDENSE CAREFULLY
If you condense, the rule is:
- Cut redundancy, not signal.
- Preserve all proof points: Industry Firsts, 602M+, 100M+, brand names, PSG collab callouts, EQUAL banner, collab photos.
- When you remove copy, retune surrounding spacing, type sizes, and reveal timing so the layout doesn't end up airy and hollow. The page should feel TIGHTER, not THINNER.
- Don't break responsive behavior — re-test at 1440 / 768 / 375 after every condensing pass.

STEP 4 — CONSTRAINTS YOU MUST RESPECT
- NO em dashes anywhere on the site. Use commas, colons, pipes, or middle dots (·).
- NEVER rotate images. Use object-position only.
- Keep all design tokens (--black, --teal, --purple, --white) untouched unless I approve.
- Preserve the file structure: one HTML file, inline <style> and <script>.
- Don't delete index_v1_backup.html.
- Don't create new files unless absolutely necessary.

STEP 5 — VERIFY BEFORE CLAIMING DONE
- Re-screenshot every section at the 3 viewports after edits.
- Diff the audit punch list against what was actually shipped.
- Confirm the live site (GitHub Pages: jadyazbek89-web.github.io) reflects the changes after push.
- Then and only then report "done" — and report it with evidence, not assertion.

STEP 6 — COMMIT AND PUSH
- Commit in small, logical chunks with clean messages (not one giant "audit" commit).
- Push to GitHub Pages after each meaningful chunk so I can preview as you work.

STEP 7 — END-ROUTINE
When the audit and edits are complete:
- Append a new Session Log entry to CLAUDE.md covering everything done.
- Update the Master Pending List.
- Update memory if any new permanent rules came up.
- Output the final pending list (should be empty or nearly so).

OUTPUT STYLE
- Be terse in chat — I want progress, not narration.
- Show me screenshots when they actually change my understanding of something.
- Use Playwright proactively. Don't ask if you should screenshot — just do it.
- If you find something that genuinely needs my call, ask in one line, give me your recommendation, and wait.

THE BAR
The bar is not "good portfolio." The bar is: a creative director in Dubai opens this on their phone between meetings, scrolls once, and DMs me on LinkedIn the same day. Everything in this audit should serve that single outcome.

Begin with STEP 0.
