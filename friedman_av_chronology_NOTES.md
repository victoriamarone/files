# Friedman A/V Chronology — companion notes

**File:** `friedman_av_chronology.csv` — 55 rows, sorted ascending by `date_iso`.
Columns: `date_iso, date_confidence, title, series, type, length, source, url, notes, watched`.
`watched` is empty throughout — it is yours to tick.

Date confidence breakdown: **9 exact, 23 approx, 23 unknown**.
Two of the 55 rows are deliberate **gap/summary rows**, not individual works
(the Economics Cassette Series, and the undated remainder of the C-SPAN library).
Nothing in this file was invented — where a date, runtime or URL could not be
verified it is blank, or the row is marked `unknown` and the `notes` field says why.

---

## Read this first: the research environment was crippled

This session had **no working page-fetch capability**. Both routes failed:

- `WebFetch` returned `getaddrinfo ENOTFOUND` for **every** host tried
  (`example.com` included) — a DNS failure inside the tool, not a site problem.
- Direct `curl` through the configured egress proxy returned
  `CONNECT tunnel failed, response 403` for **every** host tried:
  `www.hoover.org`, `www.c-span.org`, `americanarchive.org`, `archive.org`,
  `www.nobelprize.org`, `www.freetochoosenetwork.org`,
  `digitalcollections.hoover.org`, `searchworks.stanford.edu`, `oac.cdlib.org`,
  `en.wikipedia.org`, `www.thetvdb.com`.

So the brief's "known obstacle" was much wider than `miltonfriedman.hoover.org`:
**no host was reachable.** Everything below was assembled from web-search result
summaries only — i.e. from search engines' own extracts of those pages, never
from the pages themselves. That is why so many rows are `approx`: the fact was
attested, but the record could not be opened and read field-by-field.

**Practical consequence for you:** the three structured catalogues that would
have carried this file — the AAPB Firing Line catalogue, the C-SPAN person page,
and the Hoover Economics Cassette Series list — are all pages that must be
*paged through*, not searched. They are fine in your own browser. Roughly two
hours of manual transcription from those three pages would roughly triple this
file's row count. Direct links are given in each section below.

---

## Coverage by scope area

| # | Area | Verdict | Rows |
|---|------|---------|------|
| 1 | Free to Choose (1980) | **Good** — complete, dates approx | 10 |
| 2 | Free to Choose (1990) | **Partial** — complete titles, no dates | 5 |
| 3 | Milton Friedman Speaks | **Good on titles, poor on dates** | 15 |
| 4 | Firing Line appearances | **Poor** | 3 |
| 5 | C-SPAN | **Poor** | 2 (1 real + 1 gap row) |
| 6 | Notable one-offs | **Good** | 18 |
| 7 | Economics Cassette Series | **Failed** — 1 gap row for ~206 tapes | 1 |

### 1. Free to Choose (1980) — good
All ten episodes, in order, with the weekly Friday sequence 18 Jan – 21 Mar 1980.
Each row notes the two-part structure (location documentary half, then the studio
discussion/debate half where Friedman takes on a panel of critics).

Marked `approx` because of a genuine source conflict: TheTVDB's aired-order
listing starts the series 18 Jan 1980, while Free To Choose Network's own page
says the programs "first aired January 11, 1980". PBS distributed station by
station, so local air dates really did vary. **Episode order is certain; the
exact calendar dates are not.** If you want this nailed down, the Free To Choose
Network page is the authority to trust over TheTVDB.

### 2. Free to Choose (1990) — partial
All five titles and all five celebrity introducers (Schwarzenegger, Shultz,
Reagan, David Friedman, Steve Allen) are solid. **No air dates exist in any
accessible source.** TVmaze and TheTVDB both show `1990-01-01` for all five,
which is a placeholder; one listing gives 2 Feb 1990 as the series' last air
date. Sources also disagree on the broadcaster — PBS for the series, CNBC for
the newly produced discussion segments. All five are dated `1990-00-00` /
`unknown`, in official episode order.

