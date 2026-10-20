# Beijing Field Campaign — Site Briefing

**Campaign:** Fall atmospheric-sensing field campaign, Beijing
**Prepared:** 2026-10-20, 09:13 Beijing local time (Asia/Shanghai, UTC+8)
**Status:** Draft for team review — tracked in issue #1 (`Beijing site briefing status tracker`)

---

## 1. Current Conditions — Beijing

*Snapshot taken 2026-10-20 09:00 local time. Site coordinates ~39.93° N, 116.39° E.*

| Parameter | Value |
|---|---|
| Temperature | **12.3 °C** (54.1 °F) — feels like 9.5 °C |
| Condition | **Patchy rain nearby** (100% cloud cover) |
| Wind | **13.3 km/h (8.3 mph) from NNE** (15°); gusts to 19.9 km/h |
| Humidity | **63%** |
| Pressure | 1022 hPa |
| Visibility | 10 km |
| Precipitation | 0.02 mm (last hour); 17% chance of rain |
| UV index | 0.3 |

**Air quality (same snapshot):** PM2.5 **64.7 µg/m³**, PM10 **135 µg/m³**, NO₂ 56.2 µg/m³, O₃ 5 µg/m³, SO₂ 7.5 µg/m³, CO 2.4 mg/m³ → US EPA index **3 (Unhealthy for Sensitive Groups)**; UK DEFRA index 8 (High).

## 2. Timezone & Local Time

- **IANA timezone:** `Asia/Shanghai` — **UTC+8**, no daylight saving.
- Local time at preparation: **09:13, Tuesday 2026-10-20**.
- Rule of thumb: Beijing local time = UTC + 8 h (e.g., 09:00 Beijing = 01:00 UTC).

## 3. 7-Day Forecast (2026-10-20 → 2026-10-26)

| Date | Day | Daytime high | Overnight low | Rain chance | Conditions |
|---|---|---|---|---|---|
| 2026-10-20 | Tue | 15.2 °C | 9.7 °C | 59% (~4.0 mm) | Smoky haze; max wind 22.7 km/h; avg RH 48%; UV 2.6 |
| 2026-10-21 | Wed | 17.0 °C | 9.4 °C | 0% | Sunny; dry NW flow; avg RH 18%; UV 2.2 |
| 2026-10-22 | Thu | *n/a* | *n/a* | *n/a* | *(not retrievable — see note)* |
| 2026-10-23 | Fri | *n/a* | *n/a* | *n/a* | *(not retrievable — see note)* |
| 2026-10-24 | Sat | *n/a* | *n/a* | *n/a* | *(not retrievable — see note)* |
| 2026-10-25 | Sun | *n/a* | *n/a* | *n/a* | *(not retrievable — see note)* |
| 2026-10-26 | Mon | *n/a* | *n/a* | *n/a* | *(not retrievable — see note)* |

> **Data-availability note (days 3–7):** Daily summaries for Oct 22–26 could not be retrieved from the campaign's weather feed. The forecast endpoint returns the full hourly series for the current day first and truncates before later days' daily blocks; the history endpoint only serves dates up to tomorrow; and the future-weather endpoint only covers dates ≥ 14 days out. Sunrise/sunset/moon data **are** available for all seven days (Section 4). **Action:** re-pull the daily summaries for Oct 22–26 from the operational console before final sign-off.

**Operational read for the first 48 h:** Today (Tue) is the roughest day of the window — a 59% rain chance, smoky haze, and PM2.5 already at 64.7 µg/m³; keep optics sheltered and expect wet aerosol. A dry northwest airflow clears things overnight: Wednesday is sunny and dry (overnight RH ~18–20%, dew point ≈ −13 °C) with NW winds around 16–20 km/h and gusts near 50 km/h in the early hours — good ventilation and dispersion conditions, but secure loose equipment and expect wind noise on acoustic/micrometeorological sensors.

## 4. Astronomy & Observation Windows

### Tomorrow — Wednesday 2026-10-21

