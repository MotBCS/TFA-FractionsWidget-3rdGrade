# Fractions Widget - 3rd Grade

## Grade Level
3rd Grade

## Subject Area
Math

## Topic
Fractions — Adding Fractions with the Same Denominator

## Objective
This widget is designed to teach a short, focused 5-minute lesson on adding fractions that share the same denominator. Using a pizza as a visual model, students will learn:

- What a fraction's **numerator** (top number) and **denominator** (bottom number) represent
- That when two fractions have the **same denominator**, you only need to add the numerators, and the denominator stays the same
- How to apply this rule to solve addition problems, both with multiple-choice questions and a fill-in-the-blank challenge
- How to check their own understanding through immediate, encouraging feedback

By the end of the lesson, students should be able to explain the "same bottom number" rule in their own words and correctly add two or more fractions with matching denominators.

---

## Widget Walkthrough

The widget is a single self-contained webpage with a purple header, a progress bar, and one "screen" visible at a time. Students move forward and backward using **Next →** and **← Back** buttons, and the progress bar/step counter at the top always shows where they are in the lesson (e.g., "2 of 6").

**Step 0 — Welcome**
An introduction screen with a friendly greeting, a large animated pizza emoji, and a short message from the "teacher" setting up the lesson. Students click **Start the lesson!** to begin.

**Step 1 — What's a numerator and a denominator?**
A visual diagram of the fraction 3/4, with the numerator highlighted and labeled with a downward arrow, and the denominator highlighted and labeled with an upward arrow. Two short explanation boxes define each part in plain, 3rd-grade language.

**Step 2 — Warm-up: Count the pieces**
A circular pizza is shown cut into 8 equal slices with 3 slices colored in. Students answer a multiple-choice question ("What fraction was served?") to practice identifying a fraction from a picture. A "Remember" tip reinforces what the numerator and denominator mean.

**Step 3 — Learn the fraction rule**
The core rule is introduced: *"When the bottom numbers match, just add the top numbers. The bottom number stays the same!"* This is illustrated with the equation 2/8 + 3/8 = 5/8, shown both as stacked-fraction notation and as three side-by-side pizza circles (2 slices filled, 3 slices filled, 5 slices filled).

**Step 4 — Let's try it together**
A guided practice problem (1/6 + 2/6 = ?) using two pizzas and a "?" placeholder. Students select the correct answer from three choices and get instant feedback explaining why it's correct or how to fix their thinking.

**Step 5 — Let's try a challenge!**
An independent challenge where three friends (Amy, Morgan, and Max) share a 10-slice pizza. A single pizza is shown with three color-coded wedges (one color per friend) and a matching legend. Students type in the missing numerator (3 + 2 + 2) and click **Check my answer** to get feedback, retrying if needed.

**Step 6 — Recap**
A celebratory closing screen with stars and a 3-point recap of the rule:
1. Check: same denominator?
2. Add the numerators.
3. Keep the denominator the same.

---

## Technologies Used

- **HTML5** — structures all six lesson screens/steps as a single page, using semantic elements and accessibility features (`aria-live`, `aria-label`, `role="progressbar"`, screen-reader-only text) so the lesson is usable with assistive technology.
- **CSS3** — handles all styling and animation, including:
  - Custom CSS variables for a consistent color palette and easy theming
  - **Conic gradients** to draw the circular pizzas (crust, slice dividers, and colored "eaten" wedges) without any external images
  - Keyframe animations for the floating pizza, button feedback (celebrate/wiggle), star bounce, and falling confetti
  - A `prefers-reduced-motion` media query so animations can be disabled for students who need it
  - Responsive layout (`clamp()`, media queries) so the widget works on both projector screens and smaller devices
- **Vanilla JavaScript (no frameworks or libraries)** — controls all interactivity:
  - Screen navigation (Next/Back), progress bar updates, and step labeling
  - Answer checking for multiple-choice questions and the fill-in-the-blank challenge, with pass/fail feedback messages
  - A `paintPizza()` function that dynamically draws each pizza's conic-gradient slices and colored wedges based on the numerator/denominator values passed in
  - A lightweight confetti effect generated and animated entirely in JS/CSS

The entire widget is a **single HTML file** with no build step, external dependencies, or internet connection required — it uses only system fonts (Trebuchet MS/Avenir Next) and native browser CSS/JS, so it can be opened directly in a browser or projected on a classroom screen without any setup.