### 3. Milton Friedman Speaks — good titles, no dates
All **15** lecture titles are confirmed (cross-checked between TheTVDB's series
listing and the Free To Choose Network / Idea Channel catalogue). Lectures 12–15
are catalogued with the year 1978; lectures 1–11 carry **no published year at
all**, so they are dated `1977-00-00` / `unknown` purely to hold series order —
treat that year as a placeholder, not a finding.

**No individual recording date or venue is published anywhere** — not by Free To
Choose Network, not by the Idea Channel listing, not by Hoover's finding aid.
The brief expected these two sources to carry venues; they do not. Audio of the
original lectures is in the Hoover Friedman papers, so the venues may exist on
item-level records inside `miltonfriedman.hoover.org` — worth a look, but I could
not confirm it.

Two 1978 talks are listed **separately** because they are *not* confirmed parts
of this series, despite the overlapping period: the Kansas State Landon Lecture
(27 Apr 1978) and "Capitalism and the Jews" at the University of Chicago Law
School. Do not merge them without checking.

### 4. Firing Line — poor (biggest gap after the cassettes)
Only **three** rows: "The Economic Crisis" (8 Jan 1968, episode 83 / Hoover
S0083) and both parts of the privatization debate (2 May 1986, Hoover S0688).

Hoover's Collected Works site reportedly shows **5 Firing Line records** for
Friedman, and IMDb spans his appearances **1968–1990**, so at least two and
probably several more episodes exist that are not in this file. Hoover's DVD
release notes mention him among guests on "thirty additional programs."

The AAPB Firing Line collection (1,505 episode-level records, 1971–1999; 396
with digitised video, the rest transcript-only) has exactly the structured
per-episode records with guest lists that this task needed — and its catalogue
search was the single most valuable thing I could not reach. Records use `S`
numbers (e.g. `S0111; The Nixon Presidency`, 1973-09-28).

**Do this by hand:** search `https://americanarchive.org/catalog` for
`Milton Friedman` restricted to the Firing Line collection
(`https://americanarchive.org/special_collections/firing-line`), and cross-check
Hoover's collection page (`https://www.hoover.org/library-archives/collections/firing-line`).
Every AAPB record carries a broadcast date and a guest list.

