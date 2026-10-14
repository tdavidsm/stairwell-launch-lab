# 🎯 Stairwell Launch Lab

**▶ Use it:** https://tdavidsm.github.io/stairwell-launch-lab/

A simulation of the stairwell projectile lab. A ball bearing rolls down a ramp and launches **horizontally**. Students find the ramp's launch speed at a lab table, then predict where the ball will land in the stairwell, place a target there, and get **one official drop**. The score depends on how close the carbon-paper mark is to the bullseye.

## The lab
- **🧪 Lab table (find the launch speed).** The ramp sits at the edge of a table. Each release leaves a mark on carbon paper on the floor. Students measure the drop height and the landing distances with the tape, then work backward: `t = √(2·Δy ÷ a)` and `Vx = Δx ÷ t`.
- **🪜 Stairwell (predict the landing).** Modeled on the real stairwell, looking along the stairs. From the landing out, there is the **landing railing**, then a **gap of about 15 cm (6 in)**, then the **stair railing** at the edge of the steps, then the step's tread.
  - The ramp's base rests on the landing railing with a clamp. Students drag it (or use **Hang out ◀ ▶**) to set how far it hangs out over the step. It **starts flush with the landing railing**.
  - The **plumb bob** hangs from the end of the ramp. It only marks the step if the ramp reaches past the stair railing. Otherwise it dangles down the gap or rests on the railing. The correct setup has it about 1 to 2 inches past the stair railing.
  - Students slide the ramp along the railing (side view) to line it up over the middle of a step. Each lower step is 18 cm farther below the railing. Then they measure the drop, calculate `t` and `Δx = Vx·t`, and place the target with the tape.
  - **Both classic mistakes are possible, and the result screen spots them.**
    - **Mistake 1:** leaving the ramp flush with the landing railing (over the gap) and measuring Δx from the step edge. The flight starts about 15 cm before the edge, so the target ends up too far out.
    - **Mistake 2:** hanging the ramp out but measuring from the step edge instead of the plumb mark. The target ends up short by the overhang.
    - Either way, the explanation names the cause.
  - Level 1 walks students through hanging the ramp out and measuring from the plumb mark. Levels 2 and 3 leave both mistakes open.
  - A ramp that isn't lined up over the middle of the step puts the mark off to the side, and far enough off it clips the step edge.
- **📏 Tape measure.** Turn it on and drag from one dot to another (ramp end, plumb mark, step edge, landing marks, bullseye). While the tape is on in the stairwell, a close-up of the step edge makes the plumb mark and the step edge easy to tell apart. Readings appear in the lab notebook to the millimetre and update live as the target moves. One drag to the cluster of landing marks gives a reading for each mark, and a magnified close-up shows them separately.
- **Scoring.** The target has 2 cm rings worth 100 / 80 / 60 / 40 / 20. The ball has realistic scatter (about ±0.6% in speed), so averaging several table launches helps. A careful student scores a bullseye almost every time.

## Three levels, less help each time
1. **Guided.** Fourteen prompted steps. Each measurement and calculation is checked before moving on, with hints (for example, "That looks like centimeters").
2. **Some help.** A checklist and blank X/Y setup tables. Nothing is checked, and the equations are tucked behind a "Need the equations?" toggle.
3. **On your own.** Just the equipment, the tape, a calculator and a notes box.

Each level (and each retry) uses a **different ramp and table height**, so numbers can't be carried over. Hitting the target paper (20+ points) unlocks the next level. After all three, students get a completion code: initials in the 3rd and 6th spots, with the total score after the dash.

## Teacher notes
- **🔑 Teacher unlock:** passcode **1253** opens every level until the page is reloaded.
- **Google Form turn-in:** connected to the *Stairwell Lab Simulation — Completions* form. **Turn it in** opens it with the name, code, the three level scores and the total filled in. To use a different form, make a pre-filled link with `NAME`, `CODE`, `L1`, `L2`, `L3`, `TOTAL` typed into the matching questions, and paste it into `FORM_PREFILL_LINK` near the top of the script.
- **Settings** (top of the script): railing height, gap width, stair-railing position and height, ramp base length and maximum overhang, step rise and depth, number of steps, stair width, target size, how close "lined up" must be, and the score needed to unlock the next level.
- Best scores are saved in the browser on that device.

## Tech
A single self-contained `index.html`: plain HTML/CSS/JS on canvas, with no dependencies. Built for iPad Safari; also works on Chromebooks and laptops.
