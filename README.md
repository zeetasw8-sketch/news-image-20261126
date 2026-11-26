# Thursday 26 November 2026 — World Frontpage

One 1024x1024 PNG that sums up the world's news on Thursday
26 November 2026. A broadsheet front page with a navy masthead,
three hero stories, ten medium cards, a UTC timeline, a world map
with 13 numbered pins, 22 further dated briefs, a DATE CHECK
footer, and a HOW SURE verification legend. In total: 35 dated
stories, spanning 9 regions and 14 fields. Every story carries a
date and a verification label (OFFICIAL / CONFIRMED / REPORTED /
CLAIM), and nothing is stated as fact without a source.

This is an entry for the make.fun competition `news-image-20261126`
($100). It follows the winner's recipe: density of dated stories,
strict date discipline, a verification audit, and a clear
structure.

v3 (26 Nov 2026): corrected the Nvidia close to the verified
$149.30 (−3.91%) — v2's $142.90/−8.03% was the intraday low, not
the close — and removed unverified items (the "65% of deaths age
18–24" chip, "60–70 mph" gusts, "6–7 in snow in St. Louis",
"Charleston tide >8 ft", and the "10 crew hurt" Merkury figure).
The Macy's Parade hero now reports the postponement to Sat 28 Nov.

### v3 accuracy corrections (what changed and why)
- **Nvidia close.** v2 printed "−8.03% to $142.90" as the Tuesday
  close. That was the intraday low, not the close. Five sources
  (Finnhub, MarketBeat, stockanalysis, Fool, Reuters) confirm the
  verified close: **$149.30, −3.91%**. The hero, the timeline, the
  DATE CHECK footer and this section now all use $149.30 / −3.91%.
- **"65% of deaths age 18–24".** v2's Russia hero chip claimed
  65% of 2025 deaths were Russians aged 18–24. That figure was
  never verified, so the chip now reads ">700,000 incl. missing",
  which is the verified Mediazona total.
- **Nor'easter gusts.** v2 printed "60–70 mph". The verified NWS
  figure is gusts **up to 65 mph**, so the hero now reads "65 MPH".
- **St. Louis snow.** v2's chip claimed "6–7 in snow in St.
  Louis". Never verified — removed. The chip now reads "Balloons
  grounded • Rain 1–2 in", both verified.
- **Macy's Parade.** v2 said the parade "steps off" at 08:30 ET
  with "balloons at risk". The parade was **postponed to Sat 28
  Nov** (announced 25 Nov) — the first postponement in 100 years.
  The hero and timeline now report the postponement.
- **Charleston tide.** v2's timeline claimed "Charleston tide
  >8 ft". Never verified — removed from the timeline.
- **Merkury.** v2's brief said "10 crew hurt" (an RT figure).
  The LNA figure is 2 Libyan officers dead, so the brief now
  reads "Libya vows revenge for drone hit on Russian warship"
  (CONFIRMED).

## Hero stories

**Russian military deaths reach 490,334.** Leaked Rosstat death
records, analysed by BBC Russian and Mediazona, put Russian
military deaths at 490,334 from February 2022 to September 2026.
Over 700,000 including the missing. The Kremlin declined
to comment. Sources: BBC Russian, Mediazona, Le Monde, 24-25 Nov
2026. Label: CONFIRMED.

**Nvidia down 3.91% to $149.30.** Nvidia shares closed Tuesday
25 November down 3.91% at $149.30 (verified close; $142.90 was
the intraday low), after a 5.86% fall on Monday.
Trump is open to pardoning CEO Jensen Huang. U.S. markets are
closed on 26 November for Thanksgiving, so there is no newer
price. Sources: Finnhub, NY Post, 25 Nov 2026. Label: CONFIRMED.

**Thanksgiving nor'easter.** A nor'easter peaks on 26 November
with gusts up to 65 mph and 1–2 inches of rain, as the 100th
Macy's Thanksgiving Day Parade is postponed to Saturday 28
November — the first postponement in 100 years. New Jersey
declares an emergency in 21 counties. Sources: NWS/NOAA,
Reuters, 26 Nov 2026. Label: OFFICIAL.

## Medium cards

- A Houthi drone hits a Riyadh tower for the second time; 11
  people hurt (24 Nov, CONFIRMED).
- Huawei is found guilty on 10 of 12 counts in Brooklyn;
  sentencing is set for 14 September 2027 (24 Nov, OFFICIAL).
- Shanghai party chief Chen Jining, 62, is probed by the CCDI
  (24 Nov, OFFICIAL).
- Shenzhou-24 launches: the first Pakistani in orbit, and the
  first foreigner aboard Tiangong (25 Nov, CONFIRMED).
- The Bangladesh garment wage rises 36% to 17,000 taka
  (25 Nov, CONFIRMED).
- U.S. tariffs: India up to 25%, Vietnam 35%, China 20%
  (25 Nov, OFFICIAL).
- Australia CPI is up 4.9% year on year; the RBA rate is 4.85%
  (25 Nov, OFFICIAL).
- Venezuela's debt is $237.5bn, 242% of GDP (24 Nov, OFFICIAL).
- All hostages from the Cartagena supermarket are freed
  (25 Nov, CONFIRMED).
- Vaibhav Sooryavanshi, 15, hits 204 off 53 balls — the fastest
  List A double century (24 Nov, CONFIRMED).

## Dates that did not make it

The ICJ Myanmar ruling was 19 November, not 25 November. The
Hormuz mines are an older event. The Microsoft outage was 12-13
November, not 26 November. There is no Nvidia price for 26
November, because U.S. markets are closed for Thanksgiving.

## The image

The page was rendered with Python and Pillow: flat colours, simple
pictograms, DejaVu type. The result is `entry.png`, 1024x1024,
231,999 bytes, sha256
`69e30d34e3fe011d7e8040a800b4b69ce989820ba54051f13e457d308eea1be5`.
The render is fully deterministic — a fixed palette, fixed fonts,
no randomness, no clock — so repeated runs give byte-identical
output. The render script itself is not part of this entry.

## Run it

`main.ts` needs no network. It validates the bundled PNG (magic
bytes, 1024x1024 dimensions, 1 MiB cap), copies it to
`MAKEFUN_OUTPUT_DIR` (default `/output`), reads the copy back and
verifies it is byte-identical.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
sha256sum out/entry.png entry.png   # both hashes must match
```

## Files

- `main.ts` — the entrypoint; copies and verifies `entry.png`.
- `entry.png` — the front page image (1024x1024).
- `README.md` — this file.
- `LICENSE` — MIT.

## Sources

Reuters, BBC, Mediazona, WSJ, NY Post, NWS/NOAA, Xinhua, USTR,
ABS/RBA, DOJ, CGTN/WHO.
