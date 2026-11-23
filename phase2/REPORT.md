# USDJPY PHASE II - DATA RECEIPT & DIGEST

Run: phase2_digest.py (python 3.12.14) at 2026-11-23 08:16:11 UTC. Input dir: `/workspace/USDJPY`. Files found: 8.

## MANIFEST

| file | bytes | md5 | rows | first bar | last bar | tf | claimed | actual | symbol |
|---|---|---|---|---|---|---|---|---|---|
| CCMonthCapture USDJPY D1 20140728-20261123.csv | 647482 | 5919452581cbca937a321aaa9402feab | 11268 | 2014-07-28 21:00:00 | 2026-11-22 22:00:00 | d1 | 2014-2026 | 2014-07-28 21:00:00 .. 2026-11-22 22:00:00 | USDJPY |
| CCMonthCapture USDJPY h4 20140728-20261123.csv | 1010859 | 482acb97dfca9877d9f0ed2edaac2783 | 17617 | 2014-07-28 21:00:00 | 2026-11-23 06:00:00 | h4 | 2014-2026 | 2014-07-28 21:00:00 .. 2026-11-23 06:00:00 | USDJPY |
| CCMonthCapture USDJPY t100 20220101-20221231.csv | 12810654 | 4b6e79401991736d94cba78396c37e2f | 230672 | 2022-01-02 23:03:42 | 2022-12-30 21:55:46 | t100 | 2022 | 2022-01-02 23:03:42 .. 2022-12-30 21:55:46 | USDJPY |
| CCMonthCapture USDJPY t100 20230101-20231231.csv | 12088672 | 434c03b5095ca52ecdc220dacb4a1d87 | 217850 | 2023-01-01 22:19:01 | 2023-12-29 21:56:06 | t100 | 2023 | 2023-01-01 22:19:01 .. 2023-12-29 21:56:06 | USDJPY |
| CCMonthCapture USDJPY t100 20240101-20241231.csv | 12901623 | 8f0030db823f8c2a4f5f1d31180a3fcc | 232215 | 2024-01-01 22:15:52 | 2024-12-31 21:56:57 | t100 | 2024 | 2024-01-01 22:15:52 .. 2024-12-31 21:56:57 | USDJPY |
| CCMonthCapture USDJPY t100 20250101-20251231.csv | 12651200 | c530ab5391588e9cba15dc4836ed867a | 227674 | 2025-01-01 22:05:01 | 2025-12-31 21:58:58 | t100 | 2025 | 2025-01-01 22:05:01 .. 2025-12-31 21:58:58 | USDJPY |
| CCMonthCapture USDJPY t100 20260101-20261123.csv | 10400839 | a62e34d53e8fb6b5bd35d8ddd80cfdfc | 187147 | 2026-01-01 22:37:18 | 2026-11-23 07:18:13 | t100 | 2026 | 2026-01-01 22:37:18 .. 2026-11-23 07:18:13 | USDJPY |
| CCMonthCapture USDJPY t750 20220101-20261123.csv | 8113534 | 1df1e195e8d28b670d3022b096af0868 | 146078 | 2022-01-02 23:05:22 | 2026-11-23 07:45:29 | t750 | 2022-2026 | 2022-01-02 23:05:22 .. 2026-11-23 07:45:29 | USDJPY |

- **d1**: 11268 rows (1 file), 2014-07-28 21:00:00 .. 2026-11-22 22:00:00; overlap 0/0 identical, 0 conflicts.
- **h4**: 17617 rows (1 file), 2014-07-28 21:00:00 .. 2026-11-23 06:00:00; overlap 0/0 identical, 0 conflicts.
- **t100**: 1095558 rows (5 files), 2022-01-02 23:03:42 .. 2026-11-23 07:18:13; overlap 0/0 identical, 0 conflicts.
- **t750**: 146078 rows (1 file), 2022-01-02 23:05:22 .. 2026-11-23 07:45:29; overlap 0/0 identical, 0 conflicts.

