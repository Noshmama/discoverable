# GetDiscoverable.io — How We Do It

The working standard for this site: voice, method, the build checklist, distribution, and
the strategy behind it. If you're writing or publishing anything here — Zillah, a
freelancer, or a future session — follow this. It's the method written down so it doesn't
have to live in someone's head.

---

## 1. Voice

- **Never use "quiet" or "quietly."** Standing rule, no exceptions.
- **Go light on em-dashes.** They read as an AI tell and get stripped.
- **Plain, direct, declarative.** No hype. "Bye bye manual SEO" energy is banned.
- **Never fabricate or overstate.** Every claim is grounded. If the only evidence is
  Zillah's own article, say so — don't inflate it into independent proof. Don't overstate
  her background or experience.
- **Answer-first.** Lead with the plain answer, then explain.

## 2. How a post gets made

- **Ground it in a real, specific source** — a real AI answer, a reader's question, a named
  statistic, a screenshot. Not guesses.
- **The headline is the question a real person types; the first line is the answer.**
- **The "is the answer the same?" test.** Every post must add something the existing posts
  don't. No reruns of a thesis already covered — narrow the angle or add a net-new idea.
- **Titles lead with the benefit in plain language, keyword second.** Never jargon-first.
  (A reader doesn't search "location pages"; they search "wine tasting near me.")

## 3. The build checklist (every post, every time)

- **One `<h1>`, then `<h2>`s.** Never skip a level. Use `<h3>` only as a genuine sub-point
  under an `<h2>`.
- **Answer-first block** near the top (the indigo callout box).
- **Schema:** `BlogPosting` always; add `FAQPage` with the exact questions people search;
  add `HowTo` for step/checklist posts. Validate the JSON before committing.
- **Internal links** into the relevant cluster (related posts, the structured-data explainer,
  the case study, etc.).
- **Machine-readable:** real on-page text, never PDFs or images for facts; structured data;
  one consistent name.
- **Wire every new post into all four:** the blog index (`blog/index.html` — a card *and* the
  `blogPost` JSON-LD array), `sitemap.xml`, `rss.xml`, and `llms.txt`.
- **Request indexing** in Google Search Console after publishing (new URLs especially).

## 4. Distribution

- **LinkedIn:** no link in the body — put the URL in the first comment. Lead with the finding,
  not "excited to announce." Contrarian/debunk posts break through; plain explainers get
  throttled.
- **Punchdown:** a teaser that earns the click, with a tagged link to our own site
  (`?utm_source=punchdown&utm_medium=referral&utm_campaign=<post>`).
- **COLAClear → GetDiscoverable cross-links** carry `utm_campaign=winery-crosslink`.
- **Wine Business is the best backlink shot.** When a byline runs, make sure the bio link
  to getdiscoverable.io stays a live, followable hyperlink.

## 5. The strategy (the north star)

- **The bottleneck is authority** — backlinks and third-party corroboration — not content
  volume or tooling. One real byline beats ten more posts.
- **One page per query.** Differentiate overlapping posts by intent; never let two pages
  compete for the same search, and never internally link two that do.
- **Chase winnable, specific searches** (striking-distance and long-tail), not head terms a
  young domain can't win.
- **The frame is three layers:** SEO (ranking), AEO (the answer box), GEO (being named inside
  an AI answer).
- **The metric that matters is "does the machine name us?"** — not vanity traffic.
- **Ignore the hype cycle.** The model is augmentation, not automation: keep the judgment,
  drop the drudgery. Mass auto-published content is scaled content abuse and gets penalized.

## 6. The two stacks

- **GetDiscoverable.io** → this repo (`/workspace/discoverable`). Push to `main`; Vercel
  auto-deploys. robots.txt already welcomes the AI crawlers (GPTBot, Google-Extended,
  ClaudeBot, PerplexityBot, and more).
- **COLAClear.com** → develop on a branch, open a PR to `master` (don't push to `master`
  directly). Its press page also lists Zillah's bylines and should be kept in sync.

## Definition of done

A post is done when it is: grounded in a real source, answer-first, correctly structured
(one H1, clean hierarchy, valid schema), wired into the index, sitemap, RSS, and llms.txt,
published, submitted for indexing, and has a promo drafted.
