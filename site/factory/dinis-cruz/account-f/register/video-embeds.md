# Embedding YouTube and Instagram videos on a news site: rights ruling

Asked by cl-6.conductor for Dinis's videos section (AI and tech videos per region, official embed players, "no-origin iframes"). Read at source 2026-11-28T16:11:37Z. Not legal advice. No agent accepts terms (R13): embedding by iframe needs no account, and nothing here accepts a term for Dinis.

## Short answer

| | YouTube | Instagram |
|---|---|---|
| Ruling | READ OK to embed through the official player, with the conditions below | NEEDS DINIS: not cleared by me; Meta's own terms refuse my reading |
| Credit | Name the channel and link the video on YouTube, beside the player | Same, beside the embed |
| Per-item check | Yes: the owner may block embedding | Yes: public posts only, and the account must have Embeds on |

## YouTube (read: youtube.com terms of service; developers.google.com YouTube required minimum functionality and IFrame player reference; robots allow the pages)

- Allowed: the terms say "You may also show YouTube videos through the embeddable YouTube player." The terms also say users grant others a licence to use content "only as enabled by a feature of the Service (such as video playback or embeds)". So an embed through the official player is within what YouTube lets any site do. I found no ban on a commercial or news site in the sentences I read; I did not read the whole terms page, and a clause I missed is possible.
- "No-origin iframes" cannot be done as the words suggest. YouTube's required minimum functionality says API clients using the embedded player "must provide identification through the HTTP Referer request header" and must not set a Referrer-Policy "in a way that suppresses the Referer value"; it recommends "strict-origin-when-cross-origin". The IFrame reference lists error 153: "The request does not include the HTTP Referer header or equivalent API Client identification." So an iframe with referrerpolicy="no-referrer" breaks the rule and the player may refuse to play. Use strict-origin-when-cross-origin. A sandbox attribute is a separate question for cl-6.dev and cl-6.security; it does not by itself touch these terms.
- Do not change or cover the player; do not copy the video, its thumbnail or its text out of the player. Link, embed, nothing else.
- Per item: the owner may disallow embedding (the reference lists error 101 and 150: "The owner of the requested video does not allow it to be played in embedded players"). Check each video plays embedded before listing it, and remove it when it stops.
- Credit line (our choice, not found as a YouTube requirement): "Video: <title>, <channel>, on YouTube" with the title linked to the video's own YouTube page, and the date listed.
- Privacy is not a rights question but matters: the player talks to Google when the page loads. The privacy-enhanced domain (youtube-nocookie.com) is not something I read; cl-6.security decides, and the page must not identify readers (the observability rule).

## Instagram

- Meta's pages that hold Instagram's own terms and help text (instagram.com, help.instagram.com) refuse Claude in robots.txt (ClaudeBot disallowed; instagram.com disallows every agent). Not read, not worked round (R13).
- One slip to record: I requested instagram.com/legal/terms and one help.instagram.com page before checking their robots files in this run. I did not read or use what came back and deleted it. A rule bend, logged in my status exceptions.
- What I could read: Meta's developer documentation (developers.facebook.com, robots allow). It says the Instagram oEmbed endpoint "is only meant to be used for embedding Instagram content in websites and apps"; that "Posts on private, inactive, and age-restricted Instagram accounts are not supported"; and that "Accounts that have disabled Embeds are not supported". The endpoint is on graph.facebook.com and needs a Meta app and token, which means accepting Meta's platform terms: Dinis's act, not an agent's.
- So the document supports embedding public posts through Instagram's own embed code, one by one. It does not tell me the terms on a commercial news site, on credit or on ads; I could not read them. Until a person reads Meta's terms in a browser and Dinis says yes, Instagram is not cleared.
- If cleared: use Instagram's own embed code unaltered; only public posts with Embeds on; credit "Post by <account>, on Instagram" linked to the post; re-check each post; remove it when it goes private or Embeds are turned off.
- Privacy: Instagram's embed loads a Meta script and tracks. cl-6.security to rule before any build.

## Both: choose what to embed

- Prefer official channels of organisations, events and publications. No video where a private person, a child or someone's home is the subject, and never name a private person.
- Nothing from a billed page that shows ads we do not control without Dinis knowing: his own MEO reason ("their side is riddle with adds") applies to YouTube's player ads too; he decides.
- Each listed video needs a record: URL, channel, date listed, embed check passed (date), by whom. I will check a sample at each wake.

## One line Dinis needs

"YouTube embeds through the official player are fine on promptugal.news with a link and the channel named; Instagram waits until Meta's terms are read."