## FORMAT

- CCMonthCapture USDJPY D1 20140728-20261123.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY h4 20140728-20261123.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY t100 20220101-20221231.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY t100 20230101-20231231.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY t100 20240101-20241231.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY t100 20250101-20251231.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY t100 20260101-20261123.csv: 7 fields date,time,O,H,L,C,V confirmed
- CCMonthCapture USDJPY t750 20220101-20261123.csv: 7 fields date,time,O,H,L,C,V confirmed

## INTEGRITY

- **d1**: wrong-field-count 0; OHLC violations 0; duplicate ts 0; non-monotonic 0; zero-range 0; zero-volume 0.
- **h4**: wrong-field-count 0; OHLC violations 0; duplicate ts 0; non-monotonic 0; zero-range 0; zero-volume 0.
- **t100**: wrong-field-count 0; OHLC violations 0; duplicate ts 0; non-monotonic 0; zero-range 0; zero-volume 0.
- **t750**: wrong-field-count 0; OHLC violations 0; duplicate ts 0; non-monotonic 0; zero-range 0; zero-volume 0.

## GAPS & SEAMS

Timezone evidence (finest timeframe t100): UTC: session-open days (first bar after a >6h gap) start at 21:00-23:59 in 100% of cases; the 21/22 split flips with US DST (EDT/EST), matching the 21:00/22:00 UTC session boundary (histogram in receipt.json).
- d1 (thr 10.0h): weekend 587, holiday 78, UNEXPLAINED 946.
- h4 (thr 10.0h): weekend 590, holiday 11, UNEXPLAINED 1.
- t100 (thr 6.0h): weekend 255, holiday 4, UNEXPLAINED 0.
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
- holiday gaps by name: Christmas x21; New Year's Day x19; MLK Day x10; Presidents Day x10; Memorial Day x10; Labor Day x10; Juneteenth x7; Independence Day x5
- hole map **d1**: 559 zero-bar days (incl. 295 Fridays - this timeframe has no Friday bars in part of its range): 2017-01-01, 2017-12-24 ... (full map in receipt.json)
- hole map **h4**: 308 zero-bar days (incl. 51 Fridays - this timeframe has no Friday bars in part of its range): 2017-01-01, 2017-12-24 ... (full map in receipt.json)
- hole map **t100**: 3 zero-bar days: 2022-12-25, 2023-12-24 ... (full map in receipt.json)
- hole map **t750**: 4 zero-bar days: 2022-12-25, 2023-01-01 ... (full map in receipt.json)
- weekend seams: 1431 total across timeframes, mean |drift| 0.09%, worst 5:
  - [h4] 2021-12-31 18:00:00 -> 2023-01-01 22:00:00 close 115.058 reopen 130.924 drift +15.866 (13.79%)
  - [h4] 2025-10-03 17:00:00 -> 2025-10-05 21:00:00 close 147.463 reopen 149.435 drift +1.972 (1.34%)
  - [d1] 2017-04-21 17:00:00 -> 2017-04-23 21:00:00 close 109.071 reopen 110.496 drift +1.425 (1.31%)
  - [h4] 2017-04-21 17:00:00 -> 2017-04-23 21:00:00 close 109.071 reopen 110.496 drift +1.425 (1.31%)
  - [d1] 2020-03-06 18:00:00 -> 2020-03-08 21:00:00 close 105.321 reopen 104.233 drift -1.088 (-1.03%)

## BAD TICKS

- **d1**: 68 flagged bars (delta_close x49; wick x30; C x8). Full rows in anomalies.csv.
- **h4**: 27 flagged bars (delta_close x20; wick x15; C x1). Full rows in anomalies.csv.
- **t100**: 5 flagged bars (H x5). Full rows in anomalies.csv.
  - CCMonthCapture USDJPY t100 20230101-20231231.csv 2023-08-11 20:55:05 O=144.944 H=144.962 L=144.812 C=144.952 V=100 [H == next-session reopen 144.962]
  - CCMonthCapture USDJPY t100 20240101-20241231.csv 2024-03-08 21:56:02 O=147.068 H=147.083 L=146.906 C=147.080 V=100 [H == next-session reopen 147.083]
