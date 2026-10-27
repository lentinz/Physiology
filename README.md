# Cardiovascular Interactive Models

**DPHT 7223: Physiology & Nutrition** · UNT Health · Fall 2026
Course director: Zachary Lentini, PT, DPT

Two interactive, browser-based models for reviewing the cardiovascular lecture (Dr. Anu Kalyanasundaram, *Cardiovascular System*). They are meant for post-lecture review and self-study: change one factor and see how the others respond.

| Model | Link | What it shows |
|---|---|---|
| Cardiac Hemodynamics | [Open the hemodynamics model](https://lentils.github.io/Physiology/cv-hemodynamics.html) | How heart rate, preload, afterload, contractility, blood volume and venous return affect stroke volume, ejection fraction, cardiac output and blood pressure |
| Cardiac Electrophysiology | [Open the electrophysiology model](https://lentils.github.io/Physiology/cv-electrophysiology.html) | Conduction, SA node vs ventricular action potentials, autonomic control of heart rate, the ECG, and common arrhythmias |

**Live versions (GitHub Pages):**

- Hemodynamics: <https://lentils.github.io/Physiology/cv-hemodynamics.html>
- Electrophysiology: <https://lentils.github.io/Physiology/cv-electrophysiology.html>

## Hemodynamics model

Tabs: **Circulation**, **PV loop**, **Cardiac cycle**, **Frank-Starling**, **HR and output**, **Venous return**.

- Controls: heart rate, preload and filling, contractility, ventricular stiffness, afterload (resistance), blood volume, venous tone, muscle pump, breathing, posture, exercise intensity, and an optional baroreflex.
- Preset scenarios: rest, exercise (moderate and maximal), standing, blood loss, weak pump, trained athlete, and others.
- Resting reference values: HR 70 bpm, EDV about 120 mL, ESV about 50 mL, SV about 70 mL, EF about 58%, CO about 4.9 L/min, BP 120/80 mmHg.
- Maximal untrained exercise gives a cardiac output of about 21 L/min, in line with Powers Table 9.2.

## Electrophysiology model

Tabs: **Conduction**, **Action potentials**, **ECG**.

- Controls: exercise intensity, sympathetic activity, parasympathetic (vagal) activity, extracellular K⁺, and rhythm (sinus, atrial fibrillation, ventricular tachycardia, ventricular fibrillation).
- Exercise withdraws vagal tone first, then raises sympathetic drive (Powers, Ch. 9).
- Action potential phases and the main currents are drawn qualitatively. The contraction (E-C coupling) trace is optional.
- Intrinsic SA node rate with no nerve input is about 100 bpm. Resting rate is about 70 bpm.

## Features common to both

- Preset scenarios, a "pin current as reference" dashed overlay, and a plain-language note on what changed and why.
- A learning-objectives list mapped to the lecture objectives, with "Set up" buttons and prompts to try.
- Connections to Module 3, Lab 5 (Cardiovascular Demands & Responses to Physical Activity).
- An About sheet with sources and a disclaimer.
- Works on desktop and phone, in light and dark mode. No scoring, accounts or tracking. Only the selected tab and ticked objectives are remembered, in the browser's local storage.

## Running it

Each file is a single self-contained HTML page. Open it in any modern browser, or host it with GitHub Pages:

1. Put both HTML files in the repository (the root, or a `/docs` folder).
2. Go to **Settings → Pages**, choose the branch and folder, and save.
3. Keep the two files in the same folder so the links between the models work.

Fonts (IBM Plex Sans and Mono) load from Google Fonts. Without a connection the page falls back to system fonts and works normally.

## Sources

- Kalyanasundaram A. *Cardiovascular System: Cardiac Function, Electrophysiology and Blood Circulation* (lecture slides). DPHT 7223, UNT Health, Fall 2026.
- Berne & Levy, *Physiology*, 6th ed. (action potential and excitation-contraction coupling figures cited in the lecture slides).
- Boron & Boulpaep, *Medical Physiology*, 3rd ed. (conduction system and arrhythmia figures cited in the lecture slides).
- Powers SK, Howley ET, Quindry JC. *Exercise Physiology: Theory and Application to Fitness and Performance*, 12th ed., Chapter 9, Circulatory Responses to Exercise.
- DPHT 7223 Module 3, Lab 5: Cardiovascular Demands & Responses to Physical Activity.

## Limitations

These are simplified, qualitative teaching models. Constants are illustrative and are not patient data or clinical tools. The electrophysiology model stays at lecture level, and the K⁺ slider goes slightly beyond the slides.

> **This model was AI-generated and may contain errors. If anything here differs from the official course materials, the official course materials take precedence.**

## Credits

Built with Claude (Anthropic) under the direction of the course director. Review for accuracy against the course materials before adoption.

## License

Add a license of your choice before publishing (for example, CC BY-NC 4.0 for course materials). All rights reserved by default if none is added.
