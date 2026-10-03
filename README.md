# Lights Out

A single-page Formula 1 trivia site built around the 2026 Bahrain Grand Prix in Malaysia, held at Sepang.

## What is in it

- A start-lights reaction test with synthesised engine sound
- The race weekend: circuit maps for Sepang and Sakhir, a simulated lap, session times and results, and Sepang's history
- 2026 championship standings for drivers and teams
- F1 teams, with a head-to-head card for each pair of teammates
- F1 history, season by season since 1950
- All-time records, an eight-question quiz and quick facts
- English and Bahasa Melayu, switched from the header

## Files

Everything is in `index.html`. There is no build step and nothing to install.

## Publish with GitHub Pages

1. Create a repository and upload `index.html` and this `README.md`.
2. Open the repository's **Settings**, then **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and the `/ (root)` folder, and save.
4. After a minute the site is live at `https://<username>.github.io/<repository>/`.

To serve it from the root of a user site, put `index.html` in the `<username>.github.io` repository instead.

## Things to know

- **Data is fixed in the page.** Standings are as of round 15 and session results were last updated on 3 October 2026. Nothing is fetched live, so update the numbers in `index.html` by hand.
- **Fonts** load from Google Fonts. The page falls back to system fonts if they are unavailable.
- **Sound** is generated in the browser with the Web Audio API. There are no audio files.
- **Car tech section** is present in the code but hidden. Remove the `hidden` attribute from `<section id="tech">` to bring it back; it loads three.js from cdnjs when shown.
- **Language and sound preferences** are saved in the visitor's browser with `localStorage`.

## Credits

- Circuit outlines are drawn from the open [f1-circuits](https://github.com/bacinger/f1-circuits) dataset by Tomislav Bacinger.
- Flags, helmets and team badges are original drawings.

This is an unofficial fan page. It is not affiliated with Formula 1, the FIA or any team.
