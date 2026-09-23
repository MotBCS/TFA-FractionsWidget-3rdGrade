# Fraction Pizza Party

An interactive, 5-minute browser lesson that teaches basic fractions using pizza.

## Grade Level
3rd Grade

## Subject Area
Math

## Topic
Fractions — identifying and building fractions with equal parts (numerator and denominator)

## Learning Objective
By the end of this 5-minute lesson, the student will be able to:
- Explain that a fraction shows equal parts of one whole
- Identify the numerator (top number) as the parts you have, and the denominator (bottom number) as the total equal parts
- Read a fraction from a shaded pizza
- Build a given fraction by tapping the correct number of pizza slices (e.g., tap 3 of 6 slices to make 3/6)

## How the Lesson Is Structured
1. **Welcome** — introduces the pizza theme
2. **What Do These Numbers Mean?** — defines numerator and denominator
3. **Warm-up** — multiple-choice question
4. **Build a Fraction** — interactive
5. **Try It Yourself** — multiple choice question
6. **Your Turn** — interactive
7. **Recap** — reviews numerator, denominator, and equal parts

## Technologies Used
- **HTML5** — page structure and content
- **CSS3** — all styling and layout, including:
  - CSS custom properties (variables) for the color palette
  - `conic-gradient` and `repeating-conic-gradient` to draw the pizza slices without images
  - CSS animations for the floating pizza, confetti, and feedback pop-ins
  - Responsive layout with media queries for mobile screens
  - `prefers-reduced-motion` support for accessibility
- **Vanilla JavaScript (no frameworks or libraries)** — handles:
  - Slide navigation (Back / Next) and progress bar
  - Multiple-choice question checking and feedback
  - Tap-to-build pizza interactivity (converts a click's angle from the pizza's center into a slice index)
  - Answer-gated progression (Next is disabled until the question is answered correctly)
  - Confetti celebration on lesson completion

No build tools, servers, or external JavaScript libraries are required — the lesson runs entirely in the browser from `index.html` and `styles.css`.

## Files
- `index.html` — lesson content and behavior
- `styles.css` — visual design and layout