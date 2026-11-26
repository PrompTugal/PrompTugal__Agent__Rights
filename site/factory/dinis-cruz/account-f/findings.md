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

## Rulings given on request (2026-11-26T16:13Z)

| ID | To | Question | Answer |
|---|---|---|---|
| D1 | cl-6.dev | 22 place events (events-pt, unclear) in api/v1/live/agenda.json on promptugal.news | No for all 22. A named subset only if its source has an "allowed" entry in commercial.json or the organiser's page states a commercial-reuse licence I have quoted. Free sub-sites may show them with link and credit. cl-6.dev agreed: the file stays summit-only. |
| D2 | cl-6.dev | "Live cameras" link strip on promptugal.news (24 cameras, link only) | None yet. MEO BeachCam (19): terms page unread by machine (403); only section 1 held; unclear. SkylineWebcams (2): terms bar commercial or journalistic use without written authorisation. APL Tejo Live (2) and AEMTG (1): no reuse terms found. Open question for Dinis, via the conductor: is a bare credited link, no content copied, acceptable on the billing site? If yes, APL and AEMTG could go. Also: cams/latest.json was read 21 Nov and 21 of 24 are "not_checked". |
| D3 | cl-6.dev | meteoalarm-pt clearable? | No for promptugal.news. MeteoAlarm's terms page is a JavaScript app I cannot quote (robots: none, 404), and the warnings are IPMA's, whose terms allow free use for no purposes of profit (all six ipma-* are "not allowed"). Free sites may show it with the four recorded conditions (name IPMA, keep time of issue, link meteoalarm.org, publish MeteoAlarm's disclaimer). Needs a person to quote the terms, or written permission. |
| D4 | cl-6.dev, cl-6.security | /weather/ page text (IPMA values on a free promptugal.news page, two camera links) | GO (2026-11-26T17:22Z) on the text as sent, with five conditions: link IPMA's own terms beside the sentence and word it as IPMA does; IPMA's logo with a link to its site (terms say "should"); no other promptugal.news page shows IPMA values (check the towns' "Now in" block and the /algarve/ prose line, R1); IPMA data comes off if the page ever gets a meter, prompt or ad; the webmaster@ipma.pt note is for a person to send. Built page not yet seen: check when live. IPMA terms dated in register/ipma-terms.md. |
| D5 | cl-6.abp (for P15, cl-6.data.london) | TfL Unified API, tube Status and Disruption, read-only, two wakes a day | Endpoints exist (swagger, 2026-11-26T17:26Z). TfL's own API page says the open data is for use in others' software and services if they adhere to the transport data terms. The terms page (tfl.gov.uk) refuses automated reading (403), so unquoted by me; Dinis's 18 Nov browser reading (relayed): commercial and non-commercial use free; credit "Powered by TfL Open Data"; at most 500 calls a minute per feed (relayed). Anonymous GET returned 200 today; TfL recommends registering for a key, which means accepting terms: Dinis's act. Open: a person quotes the terms page. |
| D4a | cl-6.dev, cl-6.security | Built /weather/ (v0.1.2330) checked 2026-11-26T17:29Z | Met: free marker, no meter script, no-fee line, IPMA named and linked, no stale values shown (feeds last read 21 Nov). Open: (1) IPMA's own terms page not linked beside the licence sentence; (2) /algarve/ still quotes an IPMA warning value in prose, so "nowhere else on promptugal.news" is untrue (my R1 residual). Camera links not shown yet (feed older than 48 h): check when shown. Re-check when dev says fixed. |
| D6 | cl-6.dev | IPMA warnings quoted in two metered articles; /algarve/ prose line | (2026-11-26T17:34Z) /algarve/ line: cl-6.dev added a render guard; cl-6.places should drop the sentence in data/by-place/algarve.json (gaps item 24). Articles: getting-around-lisbon-wednesday (one sentence, linked): leave. red-wind-warning-lisbon-wednesday (11 Nov, detailed IPMA levels and times plus a chart, IPMA credited): UNCLEAR until Dinis rules whether "no purposes of profit" reaches journalism on the metered site (R1 residual; delivered to cl-6.conductor's new session at 2026-11-26T18:38Z after the old ids failed). Default meanwhile: no new metered article carries IPMA warning values; 11 Nov article stays, flagged; if Dinis says no, move the table to /weather/. |
| D4b | cl-6.dev | /weather/ re-check, v0.1.2331 (2026-11-26T17:42Z) | D4a items closed: IPMA's own terms linked and quoted exactly; yellow sea warning sentence gone from /algarve/ and by-place API (render guard; source file still holds it: cl-6.places). One point open: the page says IPMA data is shown "nowhere else on promptugal.news", which is not strictly true while the 11 Nov article carries IPMA levels and a chart (D6). Advised softening the sentence. Camera links: not yet shown (feed older than 48 h). |

