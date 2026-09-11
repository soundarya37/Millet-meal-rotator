# Millet Meal Rotator (Prototype)

A single-file HTML companion tool for a beginner transition to a millet-based diet, built around Dr. Khadar Vali's Siridhanya rotation rule: one millet variety per day, rotated every two days, never mixed.

## Description

This is a lightweight feel-test, not a full tracker. It answers one question day to day: which millet am I on, and did I soak it in time? The tool locks each two-day block to a single variety so varieties don't accidentally cross, and surfaces a soak reminder and meal suggestions for that day.

Three parts:
- **Today card** — shows the day's assigned millet, which day of its two-day window you're on, a soak reminder, and meal suggestions for either 1 or 2 meals/day.
- **This week's rotation** — a 7-day strip (2 days back, today, 4 days ahead) showing which millet lands on which day.
- **Millet library** — reference notes per variety: soak time, texture, and what it works well as.

All data is in-memory placeholder content and resets on reload. The rotation is calculated from whatever start date you set, cycling through foxtail, kodo, and little millet — the three varieties currently on hand.

## Visuals

Botanical-dark theme, consistent with the rest of the build series: deep green panels on a near-black green background, parchment text, turmeric accent for the featured millet, sage for meal-slot labels, terracotta for the soak reminder. Fraunces for headings, Inter for body text, IBM Plex Mono for tags and dates.

## Installation

No build step. Download `millet-meal-rotator.html` and open it directly in any modern browser.

## Usage

- Set a start date — the rotation counts two-day blocks forward from that date.
- Toggle between "1 meal/day" and "2 meals/day" to match where you are in scaling up.
- The today card shows the assigned millet, soak reminder, and meal suggestions for the current day.
- The week strip shows a quick look at neighboring days without changing the start date.
- Edit the `millets` array in the script to add varieties, change meal suggestions, or update soak times.

## Support

Personal prototype with no support channel. Edit the single HTML file directly to change data or styling.

## Roadmap

- Pull meal suggestions directly from Dr. Khadar Vali's book content instead of placeholder dishes.
- Handle the "soak a bigger batch at the start of the window" workaround explicitly, rather than reminding per day.
- Add flour-making prep (6–8 hr soak + 2-day sun-dry) as a separate reminder track from same-day cooking.
- Extend the millet library as more varieties are purchased.
- Possible link to the Pantry meal planning app for shared recipe data.

## Contributing

Solo project for now — no external contributions expected.

## Authors and acknowledgment

Built by Soundarya as part of an ongoing series of single-file HTML creative and household-tooling builds.

## License

Personal project — no license specified.

## Project status

Prototype / concept test. Not actively maintained beyond this initial pass.
