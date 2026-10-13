# FX Session Clock

A single-page visualizer (Thai by default, with a TH/EN toggle in the top corner) that shows which forex trading sessions are open right now, based on your own time zone, and what to watch for in each one.

Open `index.html` in a browser. There is no build step and no dependencies beyond Google Fonts.

## Features

- **Live phase readout**: the session or overlap you are trading in now (for example "London–New York overlap"), an estimated liquidity level, and what to look for and be aware of in that phase.
- **Centre clocks**: local time in Sydney, Tokyo, London and New York, with open/closed status and a countdown.
- **24-hour timeline**: session bars, overlaps, an estimated activity curve, key daily events (Tokyo fix, PBoC fixing, US data, NY option cut, London 4pm fix, rollover) and weekend closures, all in your time zone. Click it or use the slider to preview any time.
- **Session cards**: character, main pairs, what to look for, risks, and key times converted to your zone.
- **Alerts** for the daily rollover, the weekly open, Friday afternoons and month end.
- **My trading window**: enter the hours you trade to see how much of each session and overlap it covers.
- Daylight saving time is handled for every centre via `Intl`.

Session hours follow common FX conventions (each in local time): Sydney 07:00–16:00, Tokyo 09:00–18:00, London 08:00–17:00, New York 08:00–17:00. The spot week runs Sunday 17:00 to Friday 17:00 New York time. Bank holidays and central-bank meeting dates are not tracked.
