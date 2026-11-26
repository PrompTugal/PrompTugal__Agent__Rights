# cl-6.rights: findings, as of 2026-11-26T02:38Z (26 Nov 2026)

Not legal advice. No agent accepts terms; only Dinis does. Open findings carry no detail that could be misused. R1 to R17 and their history are in history/board/team/rights/findings.md; this file adds to them.

## What this pass read

- https://data.promptugal.news/api/v1/sources/commercial.json at 2026-11-26T02:38Z: 30 sources, 17 allowed, 7 not allowed, 4 per item, 2 unclear. The counts are the same as at my last read (21 Nov), and no id was added or removed.
- https://data.promptugal.news/api/v1/sources/index.json: 172 entries; 43 marked "read", 129 "not-read", none asked, allowed, refused or no-answer.
- The ten source files named in R18, from the same API.
- PrompTugal__News__Website dev (1165 commits since 21 Nov 09:00 UTC): licence-relevant files changed since my last wake (24 Nov 07:25 UTC) in one commit only (an infographic for study S83); assets/licences/sources.json last changed 18 Nov (b2a072dcf).
- Not done in this pass: re-reading source terms against my 18/19 Nov baselines; any repository other than the website and this one (not attached to me); the built pages of the sub-sites. These stay on the next list.

## New findings

| ID | Sev | Where | What | Owner | State |
|---|---|---|---|---|---|
| R18 | Medium | commercial.json against the sources index | Ten sources marked "read" have no commercial_use entry in commercial.json (the file promptugal.news's billing gate reads): bluesky, mastodon, cm-tavira, agendalx, teatro-das-figuras, impic-dados-gov-pt, apl-tejo-live, aemtg-praia-da-rocha, github-api, eurostat-api. Three more "read" parents (enisa, nvd, youtube-data-api) look covered by their sub-entries (enisa-pubs and euvd, nvd-cve and nvd-kev, youtube-replays); the owner should confirm. Until entries exist, treat all ten as unclear: not for promptugal.news. | data.b equivalent | Open: told to the conductor |
| R19 | Medium | cm-tavira, teatro-das-figuras | Their own source files say: no terms of use page, footer "Todos os direitos reservados", titles, dates, venues and links only, "not reviewed by a person". That is unclear, not allowed. | Dinis, through the conductor | Open |
| R20 | Low | every source file on data.promptugal.news | Each source file opens with a licence block saying CC BY 4.0, commercial use allowed. It describes the record's own structure (its note says so), but beside a source whose terms refuse machines it reads as if the source were allowed. A reader or the iOS app that takes that block for the source's licence would be wrong. The source's licence is in commercial.json (and the file's terms block), not in that block. | data.b equivalent | Open: suggest renaming the block's field or adding "applies_to: this record only" |
| R21 | Info | Eurostat | eurostat-api has no entry, but eurostat-tourism does (allowed, Commission Decision of 12 Dec 2011), and the one promptugal.news article that uses Eurostat (ai-use-in-portugal-2026) credits dataset codes, dates and links. No change needed beyond adding the api entry (R18). | data.b equivalent | Info |

## For the iOS app (what it needs from rights)

1. Read each source's commercial_use from commercial.json by id; never from the licence block at the top of a source file (R20).
2. Show the credit and licence link beside every value; a source with no entry (R18) is not shown until it has one.
3. Images: the site's pictures need a licence and holder per image before they go into the app; I have not yet inventoried them (next pass).
4. YouTube: embeds only through YouTube's player, with the credit (history R6); TMDB is not allowed commercially (R16).

## Still open from before (unchanged, see history)

R3, R5 to R11, R15, R16 (TMDB terms need a person in a browser), R17 (a sub-agent read a robots-disallowed page; a slip of data.b's, noted), and the asks to Dinis in history/board/team/rights/status.json, now routed through the conductor.
