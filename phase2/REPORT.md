# USDJPY PHASE II - DATA RECEIPT & DIGEST

Run: phase2_digest.py (python 3.12.14) at 2026-11-23 08:13:47 UTC. Input dir: `/workspace/USDJPY`. Files found: 3.

## MANIFEST

| file | bytes | md5 | rows | first bar | last bar | tf | claimed | actual | symbol |
|---|---|---|---|---|---|---|---|---|---|
| CCMonthCapture USDJPY D1 20140728-20261123.csv | 647482 | 5919452581cbca937a321aaa9402feab | 11268 | 2014-07-28 21:00:00 | 2026-11-22 22:00:00 | d1 | 2014-2026 | 2014-07-28 21:00:00 .. 2026-11-22 22:00:00 | USDJPY |
| CCMonthCapture USDJPY h4 20140728-20261123.csv | 1010859 | 482acb97dfca9877d9f0ed2edaac2783 | 17617 | 2014-07-28 21:00:00 | 2026-11-23 06:00:00 | h4 | 2014-2026 | 2014-07-28 21:00:00 .. 2026-11-23 06:00:00 | USDJPY |
| CCMonthCapture USDJPY t750 20220101-20261123.csv | 8113534 | 1df1e195e8d28b670d3022b096af0868 | 146078 | 2022-01-02 23:05:22 | 2026-11-23 07:45:29 | t750 | 2022-2026 | 2022-01-02 23:05:22 .. 2026-11-23 07:45:29 | USDJPY |

- **d1**: 11268 rows (1 file), 2014-07-28 21:00:00 .. 2026-11-22 22:00:00; overlap 0/0 identical, 0 conflicts.
- **h4**: 17617 rows (1 file), 2014-07-28 21:00:00 .. 2026-11-23 06:00:00; overlap 0/0 identical, 0 conflicts.
- **t750**: 146078 rows (1 file), 2022-01-02 23:05:22 .. 2026-11-23 07:45:29; overlap 0/0 identical, 0 conflicts.

## FORMAT

- CCMonthCapture USDJPY D1 20140728-20261123.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY h4 20140728-20261123.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY t750 20220101-20261123.csv: 7 fields date,time,O,H,L,C,V confirmed

## INTEGRITY

- **d1**: wrong-field-count 0; OHLC violations 0; duplicate ts 0; non-monotonic 0; zero-range 0; zero-volume 0.
- **h4**: wrong-field-count 0; OHLC violations 0; duplicate ts 0; non-monotonic 0; zero-range 0; zero-volume 0.
- **t750**: wrong-field-count 0; OHLC violations 0; duplicate ts 0; non-monotonic 0; zero-range 0; zero-volume 0.

## GAPS & SEAMS

Timezone evidence (finest timeframe t750): UTC: session-open days (first bar after a >6h gap) start at 21:00-23:59 in 99% of cases; the 21/22 split flips with US DST (EDT/EST), matching the 21:00/22:00 UTC session boundary (histogram in receipt.json).
- d1 (thr 10.0h): weekend 587, holiday 78, UNEXPLAINED 946.
- h4 (thr 10.0h): weekend 590, holiday 11, UNEXPLAINED 1.
- t750 (thr 6.0h): weekend 255, holiday 4, UNEXPLAINED 0.
  - UNEXPLAINED 2020-12-31 14:00:00 -> 2022-01-02 22:00:00 (8816.0h)
  - UNEXPLAINED 2022-01-02 22:00:00 -> 2022-01-03 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-03 22:00:00 -> 2022-01-04 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-04 22:00:00 -> 2022-01-05 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-05 22:00:00 -> 2022-01-06 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-09 22:00:00 -> 2022-01-10 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-10 22:00:00 -> 2022-01-11 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-11 22:00:00 -> 2022-01-12 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-12 22:00:00 -> 2022-01-13 22:00:00 (24.0h)
  - UNEXPLAINED 2022-01-18 22:00:00 -> 2022-01-19 22:00:00 (24.0h)
  - ... 937 more unexplained gaps in receipt.json