| Event | Time (local) |
|---|---|
| Sunrise | 06:31 |
| Sunset | 17:26 |
| Moonrise | 15:05 |
| Moonset | 01:17 (following night) |
| Moon phase | Waxing gibbous, **69% illuminated** |
| Daylight | ~10 h 55 min |

*Note: the dedicated astronomy feed reports 69% illumination for Oct 21, while a secondary feed reports 86% for the same date — treat it as a ~70–85% waxing gibbous. Moonrise/moonset times agree across feeds.*

### Week at a glance (2026-10-20 → 2026-10-26)

| Date | Sunrise | Sunset | Moonrise | Moonset | Moon phase (illum.) |
|---|---|---|---|---|---|
| Tue 10-20 | 06:30 | 17:28 | 14:42 | 00:16 | Waxing gibbous (77%) |
| Wed 10-21 | 06:31 | 17:26 | 15:05 | 01:17 | Waxing gibbous (69%) |
| Thu 10-22 | 06:32 | 17:25 | 15:26 | 02:18 | Waxing gibbous (78%) |
| Fri 10-23 | 06:33 | 17:23 | 15:47 | 03:18 | Waxing gibbous (86%) |
| Sat 10-24 | 06:34 | 17:22 | 16:08 | 04:20 | Waxing gibbous (92%) |
| Sun 10-25 | 06:35 | 17:21 | 16:31 | 05:24 | Waxing gibbous (97%) |
| Mon 10-26 | 06:36 | 17:19 | 16:58 | 06:30 | **Full moon (100%)** |

### Proposed observation windows (first 48 h)

1. **Pre-dawn dark-sky window, Wed 01:17 → 06:31.** Moon-free darkness for ~5 h before sunrise (moon sets 01:17). The overnight period is forecast clear with dry NW flow — the best window this week for night optical/aerosol work that needs no lunar contamination. Caveat: gusty NW winds (up to ~50 km/h) may introduce vibration on masts.
2. **Morning boundary-layer window, Wed 06:31 → ~09:30.** Sunrise plus the morning transition under sunny, dry, well-ventilated conditions — good for boundary-layer/aerosol sampling and instrument intercomparison.
3. **Evening window, Wed 17:26 → 01:17.** The waxing gibbous is up from 15:05, so the whole evening carries moonlight — useful for moonlight-referenced calibrations; avoid for dark-sky-sensitive measurements until after 01:17.
4. **Avoid today (Tue 10-20):** 59% rain chance, 100% cloud, smoky haze — unsuitable for solar/lunar optical observations; prioritize sheltered in-situ aerosol/gas measurements instead.

