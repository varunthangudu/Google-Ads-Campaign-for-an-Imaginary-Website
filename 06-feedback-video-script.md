# Feedback video script

**Target length:** 4–5 minutes. **Format:** screen recording with voiceover.

The submission form asks for a video "explaining your experience and learnings" — so
this is not a feature tour. Roughly a third of it should be about what went wrong and
what you would do differently, because that is the part that shows you understand the
work rather than just completed it.

---

## Setup before recording

Open these tabs in order so you can move through them without hunting:

1. The deployed landing page
2. The deployed page again, with `?utm_source=google&utm_medium=cpc&utm_campaign=BLR_Search_DeepCleaning&utm_term=home+deep+cleaning+bangalore&utm_content=ad_variant_a` appended
3. The GitHub repository
4. `docs/02-keyword-research-and-forecast.xlsx`, on the Budget & Forecast sheet
5. `docs/03-ad-copy-bank.md`
6. Google Ads, on the campaign overview *(if you built it in the interface)*

Record in 1080p. Use headphones with a mic rather than laptop speakers — audio quality
affects how the work is judged more than people expect.

---

## 0:00 — 0:30 · Open with the problem, not your name

> "This is a Google Ads campaign for SparkleNest, a residential deep-cleaning service
> in Bengaluru. SparkleNest is fictional — the brief allowed an imaginary website, so I
> invented the business. But I built the website for real and deployed it, because a
> campaign without a working landing page can't demonstrate message match or conversion
> tracking, and those are most of what running Google Ads actually is."

Say it plainly. Do not open with "Hello everyone, my name is…" — start with the work.

## 0:30 — 1:15 · Why this business, and why Search

Show the landing page.

Cover:
- Chose a **local service** business because the demand already exists as search
  queries. Nobody discovers they need their bathroom descaled from a banner ad.
- Conversion is a **lead**, not a purchase, so tracking can be shown without a payment
  gateway.
- Chose **Search** as the primary campaign type and can defend rejecting Performance
  Max: at roughly 130 leads a month, PMax has too little conversion data to learn from,
  and it hides the search-term report that this project is meant to teach you to read.

## 1:15 — 2:15 · Structure and keywords

Switch to the spreadsheet.

Cover:
- 26 keywords in **four tightly themed ad groups**, so each ad can match its keywords
  closely — a broad ad group is the usual cause of a low Quality Score.
- **Phrase match as the default, not broad.** On a ₹1,000 daily budget, one bad
  broad-match interpretation can eat a meaningful share of the day before anyone
  notices.
- **36 negative keywords loaded before launch**, not after. Point at the grouping:
  job seekers, DIY researchers, product buyers, out-of-area cities.
- Budget weighted **by intent, not by search volume**. AG4 has the smallest volume and
  the highest value per lead.

## 2:15 — 3:00 · Show the tracking working

This is the strongest 45 seconds in the video. Switch to tab 2, the URL with UTM
parameters.

> "This is the landing page as a real ad click would deliver it — campaign, keyword and
> creative all in the URL. The page reads those, stores them, and writes them into
> hidden fields on the form."

Fill the form. Submit. Land on the confirmation page.

> "And here they are on the confirmation page: source, campaign, the exact search term,
> the creative. In a real build this goes to the CRM instead of being displayed. It's
> visible here so you can verify the tracking actually works rather than take my word
> for it."

Then be straight about the limit:

> "The conversion IDs are placeholders, so the tags fire into nothing. The event logic
> is real and verifiable in the console; the delivery to Google Ads isn't."

## 3:00 — 3:40 · What went wrong

Do not skip this. Pick two or three real ones:

- **Character limits.** Wrote the ad copy first and hit the 30-character headline
  ceiling repeatedly. Wrote a script that validates every asset — it caught a display
  path at 16 characters against a 15-character limit that would have been rejected at
  upload.
- **Almost shipped two default settings that waste money.** Display Network expansion
  is on by default in a Search campaign, and location targeting defaults to *Presence
  or interest*, which serves ads to anyone anywhere researching Bengaluru.
- **Conversion value.** First set it to the ₹3,500 order value. That is wrong: only
  ~35% of leads become jobs, so the true expected value is ₹1,225. Feeding the headline
  figure would have made a value-based bid strategy overbid by nearly 3x.
- **Chose Manual CPC over Smart Bidding at launch,** which felt like the less impressive
  answer. But automated bidding needs ~30 conversions before it optimises rather than
  guesses, and there was no conversion history at all on day one.

## 3:40 — 4:30 · What you learned

Two or three real ones, specific enough that they could not be said about any project:

- **Most of Google Ads is subtraction.** The negative keyword list and the excluded
  settings shaped the campaign more than the keyword list did.
- **The landing page is part of the ad.** Quality Score, cost per click and conversion
  rate all move with it. Separating "the campaign" from "the website" is a false split.
- **Cost per lead is a vanity metric on its own.** A campaign can hit its CPL target and
  still lose money if the leads don't close. Cost per booked job is the number the
  business pays its bills with.

## 4:30 — 5:00 · Close

> "Everything is in the repository — the proposal, the keyword workbook with a
> formula-driven forecast, 60 validated ad headlines, seven display creatives, and the
> deployed page. The campaign was built and reviewed but never served live traffic, so
> every performance figure is a forecast and labelled as one. Thanks for watching."

---

## Recording notes

- **Do not read this script word for word.** Talk from the bullets. Slightly imperfect
  and natural beats fluent and robotic.
- Cursor movement should be slow and deliberate; fast scrolling is unwatchable.
- One take is fine. Re-record only if a section is genuinely unclear.
- Upload to **YouTube as Unlisted** (not Private — reviewers cannot open Private links)
  or Google Drive with link sharing set to *Anyone with the link*. Test the link in an
  incognito window before submitting.
