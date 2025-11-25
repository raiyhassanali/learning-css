# CSS Mini Exercise — Flexbox & Animations

This small exercise is a hands-on playground for practicing CSS layout and animations using a simple HTML page.

Files in this folder:

- `flex.html` — Example HTML page showing a heading and a `.container` holding several `.box` elements.
- `flex.css` — Styling for the page. Contains Flexbox layout rules, box styles and several CSS animations using @keyframes.

What I learned ✅

- How to link a stylesheet into an HTML page using `<link rel="stylesheet" href="flex.css">`.
- Flexbox basics: `display: flex;`, `flex-wrap`, `justify-content`, and how to arrange multiple items inside a container.
- Box model and spacing: `width`, `height`, `margin`, `border` and how these affect layout.
- Circle/oval shapes with `border-radius` and using `line-height` and `text-align` to center text vertically/horizontally.
- CSS animations:
  - Defining animation steps with `@keyframes`.
  - Playing with `transform` functions such as `rotate3d`, `translate`, `rotateX`, `rotateY`, `skewY`, and `scale`.
  - Controlling animation behaviour with `animation` shorthand: duration, timing-function (including `cubic-bezier()`), and `both` to preserve the final state.
  - Including `-webkit-` vendor-prefixed keyframes for broader compatibility.
- Practical debugging: using the browser dev tools to inspect computed styles (useful when you accidentally set `display` or `width` multiple times in a rule — the last defined property wins).

How to preview locally 🔧

- Open `c.html` directly in your browser.
- Or serve the folder with a simple HTTP server (works well for testing):

PowerShell (run in `d:\FSAI102\CSS`):

```powershell
# Start a simple Python http server on port 8000
python -m http.server 8000; # then open http://localhost:8000/c.html
```

OR if you have Node.js installed:

```powershell
# using npm package http-server (install once then run)
npx http-server -p 8000; # then open http://localhost:8000/c.html
```

How to push this repo to GitHub (example steps) ⬆️

1. Initialize a git repository (if not already):

```powershell
# only run once inside the folder
git init
git add .
git commit -m "Add CSS mini exercise: flexbox + animations"
```

2. Create a new GitHub repository using the GitHub UI and follow its instructions to add the remote, e.g.: 

```powershell
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

Notes and next steps 💡

- Try changing animation durations, delays or `cubic-bezier()` curves to learn how easing affects motion.
- Make the layout responsive by experimenting with different width units and media queries.
- Try refactoring duplicate rules and removing conflicting properties (e.g., avoid setting `display` twice in `.box`).

If you'd like, I can also:

- Add a short `index.html` to showcase the page or update the file to be responsive.
- Create a short demo GIF or add a deploy step for GitHub Pages.

Happy experimenting — great job exploring Flexbox and CSS animations! ✨
