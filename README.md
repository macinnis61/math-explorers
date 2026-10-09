# Math Explorers

A quiet, reusable toolkit for multiples, factors, prime factorization, GCF and LCM. Four tools live in one self-contained `index.html`. The identical file runs from GitHub Pages or from your computer. No build step, server, login, CDN, external fonts, analytics or student data. It uses Poppins when installed, with Arial as the offline fallback.

## Start offline

1. Extract the ZIP into a folder you can find on your classroom computer.
2. Double-click `index.html` and open it in Chrome, Firefox, Safari or Edge. If your computer opens a text editor, use **Open With → browser**.
3. Select a tool, enter your numbers, and use **Present** to hide navigation and teacher notes. The tool controls remain available. Escape or **Exit presentation** returns to the normal view. Browser full-screen is a separate command.
4. Test once with Wi-Fi off. Keep the local file available even when you usually use the hosted version.

The standalone `Math-Explorers.html` download is the same application under a descriptive filename. It needs no neighbouring files. Use `index.html` in the GitHub repository so its home URL works.

## GitHub Pages deployment

Suggested repository: `math-explorers` on your existing `macinnis61` account.

1. Sign in to GitHub and create a new public repository called `math-explorers`.
2. Upload **the contents** of this extracted folder into the repository root: `index.html`, `guide.html`, `README.md`, and `LICENSE.txt`. Do not upload only the ZIP or create an extra nested folder.
3. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Select **main**, **/(root)**, then **Save**.
4. Wait for GitHub to finish publishing; use the URL shown in Pages settings. For this account/repository, the expected URL is `https://macinnis61.github.io/math-explorers/`. It is a proposed address until you deploy.
5. Open each tool link below and check that the starting numbers are correct.
6. To update later, replace `index.html` in the same repository and commit. Keep the filename, repository name and tool route names unchanged so slide links continue to work. Refresh an open browser tab after deployment. Replace your offline copy separately.

Official instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

If using an existing Pages repository, place these files in a `math-explorers` folder within its published source. Your base URL will include that folder. Do not change the Pages settings of an existing site just for this tool.

## Stable slide links and placeholders

Use `{MATH_EXPLORERS_BASE}` as a planning placeholder for the published folder URL **including its trailing slash**. It is a token for us to replace when building slides, not a working URL and not an automatically resolved Google Slides variable.

| Slide / lesson | Placeholder link | What opens |
| --- | --- | --- |
| Multiplication Map launch / Practice 2-1 | `{MATH_EXPLORERS_BASE}#map?a=4&b=6` | Clean 12 × 12 map; markings hidden |
| Mirror facts | `{MATH_EXPLORERS_BASE}#map?a=4&b=6&mirrors=1` | Click a cell to show its mirrored fact and array |
| Common multiples / LCM | `{MATH_EXPLORERS_BASE}#multiples?a=4&b=6` | Blank number lines; step through before revealing |
| Factor pairs / prime factors | `{MATH_EXPLORERS_BASE}#tree?n=24` | Unsplit 24; choose factor pairs progressively |
| GCF / LCM connections | `{MATH_EXPLORERS_BASE}#factors?a=24&b=36` | Prime-factor comparison; GCF/LCM answers hidden |

Once deployed, replace the token with the actual base. Example:
`https://macinnis61.github.io/math-explorers/#factors?a=24&b=36`

In a future Google Slide, use a consistent button or text label such as **Explore: GCF & LCM**. Select it and use **Insert link** (Ctrl+K / Command+K), then paste the full published link. Click it during presentation, use the explorer in the browser, then switch back to your Slides tab. These are external interactives; they are not embedded executable HTML inside the slide.

Until deployment, put **INTERACTIVE LINK TO ADD: GCF & LCM / 24 and 36** in the slide's speaker notes. Do not hyperlink a made-up address. Our future slide builds can use the placeholders in their planning notes and substitute the live base once known. Keep the full route in the notes so it is easy to reconnect.

