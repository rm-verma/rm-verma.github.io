# rm-verma.github.io

Personal academic site of **Ram Milan Kumar Verma** — Ph.D. research scholar,
Department of Aerospace Engineering, IIT Bombay.

Live at <https://rm-verma.github.io>

## Structure

    index.html      the entire site — self-contained, no build step
    404.html        styled not-found page
    cv.pdf          current CV (linked from the header and the contact section)
    .nojekyll       tells GitHub Pages to serve files as-is
    assets/         images

## Editing

Open `index.html` and edit it directly. There is no generator and nothing to
compile — commit and push, and GitHub Pages redeploys within a minute or two.

Colours live as custom properties on `:root` near the top of the file, with a
dark-mode block immediately below. Change them in one place and the whole page
follows.

## Adding images

Drop files into `assets/` using these names and aspect ratios:

| File               | Ratio | Used for                             |
|--------------------|-------|--------------------------------------|
| `portrait.jpg`     | 4:5   | portrait in the *Bearing* section    |
| `plate-1.jpg`      | 4:3   | Iron Fish UUV test bed               |
| `plate-2.jpg`      | 4:3   | USV on trial                         |
| `plate-3.jpg`      | 4:3   | fully actuated quadrotor             |
| `plate-4.jpg`      | 4:3   | JetBots in formation                 |

Then, in `index.html`, replace that slot's placeholder

```html
<div class="slot">…</div>
```

with

```html
<img src="assets/plate-1.jpg" alt="Iron Fish underwater vehicle test bed">
```

The surrounding frame, caption and rotation are already styled.

## Updating the CV

Replace `cv.pdf` at the repository root. Both links point at it, so nothing
else needs changing.
