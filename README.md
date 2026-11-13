# From zero to engineer

A self-contained field guide to software engineering. Eleven levels, L0 to L10,
each with a first-principle thesis, six concepts, a three-rung practice ladder, a
capstone, a four-question self-graded gate and a reading list. One static HTML
file. No build step, no account, no backend.

## Deploy

Serve `index.html` from any static host.

- **Netlify / Vercel / Cloudflare Pages:** drag the folder onto the drop zone, or
  point the site at the directory. The build command is empty.
- **GitHub Pages:** push to a repository and enable Pages on the branch. The site
  is served from the repository root, so set the publish source to `/`.
- **Locally:** `python3 -m http.server 8000`, then open `http://localhost:8000/`.
  Opening the file directly also works.
- **Nginx / Apache:** copy `index.html` into the document root.

The page works with JavaScript off. All eleven levels and every reference stay
readable. Only progress tracking, gate grading and the spaced review queue need
JavaScript.

## How it teaches

The method cites its evidence in the sources section. In short:

- retrieval practice before any answer is revealed
- spaced review at 1, 3, 7, 14, 30, 60 and 120 days, interleaved across levels
- mastery gates at 80 percent, not time served
- worked example, then a faded example, then the cold task
- deliberate practice through one capstone per level
- predicted score against actual score, to correct overconfidence

Gates are self-graded. A pass means you were honest, not that a machine checked
you. Interleaved review and self-explanation carry moderate rather than high
evidence ratings in the literature, and are labelled as such on the page.

## Levels

| Act | Levels | Focus |
| --- | --- | --- |
| Ground | L0 to L2 | the machine, programming primitives, data and cost |
| Craft | L3 to L5 | abstraction, correctness, systems |
| Systems | L6 to L8 | persistent state, architecture, collaboration |
| Judgment | L9 to L10 | reliability and security, synthesis |

## Data

Progress, gate scores, predictions and review dates live in `localStorage` under
the key `se-ladder-v1` in the browser that saved them. Clear them with the
"Clear progress" control in the rail. Nothing leaves the device.

## Design

Editorial theme: uncoated stock paper, printed black ink, a condensed display
face over a serif reading face, square corners, a heavy ink rule over hairlines,
and one printer's green used as a signal. Fonts come from Google Fonts with
system fallbacks. The content is not readable without them, but it still works.

## Limits

Hour budgets are planning estimates, not measurements. The capstones require
real artefacts that this page cannot inspect. L10 is open ended, and mastery is a
practice rather than a certificate.