- **t750**: 6 flagged bars (H x4; delta_close x2; wick x1). Full rows in anomalies.csv.

## CROSS-VALIDATION

- same-timeframe overlaps: no same-timeframe overlaps (one file per timeframe)
- daily H/L t100 vs d1, printed-day: 1268 days, H match 57 (4.5%), L match 58 (4.6%)
- daily H/L t100 vs d1, session-day: 1269 days, H match 1189 (93.7%), L match 1091 (86.0%)
- daily H/L t100 vs h4, printed-day: 1217 days, H match 143, L match 120
- daily H/L t100 vs h4, session-day: 1013 days, H match 198, L match 180
- daily H/L h4 vs d1, session-day: 2683 days, H match 622 (23.2%), L match 594 (22.1%) - h4 grid is offset from the d1 day stamp, both readings reported

## CALIBRATION DIGEST

(per-year tables shown for 2021+; full history incl. pre-2021 in receipt.json. Cost tiers for USDJPY: base 0.0030, stress 0.0050 per unit = 0.300/0.500 pips, as % of avg bar range.)

### d1 (reference bars/day ~n/a; ref ticks/day ~104000)

- d1: cross-validation/synthetic frame; per-year table and 2021+ stats in receipt.json.

### h4 (reference bars/day ~n/a; ref ticks/day ~104000)

- h4: cross-validation/synthetic frame; per-year table and 2021+ stats in receipt.json.

### t100 (reference bars/day ~n/a; ref ticks/day ~104000)

| year | bars | days | bars/day | ticks/day | min/bar | avg rng | med rng | avg rng % | base % | stress % |
|---|---|---|---|---|---|---|---|---|---|---|
| 2022 | 230672 | 311 | 741.7 | 74171.0 | 1.25 | 0.038 | 0.032 | 0.03 | 7.92 | 13.19 |
| 2023 | 217850 | 311 | 700.5 | 70048.0 | 1.42 | 0.038 | 0.033 | 0.03 | 7.9 | 13.17 |
| 2024 | 232215 | 314 | 739.5 | 73954.0 | 1.3 | 0.04 | 0.033 | 0.03 | 7.59 | 12.66 |
| 2025 | 227674 | 312 | 729.7 | 72972.0 | 1.33 | 0.039 | 0.034 | 0.03 | 7.61 | 12.68 |
| 2026 | 187147 | 280 | 668.4 | 66838.0 | 1.43 | 0.031 | 0.026 | 0.02 | 9.64 | 16.06 |

- hourly bar density (00-24, printed hours): 00:53009 01:51659 02:40231 03:35040 04:33113 05:37359 06:48776 07:59575 08:58904 09:50844 10:45150 11:46264 12:61989 13:73934 14:77030 15:67361 16:51344 17:42691 18:40685 19:37045 20:25955 21:11632 22:18061 23:27907
- dead hours: none; top hours: 14,13,15,12,07,08
- Feb-Mar 2026: peak H 160.462 @ 2026-03-29 22:35:22; max close 160.451 @ 2026-03-29 22:41:29; max bar range 0.956 @ 2026-02-11 13:29:51; max |dC| 0.57% @ 2026-02-11 13:29:51; March trough close 156.096; drawdown from max close 2.71%.
### t750 (reference bars/day ~n/a; ref ticks/day ~104000)

- t750: cross-validation/synthetic frame; per-year table and 2021+ stats in receipt.json.


## PHASE II READINESS

- t500 ABSENT: MA layer not runnable; t500 exports required.
- t100 2022-01-02..2026-11-23: entry layer READY (1095558 bars), but faithful-transpose cells NOT runnable - t500 MA layer absent, t500 exports required.
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
