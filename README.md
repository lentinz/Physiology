# Physiology Interactive Models

**DPHT 7223: Physiology & Nutrition** · UNT Health · Fall 2026
Course director: Zachary Lentini, PT, DPT

Three interactive, browser-based models for post-lecture review and self-study of normal and exercise physiology: change one factor and see how the others respond. Each is a single HTML file, and each header links to the other two.

| Model | Live link | Lecture | What it shows |
|---|---|---|---|
| Cardiac Hemodynamics | [Open](https://lentinz.github.io/Physiology/cv-hemodynamics.html) | Dr. Anu Kalyanasundaram, *Cardiovascular System* | How heart rate, filling, contractility, resistance and blood volume affect stroke volume, cardiac output and blood pressure at rest and in exercise |
| Cardiac Electrophysiology | [Open](https://lentinz.github.io/Physiology/cv-electrophysiology.html) | Dr. Anu Kalyanasundaram, *Cardiovascular System* | Conduction, SA node and ventricular action potentials, the ECG, and autonomic control of heart rate |
| Pulmonary Physiology | [Open](https://lentinz.github.io/Physiology/cv-pulmonary.html) | Dr. Darby Smith, *Pulmonary Physiology* | Breathing mechanics, lung volumes, ventilation, gas exchange, oxygen transport, control of breathing and VO₂max |

Scope: **normal physiology and exercise physiology only.** Disease states are planned for a separate pathophysiology version, so physiology students are never switched into them by accident.

## The three people

All three models use the same three people, so a student can follow one person across systems. Same age (30); fitness is the only variable.

- **Drew** (deconditioned), **Taylor** (typical, the default) and **Elliot** (endurance-trained).
- Exercise intensity is a percent of each person's own maximum, so people are compared at the same relative effort.
- The pulmonary model takes heart rate and cardiac output straight from the hemodynamics model.
- Resting values and maxima (for example VO₂max of about 35, 46 and 58 mL/kg/min) are illustrative, not measured data.

## Hemodynamics model

Tabs: **Overview**, **Circulation**, **PV loop**, **Cardiac cycle**, **Frank-Starling**, **HR and output**, **Blood pressure**.

- Controls: person, exercise intensity, heart rate, filling, contractility, stiffness, resistance, blood volume, venous tone, muscle pump, breathing, posture and an optional baroreflex.
- Resting reference (Taylor): HR 70 bpm, SV about 70 mL, CO about 4.9 L/min, BP 120/80 mmHg. Maximal CO is about 21.5 L/min.
- Design decisions are in `DESIGN_Hemodynamics_v2.md`.

## Electrophysiology model

Tabs: **Overview**, **Conduction**, **Action potentials**, **ECG**, **Autonomic control**.

- Controls: person, exercise intensity and autonomic balance, with a comparison of all three people.
- Exercise withdraws vagal tone first, then raises sympathetic drive (Powers, Ch. 9).
- Intrinsic SA node rate with no nerve input is about 100 bpm. The resting rate is lower because of vagal tone.

## Pulmonary physiology model

Tabs: **Overview**, **Airways and breathing**, **Lung volumes**, **Ventilation**, **Gas exchange**, **O₂ transport**, **Control of breathing**, **Exercise and VO₂max**.

- Controls: person, exercise intensity, elevation (Gas exchange, O₂ transport and Control of breathing only), breathing pattern (Ventilation only), and pH, temperature and PCO₂ at the muscle (O₂ transport, with Show details).
- Resting reference (Taylor): 12 breaths/min × 500 mL, ventilation about 6 L/min, alveolar ventilation about 4.2 L/min, alveolar PO₂ about 100 mmHg, arterial saturation about 97%.
- VO₂ comes from the Fick equation (cardiac output × arterial-venous O₂ difference). Ventilation rises with VO₂ and then more steeply above the ventilatory threshold.
- Control of breathing follows the lecture: a fast rise from central command and joint and muscle input, then a slower chemical rise.
- Lung volumes are an introduction only. Altitude changes the inspired PO₂ only; acclimatization, altitude illness and performance are left to the environmental considerations lecture.
- Dead space is set at 150 mL per breath (not in the lecture slides). Resting ventilation is about 6 L/min; the lecture quotes about 5.

## Features common to all three

- A person selector and a dashed comparison line (typical person doing the same thing, or this person at rest).
- A collapsible concept panel on every tab, tap-to-explain question marks on chart elements, and a "What changed and why" note.
- Details toggles that default to off, a short scenario list per tab, and pause and speed controls (½× by default).
- A learning-objectives list with "Set up" buttons and prompts to try.
- An About sheet with sources, what is illustrative, and a disclaimer.
- Nothing relies on color alone. Works on desktop and phone, in light and dark mode. No scoring, accounts or tracking. Only the selected tab, details setting and ticked objectives are remembered, in the browser's local storage.

## Running it

Each file is a single self-contained HTML page. Open it in any modern browser, or host it with GitHub Pages:

1. Put all three files in the repository (the root, or a `/docs` folder): `cv-hemodynamics.html`, `cv-electrophysiology.html`, `cv-pulmonary.html`.
2. Go to **Settings → Pages**, choose the branch and folder, and save.
3. Keep the three files in the same folder, with these exact names, so the links between the models work.

Fonts (IBM Plex Sans and Mono) load from Google Fonts. Without a connection the page falls back to system fonts and works normally.

## Sources

- Kalyanasundaram A. *Cardiovascular System* (lecture slides). DPHT 7223, UNT Health, Fall 2026.
- Smith D. *Pulmonary Physiology* (lecture slides). DPHT 7223, UNT Health, Fall 2026.
- DPHT 7223 *Thermoregulation & Environmental Considerations* lecture slides (inspired PO₂ formula).
- Powers SK, Howley ET, Quindry JC. *Exercise Physiology: Theory and Application to Fitness and Performance*, 12th ed., Chapter 9.
- Severinghaus JW. Simple, accurate equations for human blood O₂ dissociation computations. *J Appl Physiol* 1979;46(3):599-602. [PubMed search](https://pubmed.ncbi.nlm.nih.gov/?term=Severinghaus+Simple+accurate+equations+for+human+blood+O2+dissociation+computations)
- Physiology, Lung Dead Space. *StatPearls*. <https://www.statpearls.com/point-of-care/24497>
- DPHT 7223 Module 3, Lab 5 (Cardiovascular Demands & Responses to Physical Activity) and Module 4, Lab 6 (Pulmonary Function Assessment & Application). Named only on the About sheets.

The full source lists, and which values are sourced versus illustrative, are on each model's About sheet.

## Limitations

These are simplified, qualitative teaching models. Constants are illustrative and are not patient data or clinical tools. Several citations (for example the hemodynamics blood pressure notes) have not been independently verified against the originals and should be checked before adoption.

> **These models were AI-generated and may contain errors. If anything here differs from the official course materials, the official course materials take precedence.**

## Credits

Built with Claude (Anthropic) under the direction of the course director. Review for accuracy against the course materials before adoption.

## License

Add a license of your choice before publishing (for example, CC BY-NC 4.0 for course materials). All rights reserved by default if none is added.
