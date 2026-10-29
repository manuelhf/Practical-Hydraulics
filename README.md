# CEG8102 — Practical Hydraulics

Interactive teaching website for Practical Hydraulics at Newcastle University, developed from Dr Manuel Herrera's lecture presentations.

## Contents

- **Hydrostatics and hydrodynamics:** properties of liquids, hydrostatic pressure, gates, and pressure head.
- **Pipe flow, Part 1:** Bernoulli's equation, ideal tank discharge, and Venturi meters.
- **Pipe flow, Part 2:** Reynolds number, friction factors, energy losses, Darcy–Weisbach, Hazen–Williams, and pipe sizing.
- **Pipe networks:** pipes in series, parallel and branched systems, distribution hydraulics, and a quickfire quiz.
- **EPANET and WEPANET:** a two-screen introduction to the EPANET modelling framework (network components, inputs, governing principles, outputs, and extended-period simulation), followed by the [KIOS WEPANET interactive resource](https://kios-research.github.io/WEPANET/). The [KIOS WEPANET GitHub repository](https://github.com/KIOS-Research/WEPANET) provides supporting project resources, and [epanet-js](https://epanetjs.com/) is an auxiliary browser-based option.

All **76 original lecture slides** now appear as complete, full-width teaching screens in the same order as the supplied decks. They display the complete source slides, and clicking each slide enlarges it. The relevant manual solution and interactive experiments are positioned directly after the corresponding original slide. The 22 earlier source-derived illustrations have been retained as assets for compatibility.

The 22 slide-derived figures display the **complete lecture slides as previews**, and clicking each preview enlarges the **same complete slide**. No cropped-figure previews are used. The Newcastle University branding is drawn from the lecturer-provided slides.

Interactive calculations are explanatory teaching models with stated assumptions. They are not professional hydraulic design software.

## Publish on GitHub Pages

1. Create a GitHub repository. Before publishing publicly, check redistribution permissions for University and third-party figures.
2. Upload the **contents** of this folder — `index.html`, `README.md`, and `assets/` — to the repository root.
3. Open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, and save.
4. Use the published GitHub Pages URL in Canvas. No build dependencies or web server are required.

The separate `Practical_Hydraulics_Standalone.html` file is provided for local use and review, with all slide images and university marks embedded. It is not required for the GitHub Pages repository.

## Classroom controls

- Open a session from the home page or sidebar, and navigate with Next/Previous or the left/right arrow keys.
- **Focus mode** removes the sidebar for projection.
- Click a slide image to enlarge it. Use **Close** or **Esc** to return to the lesson.
- **Study notes** expand to show brief explanations.
- Hydraulic sliders and the quickfire quiz work locally without a network connection.
- Vevox polls require a separate Vevox session. This site does not create or open Vevox polls.

### Vevox ID

Set `PUBLISHED_VEVOX_SESSION` in `index.html` to the **nine-digit student joining ID**, if you want the number visible to all viewers. Keep account credentials and presenter tokens private. Without a published joining ID, the lecturer may set it locally using the **Vevox** button; it does not propagate to student devices.

The existing poll prompts include a word cloud about liquids, and a question about whether discharge remains constant as a tank empties. The quickfire game in Lecture 8 runs directly in the website.

## Simplifications and scope

- The hydrostatic gate assumes a vertical rectangular plate with its top at the water surface.
- Tank discharge uses an instantaneous, ideal outlet calculation; no dynamic emptying simulation.
- The Venturi model assumes steady horizontal incompressible flow without hydraulic losses.
- Darcy friction factors use a turbulent approximation, 64/Re under laminar conditions, and no false precision in transition.
- Pipe examples use explicit assumptions on local-loss coefficients, roughness, flow conditions, and viscosity.
- All videos and modelling apps are external links, so availability depends on internet access and the provider.
- The KIOS WEPANET website and GitHub URL were supplied for this course; verify that both open successfully on the teaching-room network before the practical. The introductory EPANET concepts are based on the [US EPA EPANET documentation](https://www.epa.gov/water-research/epanet).

## File structure

```
index.html
README.md
assets/
  slide-*.webp          # complete 16:9 lecture slide previews
  newcastle-*.webp      # crest and wordmark
  *.webp                # retained source-derived assets
```

© Course teaching materials. Check redistribution permissions before public hosting.


## Worked hydraulic solutions

Fourteen full, student-facing manual solution screens are located immediately before the corresponding interactive experiments. They use the lecture gate, tank, reservoir, pipe-sizing, local-loss, and parallel-pipe cases, together with clearly labelled illustrative extensions where the lecture materials provide a symbolic method. Hand calculations are visible and do not require JavaScript. The interactive experiments follow as consolidation.

Two original slide values warrant care: with D=0.2 m and v=4.0 m/s the short-pipeline discharge is 0.126 m³/s (the slide says approximately 0.123 m³/s). With the stated SI Hazen–Williams formula, C=130, Q=0.4 m³/s, and D=0.45 m, the head loss is about 58 m; therefore that trial diameter fails a 50 m criterion by Hazen–Williams even though it meets the Darcy–Weisbach criterion.

## Source-faithful teaching sequence

The four sections use the complete original decks in order: Lecture 2 (14 slides), Lecture 3 (12 slides), Lectures 6–7 (31 slides), and Lecture 8 (19 slides). The original slide image is the primary source of content and equations. Full slide text can be opened under each slide, and supplementary explanations, hand-calculation steps, and interactive demonstrations are placed next to their corresponding slides. The source PDF exports are used only as input to generate images and are not distributed. No changes were made to the original Google Slides.