- holiday gaps by name: Christmas x19; New Year's Day x17; MLK Day x10; Presidents Day x10; Memorial Day x10; Labor Day x10; Juneteenth x7; Independence Day x5
- hole map **d1**: 559 zero-bar days (incl. 295 Fridays - this timeframe has no Friday bars in part of its range): 2017-01-01, 2017-12-24 ... (full map in receipt.json)
- hole map **h4**: 308 zero-bar days (incl. 51 Fridays - this timeframe has no Friday bars in part of its range): 2017-01-01, 2017-12-24 ... (full map in receipt.json)
- hole map **t750**: 4 zero-bar days: 2022-12-25, 2023-01-01 ... (full map in receipt.json)
- weekend seams: 1176 total across timeframes, mean |drift| 0.10%, worst 5:
  - [h4] 2021-12-31 18:00:00 -> 2023-01-01 22:00:00 close 115.058 reopen 130.924 drift +15.866 (13.79%)
  - [h4] 2025-10-03 17:00:00 -> 2025-10-05 21:00:00 close 147.463 reopen 149.435 drift +1.972 (1.34%)
  - [d1] 2017-04-21 17:00:00 -> 2017-04-23 21:00:00 close 109.071 reopen 110.496 drift +1.425 (1.31%)
  - [h4] 2017-04-21 17:00:00 -> 2017-04-23 21:00:00 close 109.071 reopen 110.496 drift +1.425 (1.31%)
  - [d1] 2020-03-06 18:00:00 -> 2020-03-08 21:00:00 close 105.321 reopen 104.233 drift -1.088 (-1.03%)

## BAD TICKS

- **d1**: 68 flagged bars (delta_close x49; wick x30; C x8). Full rows in anomalies.csv.
- **h4**: 27 flagged bars (delta_close x20; wick x15; C x1). Full rows in anomalies.csv.
- **t750**: 6 flagged bars (H x4; delta_close x2; wick x1). Full rows in anomalies.csv.

## CROSS-VALIDATION

- same-timeframe overlaps: no same-timeframe overlaps (one file per timeframe)
- daily H/L t750 vs d1, printed-day: 1267 days, H match 60 (4.7%), L match 40 (3.2%)
- daily H/L t750 vs d1, session-day: 1269 days, H match 1138 (89.7%), L match 1056 (83.2%)
- daily H/L t750 vs h4, printed-day: 1216 days, H match 130, L match 92
- daily H/L t750 vs h4, session-day: 1011 days, H match 174, L match 168
- daily H/L h4 vs d1, session-day: 2683 days, H match 622 (23.2%), L match 594 (22.1%) - h4 grid is offset from the d1 day stamp, both readings reported

## CALIBRATION DIGEST

(per-year tables shown for 2021+; full history incl. pre-2021 in receipt.json. Cost tiers for USDJPY: base 0.0030, stress 0.0050 per unit = 0.300/0.500 pips, as % of avg bar range.)

### d1 (reference bars/day ~n/a; ref ticks/day ~104000)

- d1: cross-validation/synthetic frame; per-year table and 2021+ stats in receipt.json.

### h4 (reference bars/day ~n/a; ref ticks/day ~104000)

- h4: cross-validation/synthetic frame; per-year table and 2021+ stats in receipt.json.

### t750 (reference bars/day ~n/a; ref ticks/day ~104000)

- t750: cross-validation/synthetic frame; per-year table and 2021+ stats in receipt.json.


## PHASE II READINESS