### 5. C-SPAN — poor
Only one dated C-SPAN item made it in: the Booknotes interview on Friedman's
introduction to the 50th-anniversary *Road to Serfdom* (20 Nov 1994, `approx` —
the date comes from the transcript header as quoted in a 1997 mailing-list post
and corroborated by Cafe Hayek; C-SPAN's own transcript URL no longer resolves).

A **gap row dated 1991-00-00** stands in for the rest. Note a correction to the
brief: C-SPAN's Friedman person page states **17 videos**, not ~26, with the
first appearance a **1991 speech**; most frequent co-appearers Brian Lamb (3) and
Rose Friedman (2). Items glimpsed but not dateable: an *In Depth* episode
(program id 171801), a 2006 American Legislative Exchange Council speech, a 2002
Cato Institute tribute, and a "Milton & Rose Friedman" school-choice interview
with Brian Lamb.

**Do this by hand:** `https://www.c-span.org/person/?20878%2FMiltonFriedman=`
lists all 17 with an exact air date on every row. This is the **highest
value-per-minute** manual fix in the whole file — one page, 17 exact dates.

Separately, C-SPAN2 reran the 1980 *Free to Choose* episodes in Feb–Mar and Aug
2024. Those are rebroadcasts, so per the dedup rule they are mentioned in the
1980 episode notes rather than given rows of their own.

### 6. Notable one-offs — good
This is where the session paid off. Verified and dated:

- **Nobel lecture** "Inflation and Unemployment", 13 Dec 1976 — included as a
  `text` anchor as instructed; nobelprize.org has text and PDF, no video.
  (Watch for bibliographic records dating it 1977 — that is the volume's
  publication year.)
- **Uncommon Knowledge with Peter Robinson — six episodes**, better than hoped:
  *Take It to the Limits: Milton Friedman on Libertarianism* and
  *Presidential Report Card: Milton Friedman on the State of the Union*, both
  "Recorded on Wednesday, February 10, 1999" (two shows in one taping session, as
  was normal); *Milton's Paradise Gained* (2000-03-10); *The Economy's New
  Clothes* (2000-03-20); *The High and the Mighty: The War on Drugs*
  (2000-12-13); *Economics and War*, on the economic effects of 9/11
  (2001-09-25). The four later dates come from the `Date Created` field of
  Hoover's Collected Works item listing and are marked `approx`, because
  Date Created can be the broadcast or cataloguing date rather than the taping —
  the `Recorded on` line on each hoover.org page is the one to trust.
  Beware: Hoover's archive also shows 1999-05-15 / 1999-05-22 for the 1999
  episodes; those are broadcast dates, not the 10 Feb taping.
- **"The Power of Choice: The Life and Ideas of Milton Friedman"** — PBS,
  **Monday 29 January 2007, 10:00–11:30 p.m. ET, 90 min**, narrated by David
  Ogden Stiers. The firmest `exact` row in the file (from PBS press materials,
  which also note 29 Jan 2007 was declared Milton Friedman Day).
- **"Economic Freedom, Human Freedom, Political Freedom"**, Smith Center lecture,
  Cal State Hayward, **1 Nov 1991**, introduced by Charles W. Baird — confirmed
  by the Smith Center's own past-events page. Do not confuse it with a 2002
  address circulating under the same title.
- **Landon Lecture**, Kansas State University, **27 Apr 1978** (audio archived by
  K-State).
- **Firing Line 1968 and 1986** (see area 4).
- **Hoover audio bookends:** the 1961 debate with Senator Joseph Clark — the
  *oldest* recording among the 250+ digitised audiotapes in his papers — and
  "Vouching for Vouchers" (1997), the *most recent*. Year only for both.
- **PBS *Think Tank* #629, "The Commanding Heights"** (orig. aired 7/16/1998) —
  Ben Wattenberg with Daniel Yergin and Friedman from San Francisco, Galbraith
  later in the program. This is a **different item** from the one below.

Included but weak, flagged as such:

- **Donahue, the "greed" exchange** — `1979-00-00` / `unknown`, **URL left
  blank**. The year 1979 is agreed by several secondary sources, but there is no
  exact air date, no episode number, and no archival host. It survives only as
  YouTube reuploads with no canonical link, so I would not point you at one.
  Friedman appeared on Donahue more than once; the later appearances are
  referenced but entirely undated.
- **Commanding Heights production interview (2000)** — `2000-00-00` / `unknown`.
  PBS/WGBH shot "more than 150 on-camera interviews" and Friedman is among the
  listed interviewees with his own Interview link and an excerpts page (Mont
  Pelerin Society, Pinochet's Chile). **The brief's suggested 1 Oct 2000 could
  not be verified** — the transcript page itself was unreachable. The real date
  is in that page's header; check it in a browser and upgrade the row.
- **RÚV (Icelandic State Television), 1984** — year only. A crosstalk hosted by
  Bogi Ágústsson. No RÚV archive record found; the URL is the blog post that
  hosts the video, not an archive. A companion University of Iceland lecture is
  often mentioned but could not be dated.

Two further `text` anchors were added because they date the intellectual
turning points the recordings orbit: the **AEA Presidential Address "The Role of
Monetary Policy"** (Washington D.C., 29 Dec 1967; *AER* March 1968) and the
**Friedman–Heller debate "Monetary vs. Fiscal Policy"** (Seventh Arthur K.
Salomon Lecture, NYU, 14 Nov 1968). The latter overflowed its room and had
closed-circuit TV in adjoining classrooms, so a recording may well exist — none
is online. The book is fully digitised at FRASER.

**Deliberately excluded, and why:** a Charlie Rose Friedman interview. Hoover's
inventory references Charlie Rose items from 1999 and 2005, but the only 2005
Charlie Rose episode I could find was a rebroadcast with **Thomas** L. Friedman.
Rather than risk conflating the two Friedmans, I left it out — worth a look in
Hoover's inventory if you want it. The famous "The Social Responsibility of
Business Is to Increase Its Profits" (*NYT Magazine*, 1970) was also left out: I
could not verify its date in this session and chose omission over a remembered
date.

### 7. Economics Cassette Series — failed
**This is the biggest remaining gap by an order of magnitude: ~206 rows missing.**

One summary row is in the file, dated `1969-00-00`, per the brief's instruction.
What is established: a biweekly subscription audio commentary tied to Friedman's
*Newsweek* columns, produced by Instructional Dynamics Inc. (Chicago), 1969–1978,
ended when IDI hit financial trouble. Usual interviewer **William Clark** of the
*Chicago Tribune*; **Rose Friedman** interviewed during a six-month Vermont stay;
**Paul Samuelson** substituted for Friedman on a few programs. Hoover holds
**206 of the 215-cassette set**, "apparently the definitive collection."

Why it failed: no comprehensive list existed in the Friedman papers, so **Hoover
staff compiled one from the cassette labels** — topics, plus dates and
contributor names *where known*. That list is a document **in box 103** of the
Milton Friedman papers, announced at
`https://www.hoover.org/news/new-list-206-tapes-milton-friedmans-economics-cassette-series`.
It is not a web page that search engines expose, and with no fetch capability it
was unreachable. Also note: **most cassettes are still undigitised** — Hoover
digitises on researcher request — so even a complete list would not give you 206
things to listen to today.

Minor conflict to be aware of: a Carnegie Mellon library catalogue dates the
series 1969–1975; Hoover says 1969–78, and Hoover is describing its own holdings.

**Do this by hand:** open that Hoover announcement, follow it to the box 103
finding-aid entry, and transcribe. Even dates-only would make this the most
valuable part of the file, exactly as the brief anticipated.

---

## Which sources were productive

**Productive** (via search extracts): Hoover's main `www.hoover.org` news and
research pages — the `Recorded on …` line on Uncommon Knowledge pages is
gold-standard and gave 6 dated rows; PBS press materials (gave the single
firmest date in the file); institutional event pages that keep their own
history, i.e. the CSU East Bay Smith Center past-events page, the K-State Landon
Lecture page, the UChicago Law School recordings page; Free To Choose Network for
titles and series structure; nobelprize.org; FRASER.

**Unproductive, purely because they could not be opened:** AAPB's Firing Line
catalogue, the C-SPAN person page and Video Library, the Hoover Economics
Cassette Series list, the OAC/`oac.cdlib.org` finding aids,
`miltonfriedman.hoover.org`, `digitalcollections.hoover.org`. These are the
right sources — the brief had them correct — they just need a browser.

**Treat with caution:** TheTVDB and TVmaze. TheTVDB supplied the 1980 weekly
sequence and the 1986 Firing Line date and looks internally consistent, but it
is fan-maintained and conflicts with Free To Choose Network on the 1980 start
date. TVmaze's 1990 dates are placeholders. Every row relying on either is
marked `approx` or `unknown`.

---

## Where you will have to fill gaps by hand, in priority order

1. **C-SPAN person page** — `https://www.c-span.org/person/?20878%2FMiltonFriedman=`
   → 17 exact air dates from one page. Best effort-to-reward ratio here. Then
   delete the 1991-00-00 gap row.
2. **Economics Cassette Series, box 103** → up to ~206 rows. Biggest absolute
   gain, biggest effort, and note most tapes are undigitised.
3. **AAPB Firing Line catalogue**, search `Milton Friedman` → probably 2–5 more
   episodes with exact broadcast dates and guest lists; also lets you confirm
   whether Hoover's "5 Friedman records" matches.
4. **Commanding Heights interview transcript header** → upgrades that row from
   `unknown` to exact. One page, one date.
5. **Free to Choose Network 1980 page** → settle the 11 vs 18 Jan 1980 start and
   promote ten `approx` rows to `exact`.
6. **Hoover item-level records for Milton Friedman Speaks** → the per-lecture
   venues and recording dates, if they exist anywhere, are there.
7. **Free to Choose 1990 air dates** → may only be recoverable from PBS station
   archives or 1990 newspaper TV listings. Low odds.

A tip on sorting: `date_iso` is always populated, so the file sorts cleanly as
text. Rows sharing a `YYYY-00-00` or `YYYY-MM-00` value are left in deliberate
series/episode order, so a stable sort preserves watch order — use a stable
sort, or add a tiebreaker column, if you re-sort in a spreadsheet.
