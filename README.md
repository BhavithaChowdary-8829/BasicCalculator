# Modern Calculator 🧮

A clean, responsive calculator built with plain HTML, CSS, and JavaScript — featuring a light/dark mode toggle and a Font Awesome icon-based button layout. No frameworks, no build step.

## Features

- **Basic arithmetic** — addition, subtraction, multiplication, division
- **Percent and decimal** support
- **Clear (C)** and **backspace** to fix mistakes
- **Dark / Light mode** toggle with a smooth animated switch
- **Responsive layout** — works on desktop and mobile screens
- **Error handling** — invalid expressions show `Error` instead of breaking
- **Icon-based buttons** using Font Awesome 6

## Demo

> Add a screenshot or a live link here once deployed.
>
> ```
> ![Calculator screenshot](screenshot.png)
> ```

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and button layout |
| CSS3 | Styling, CSS variables, theming, grid layout |
| JavaScript (Vanilla) | Calculator logic and theme switching |
| Font Awesome 6 | Operator and action icons |

## Project Structure

```
calculator/
├── index.html      # Markup: navbar, display, button grid
├── style.css       # Theme variables, layout, dark mode styles
├── script.js       # Input handling, calculation, theme toggle
└── profile.jpg     # Profile picture shown in the navbar
```

## Getting Started

### Option 1 — Open directly

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/calculator.git
   ```
2. Go into the folder:
   ```bash
   cd calculator
   ```
3. Open `index.html` in any browser.

### Option 2 — Run a local server (recommended)

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` in your browser.

## How It Works

- Each number and operator button calls `appendValue()`, which adds the character to the display.
- `calculate()` evaluates the expression and updates the display; if the expression is invalid, it shows `Error`.
- `clearDisplay()` resets the display to `0`, and `deleteLast()` removes the last entered character.
- The theme toggle adds or removes a `dark` class on `<body>`, and the CSS variables handle the rest.

## Deploying with GitHub Pages

1. Push the project to a GitHub repository.
2. Open **Settings → Pages**.
3. Under **Source**, choose the `main` branch and the `/root` folder.
4. Save — your calculator will be live at `https://your-username.github.io/calculator/`.

## Roadmap

- [ ] Keyboard input support
- [ ] Calculation history panel
- [ ] Replace `eval()` with a safe expression parser
- [ ] Remember the selected theme using `localStorage`
- [ ] Scientific functions (square root, power, parentheses)

## Contributing

Contributions are welcome. Fork the repo, create a branch for your change, and open a pull request.

---

Built by **Bhavitha**