- t500 ABSENT: MA layer not runnable; t500 exports required.
- t100 entry layer ABSENT - faithful-transpose cells not yet runnable offline; t100 exports still required. t300/t750 cells are not derivable from t500 alone.
- not present in this run: t300, t500. t300 would be derivable from t100 (groups of 3, phase calibrated by sweep) if t100 present; t750 from t1 ticks (groups of 750) where tick coverage exists; neither is derivable from a coarser bar file alone.
- present extra timeframes enabling cross-validation: t750, h4, d1. NOT present in this run: t300.
- No strategy backtest in this run - receipt and digest only; the strategy grid is a separate, later prompt.

## METHOD

- Tool: `phase2_digest.py` (python 3.12.14, stdlib only): `python3 phase2_digest.py <input_dir> [--instrument I --spread-base B --spread-stress S --pip P --synth-t500] [--out DIR]`; artifacts written next to the data; raw files read-only (in-memory copies).
- Parse: CSV, delimiter/header auto-detected; dates YYYY.MM.DD/YYYY-MM-DD/YYYY/MM/DD/YYYYMMDD; times HH:MM[:SS[.fff]]; bar files = 7 fields date,time,O,H,L,C,V (time,date auto-swapped); tick files = 4 fields date,time,bid,ask (ms timestamps) summarized as tick reference only. Bar timestamps are OPEN times, printed as-is; close-time = next bar open; last bar of each file open-ended.
- Symbol gate per file: median price outside the USDJPY range (>=200) => SUSPECT wrong symbol, excluded from merge, both readings reported. XAUUSD ref 2021->2026 ~1798->~4500s; GBPJPY ref ~124-220; USDJPY ~101-160.
- Merge per timeframe: dedupe by timestamp across files; overlaps compared bit-for-bit on printed OHLCV; conflicts reported with both readings (first file kept for stats, count disclosed). Integrity: field count != 7; H < max(O,C) or L > min(O,C); duplicate/non-monotonic timestamps; zero-range; zero-volume.
- Gap threshold per timeframe = max(6h, 2.5x median inter-bar gap). Class: weekend = Thu/Fri/Sat -> Sun/Mon 40-80h (intraday DST-adjusted 48-50h: 49h + Sun-Fri UTC offset, 4h EDT / 5h EST); holiday = span covers a computed US federal holiday 1998-2026 (Good Friday via computus, observance shifts, + 2025-01-09); else UNEXPLAINED (each listed). Hole map: zero-bar dates in [first,last] excl. Saturdays + listed holidays.
- Bad ticks (instrument-scaled, % of price): |dClose| > 1.5% of prev close (across_gap if gap > threshold), wick (H-L) > 2.5% of close, H or C == next session's reopen open (3dp) after such a gap (feed-contamination class). All flagged -> anomalies.csv; nothing deleted or fixed.
- Cross-validation: same-timeframe overlap equality; t500 = groups of 5 consecutive t100 (all 5 phases swept from file start, exact OHLCV + span); t300 = groups of 3; t100/t750 vs groups of 100/750 t1 ticks (mid and bid); daily H/L of finest frame vs h4/d1 under BOTH day definitions: printed date and DST-aware session day (open 22:00 UTC EDT / 23:00 UTC EST); --synth-t500 builds t500 from t100 groups of 5 phase 0, marked SYNTHETIC (on XAUUSD native t500 matched phase 3, 375380/375380 exact, so synthetic phase-0 grid is not bit-identical to the native chart).
- Digest: per-year bars/day, implied ticks/day = bars/day x tick size, median min/bar, avg/median range and % of close; cost ratio = spread / avg range (base 0.003, stress 0.005 per unit = 0.3/0.5 pips); hourly density on printed hours; Feb-Mar 2026 blowoff/crash metrics; weekend seam drift = reopen - prior close. Timezone: session-open first-bar hour histogram of finest timeframe vs the 21:00/22:00 UTC boundary (DST-shifting).
- Budget: REPORT.md hard-capped at 15 KB (long lists truncated here; full detail in receipt.json / anomalies.csv). Prices 3dp, percentages 2dp, timestamps full date+time as printed.
