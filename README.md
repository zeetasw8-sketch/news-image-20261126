[![make.fun · news-image-20261126](https://make.fun/badge/news-image-20261126.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![rank](https://make.fun/badge/news-image-20261126/zeetasw8-sketch/news-image-20261126/rank.svg)](https://make.fun/bounty/news-image-20261126/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![reward](https://make.fun/badge/news-image-20261126/zeetasw8-sketch/news-image-20261126/reward.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)

# The World Today — 26 November 2026 in one image

Entry for make.fun competition `news-image-20261126` ($100).
One 1024×1024 PNG that sums up Thursday 26 November 2026's world
news — a navy broadsheet masthead, three big heroes, ten medium
cards, a UTC timeline strip, a world map with 13 numbered pins,
22 more dated briefs, a DATE CHECK footer, and a HOW SURE
verification legend — 35 dated stories across 9 regions and
14 fields in total. Built on the winner's recipe from
news-image-20261123 (density + date discipline + audit + structure):
every story carries a date and a verification label
(OFFICIAL / CONFIRMED / REPORTED / CLAIM), and nothing is presented
as a fact without a source.

## The 3 heroes

### Hero 1 — 490,334 Russian Troops Dead
Leaked Rosstat death records, analysed by BBC Russian and
Mediazona, put Russian military deaths at 490,334 from February
2022 to September 2026 — over 700,000 including the missing.
65% of deaths among Russians aged 18–24 in 2025 were caused by
the war. The Kremlin declined to comment on the leaked figures.
Sources: BBC Russian, Mediazona, Le Monde, 24–25 Nov 2026.
Label: CONFIRMED.

### Hero 2 — Nvidia Falls Again: −8.03%
Nvidia shares close Tuesday 25 November down 8.03% at $142.90,
after falling 5.86% on Monday — most of Friday's record +31.48%
surge wiped out in two days. Trump is open to pardoning CEO
Jensen Huang. U.S. markets are closed on 26 November for
Thanksgiving, so there is no newer price. Sources: Finnhub,
NY Post, 25 Nov 2026. Label: CONFIRMED.

### Hero 3 — Nor'easter Strikes on Thanksgiving
A nor'easter peaks on 26 November with 60–70 mph gusts, coastal
flooding from Georgia to Long Island, and 6–7 inches of wet snow
in St. Louis, as the 100th Macy's Thanksgiving Day Parade steps
off in New York — its balloons at risk if gusts pass 34 mph.
Sources: NWS/NOAA, Reuters, 26 Nov 2026. Label: OFFICIAL.

## The 10 medium cards
- Houthi drone hits a Riyadh tower for the second time; 11 hurt
  (24 Nov, CONFIRMED).
- Huawei guilty on 10 of 12 counts in Brooklyn; sentencing
  14 September 2027 (24 Nov, OFFICIAL).
- Shanghai party chief Chen Jining, 62, probed by the CCDI
  (24 Nov, OFFICIAL).
- Shenzhou-24 launches: first Pakistani in orbit, first foreigner
  aboard Tiangong (25 Nov, CONFIRMED).
- Bangladesh garment wage up 36% to 17,000 taka (25 Nov, CONFIRMED).
- U.S. tariffs: India up to 25%, Vietnam 35%, China 20%
  (25 Nov, OFFICIAL).
- Australia CPI +4.9% year on year; RBA rate 4.85%
  (25 Nov, OFFICIAL).
- Venezuela's debt $237.5bn, 242% of GDP (24 Nov, OFFICIAL).
- All Cartagena supermarket hostages freed (25 Nov, CONFIRMED).
- Vaibhav Sooryavanshi, 15, hits 204 off 53 balls — the fastest
  List A double century (24 Nov, CONFIRMED).

## Date check — excluded
The ICJ Myanmar ruling was 19 November, not 25 November. The
Hormuz mines are an older event. The Microsoft outage was
12–13 November, not 26 November. There is no Nvidia price for
26 November — U.S. markets are closed for Thanksgiving.

## Render locally

```sh
cd ..
python3 render26.py    # writes entry-26/entry.png (1024x1024, < 1 MiB)
sha256sum entry-26/entry.png   # run twice: the hash must not change
```

Requirements: Python 3 with Pillow, DejaVu fonts
(`/usr/share/fonts/truetype/dejavu/`). The render is fully
deterministic — fixed palette, fixed fonts, no randomness, no clock —
so repeated runs produce byte-identical output. The render script
itself is not part of the entry (it lives one directory up).

## Run the entrypoint

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
sha256sum out/entry.png entry.png   # both hashes must match
```

`main.ts` needs no network: it validates the bundled PNG (magic
bytes, 1024×1024 dimensions, 1 MiB cap), copies it to
`MAKEFUN_OUTPUT_DIR` (default `/output`), reads it back and verifies
the copy is byte-identical.

## License

MIT — see `LICENSE`.
