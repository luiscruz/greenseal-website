# LinkedIn distribution copy: post 3 (Aug 17, 2026)

Source post: `/blog/2026-08-17-implementation-codecs-formats.md`
Canonical URL: https://greenseal.dev/blog/2026-08-17-implementation-codecs-formats/
Status: ready to paste when Luis is ready to post (matches blog-plan status "Ready to publish")

## Post copy

ISO/IEC TS 20125-1:2026 is ISO and IEC's technical specification for building greener digital services, published in February 2026. Most guidance like this stays deliberately generic, so it doesn't need revising every time a new format ships.

TS 20125 breaks that rule exactly once.

One clause names actual codecs: WebP, AVIF, VP9, HEVC, AV1, Opus. Specific compression settings too.

That's unusual for a standard, and it's not there by accident.

We dug into why a document built to stay technology-neutral suddenly gets this specific, and what that means if you're tempted to paste this list into your engineering guidelines as-is.

Full breakdown: https://greenseal.dev/blog/2026-08-17-implementation-codecs-formats/

#GreenSoftware #SustainableSoftwareEngineering #ISO20125 #WebPerformance #SoftwareEngineering

## Notes for Luis

- Rewritten per your feedback that the previous draft was too long and read as a compressed summary rather than a teaser. That version walked through the full codec lists, the "should not shall" distinction, and the "know what's efficient and keep checking" conclusion in sequence, so a reader got the post's payoff without needing to click.
- This version stops after establishing the tension (a standard built to stay technology-neutral breaks that convention exactly once) and naming the codecs, then poses the "why" and "what does this mean for your engineering guidelines" questions without answering either. The resolution (it's a labelled example under a "should," not a requirement, and the real ask is ongoing review, not a fixed codec list) stays in the post. That's the curiosity gap that should drive the click.
- Cut from ~180 words / 7 paragraphs to ~80 words. Short, single-idea lines for feed scanning, no paragraph runs longer than one sentence.
- Link appears once, in its own line near the end, with the full URL spelled out (LinkedIn auto-shortens/cards it, but having the plain URL in the text avoids relying on the card rendering correctly).
- No stats or claims beyond what green-software-expert already reviewed in the post body: no fabricated numbers, no independent claims about codec performance.
- No em dashes or en dashes used anywhere in this copy, per house rules.
- Hashtags unchanged from the previous draft: pulled from the site's existing meta-keywords family (green software, sustainable software engineering) plus two specific to this post's angle (ISO20125, WebPerformance). Kept to five, consistent with typical LinkedIn practice of not over-tagging.
- Revised opening per Luis's feedback that "ISO/IEC TS 20125-1:2026" as a bare designation assumes the reader already knows what it is, which most LinkedIn readers won't. The first sentence now names what it's for in plain language, ISO and IEC's technical specification for building greener digital services, plus the February 2026 publication date, before the "breaks its own rule" hook. Phrasing is pulled from the site's own established language (post 1's "the first ISO/IEC technical specification for digital services ecodesign," which is careful to say "technical specification" and not "International Standard") rather than inventing new framing, so it stays consistent with how GreenSeal describes TS 20125 elsewhere and doesn't overstate it as a certified or third-party-audited standard. Added one clause explaining why standards usually stay generic ("doesn't need revising every time a new format ships") so the "breaks that rule" line lands for someone with zero prior context, then established the "TS 20125" shorthand for the rest of the copy per house style. Net addition is about 20 words; still 97 words total, within the 60-100 word range, and the "should not shall" distinction and "keep checking" conclusion are still held back for the click-through.

## Image crop: flagged, not resolved

The post's header image, `/images/blog/implementation-codecs-formats.jpg`, is 1200x627 (the same ratio the site uses for on-site OG/Twitter cards, roughly 1.91:1).

Post 1 (`requirements-and-end-of-life`) has a second, LinkedIn-specific crop that this post doesn't: `/images/blog/requirements-and-end-of-life-linkedin.jpg` at 1440x1798, a portrait ratio close to LinkedIn's own recommended 4:5 (1080x1350) for single-image feed posts. That crop shows more of the image at a larger size in-feed than a 1.91:1 landscape image does, which is presumably why post 1 got one.

This post doesn't have an equivalent crop yet. If the same treatment applies here, the follow-up would be a portrait crop of the cassette tape artwork, target roughly 1080x1350 (4:5), keeping the "Stay up-to-date" label legible in the tighter frame, saved as `/images/blog/implementation-codecs-formats-linkedin.jpg` to match the post 1 naming convention.

Not generating that image here since image creation for this series has been handled directly in the main conversation rather than by this agent. Flagging it as an open question: confirm whether post 1's portrait crop was a one-off or is meant to be the standing convention going forward, then generate the equivalent crop for this post (and going forward, for post 4 onward) if so.