*(Window margins should be refined with civil/astronomical twilight tables at final sign-off; the windows above are anchored on the feed's sunrise/sunset/moon times.)*

## 5. Background Literature — Machine Learning for Urban Air-Quality Forecasting

### Citation

> **arXiv:2506.07616** — Geng, Z., Fan, X., Lu, X., Zhang, Y., Yu, G., Li, Y., Wang, Q., Huang, C., Ma, W., Yu, Q., Wu, L., & Li, H. (2025). *FuXi-Air: Urban Air Quality Forecasting Based on Emission-Meteorology-Pollutant multimodal Machine Learning.* arXiv:2506.07616 [cs.LG]. <https://arxiv.org/abs/2506.07616>

**Why this paper:** it is a recent (June 2025), directly on-topic work on machine learning for urban/megacity air-quality forecasting, and **Beijing is one of its three evaluation cities** (with Shanghai and Shenzhen), including Beijing-specific ablation results — the closest match to our campaign site and theme among the search hits. It was downloaded and read in full for this digest.

### Key points for the background section

1. **Multimodal fusion, not single-source ML.** FuXi-Air couples three input streams — AI meteorological forecasts (FuXi-2.0), CAMS emission inventories, and national station pollutant observations — in an attention/transformer framework, with a dual-scale architecture (a 6-hour autoregressive core plus a frame-interpolation stage that refines to hourly resolution). It delivers 72-hour forecasts for six pollutants (SO₂, NO₂, CO, O₃, PM2.5, PM₁₀) across multi-site urban networks in **25–30 seconds**, versus roughly 2–3 hours for equivalent CMAQ numerical runs — an order-of-magnitude-plus efficiency gain that matters for operational, campaign-support forecasting.

2. **Meteorology dominates predictability.** Ablation experiments show meteorological drivers contribute more to forecast skill than emission inventories, and full multisource fusion beats every reduced-input configuration. Adding meteorology alone lifted Beijing O₃ forecast correlation from R = 0.22 to R = 0.86 (ΔR = 0.64, with RMSE reduced by 23.4 µg/m³), whereas the emission inventory alone gave ΔR = 0.44; station-observation-only models stayed below R ≈ 0.5 with the highest RMSEs. Implication for us: high-quality, high-resolution meteorological measurements at the site are the single most valuable input to any ML forecast layer we build.

3. **Beijing is a "meteorology-sensitive" city.** The paper's city-scale mechanism analysis attributes Beijing's particulate pollution to regional transport (Mongolian/Siberian High, cross-border dust) combined with wintertime heating emissions, with the Yanshan Mountains' blocking effect and heating-season atmospheric stability affecting even primary pollutants (CO, SO₂: ΔR = 0.12–0.30 from meteorological inputs). For Beijing PM, forecast gains came overwhelmingly from meteorology (PM2.5 ΔR = 0.34; PM₁₀ ΔR = 0.13) and barely at all from the emission inventory (ΔR ≤ 0.03) — the opposite of emission-driven Shenzhen. This is directly relevant to how we weight meteorological vs. emission data in campaign analytics.

4. **Skill levels and a known weak spot.** Over the 72-hour horizon in Beijing, correlation is strongest for O₃ (R ≈ 0.88 at 1–24 h, ≈ 0.85 at 49–72 h), solid for PM2.5 (R ≈ 0.77 → 0.70, RMSE ≤ 27.2 µg/m³) and NO₂ (R ≈ 0.77 → 0.72), but weakest for PM₁₀ (R ≈ 0.57 → 0.44) because dust-storm and episodic transport spikes are under-captured. The model also uses a quantile loss to emit 10th/90th-percentile uncertainty bands, explicitly to flag high-pollution-risk episodes — a pattern worth adopting for our own forecasting layer. (Against two CMAQ configurations — SA07 and CB06 — FuXi-Air reduced 72-h RMSE for all six pollutants, e.g. −53.95%/−36.21% for O₃.)

### Relevance to the campaign

- Prioritize high-resolution meteorological instrumentation (wind, T/RH, pressure, radiation) alongside the pollutant sensors — the evidence says meteorological data drive most of the forecastable variance in Beijing.
- Expect PM₁₀ to be the hardest quantity to predict; design sampling to capture episodic dust-transport events (consistent with today's PM₁₀ = 135 µg/m³ vs PM2.5 = 64.7 µg/m³).
- Consider a quantile/uncertainty-aware forecasting layer rather than deterministic point forecasts.

## 6. Provenance & Caveats

- Weather and astronomy data pulled from WeatherAPI feeds on 2026-10-20 ~09:00–09:25 Beijing local time (current conditions, forecast, history, and astronomy endpoints).
- The Oct 22–26 daily weather rows could not be retrieved (see the note in Section 3); astronomy for those days is complete. These values must **not** be inferred or extrapolated — re-pull from the operational console.
- Minor source variance exists in the Oct 21 moon-illumination figure (69% vs 86% across two feeds); moonrise/moonset times agree.
- Literature: the full text of arXiv:2506.07616 (v1) was downloaded and read end-to-end for this digest.
- Tracking: issue #1 (tracker) and issue #2 (literature digest, sub-issue of #1). This document lives on branch `briefing-draft` at `docs/site-briefing.md`.