**Copy lesson link** in the toolkit generates a URL with the current numbers, map toggles and answer-reveal setting. Tree links return to the starting number, not a partly completed tree. Multiples links restart the sequence. Selected map cells are not saved. For a prediction slide, copy the link while results are hidden. When using the local copy, it generates a `file:` link, which works only for that computer's file location; use a hosted link for sharing.

## During an internet outage

Open the local file before class and keep it in a browser tab alongside your slides. If the online slide link fails, switch to that local tab, choose the tool and enter the same numbers. You can bookmark local tool routes on your own computer; they are not portable links for colleagues. The local explorer works offline regardless of whether the online copy has been opened before. Your slides need their own offline preparation; this package does not make Google Slides available offline.

## Classroom use: short teaching, substantial student work

These are demonstrations and investigations, not automatic full-block lesson plans. A useful cycle is **predict → explore → explain → practise**. Usually spend 5–10 minutes in the tool, then let students work. A factor-tree lesson may need longer guided instruction and its own practice block.

| Unit context | Demonstrate | Students then do |
| --- | --- | --- |
| Practice 2-1: multiples | Click 4 × 7; rotate the array mentally. Compare multiples of 4 and 6. | Generate multiples and find common multiples/LCM on their chosen practice level. Use one known-fact question from NS05 as retrieval if appropriate. |
| Practice 2-2: divisibility | Highlight products divisible by 2, 5 or 10. Use the map as pattern evidence. | Apply and explain rules on Practice 2-2. Teach digit-sum rules separately through place-value reasoning; the map alone does not prove them. |
| Practice 2-3: factors | Locate occurrences of 24 on the map; record row/column factor pairs separately. | Complete pairs and factor rainbows, then GCF practice. Explicitly include 1 × 24, outside the map. A selected NS07 equivalence question can reinforce multiplication relationships. |
| Shared prime-factor lesson / Practice 2-4 | Build 24 from 4 × 6, restart from 3 × 8, and compare final factors. | Build and check their own trees for 12, 18, 24 or 36. Use partly completed trees for support. All students encounter prime factorization. |
| GCF/LCM connections | Compare 24 and 36. Predict from the shared and unshared prime copies. | Solve and explain a few pairs; verify GCF with factor lists and LCM with multiple lists. Extend to prime-factor methods when ready. |

Ask: **What do you predict? What changed? What stayed the same? How can you check without this tool?** Keep permanent student-map annotations light; digital highlighting does not require students to colour every matching product.

## Mathematical conventions and limits

- Map: 1–12 in each direction. It highlights every displayed product divisible by either chosen number, rather than just its row. Sage = first; muted lavender = second; dark = both. If the two numbers match, their highlights are all shared. Square diagonal is an optional outline, not a permanent alteration.
- Map limits: the missing cell 1 × 24 is not a missing factor pair. The map does not establish primality for numbers outside its range.
- Trees: starting numbers 2–360. Only factor pairs greater than 1 are offered. Prime leaves are shaded. Restart to compare a different tree. **Finish tree** is a teacher shortcut; predict or construct first.
- Number lines: intervals 1–60. Each step adds one multiple to each sequence; it is not an animation of elapsed time. The display scales to include the LCM, so large coprime intervals can produce a dense display. Use smaller classroom examples such as 4/6, 6/8, 8/12 first.
- Prime-factor comparison: numbers 1–60. Repeated prime factors are matched one copy at a time. GCF multiplies shared copies; LCM multiplies all three regions, shared copies once. The empty product is 1. One has no prime factors and is neither prime nor composite.
- Student responses and progress are not recorded. Reopening a link returns to its starting configuration.

## Sharing

Share the hosted URL or the ZIP with colleagues. This package contains original code and teaching notes, with no copies of the source commercial practice sheets. Teachers use their own copies of those resources. The permissive licence covers this toolkit's code and notes.

## Product and factor-pair investigation

Find a product: select this highlighting mode and enter a target from 1 to 360. The map highlights every occurrence of that exact product. The complete factor-pair list includes pairs outside the grid; click a pair to see its array, then use Rotate array. For example, #map?highlight=product&target=24 opens this investigation directly. GCF and LCM instructions remain visible before Reveal results; the reveal displays the calculations.
