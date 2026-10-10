# Tushar Gosavi — Portfolio (cinematic edition)

One self-contained `index.html`. No build step. Dark, editorial design with a counting preloader,
giant animated name, line-by-line headline reveals, liquid hover on the experience cards,
an interactive "Selected work" selector, and smooth scrolling.

## Put it on GitHub Pages (free)

1. On github.com click **New repository**. Name it **`<your-username>.github.io`**, set it **Public**, create it.
2. **Add file → Upload files** and drag in `index.html`, `.nojekyll`, `README.md`
   and the `assets` folder (it holds your portrait). Click **Commit changes**.
3. **Settings → Pages → Build and deployment → Source: Deploy from a branch → main → / (root) → Save**.
4. After 1–2 minutes your site is live at `https://<your-username>.github.io`.

## Your portrait

Your cut-out portrait is already included as `assets/portrait.webp` (transparent background, about 70 KB).
Keep the `assets` folder next to `index.html` when you upload to GitHub. To swap it later, replace that file
with another transparent WebP or PNG of similar proportions (about 3:4, head and shoulders). If the file is
missing the page still works — the giant name simply stands alone.

## Before you publish

- **Selected work cards** (three projects on the school website): keep only what you're happy to claim publicly
  and reword to match what you actually did. They live in the `works` array near the bottom of `index.html`.
- **Numbers:** "4+ years", "3 organisations", "6 roles" come from your resume; "13 campuses" and the PageSpeed
  "35 to 55" come from the website work. Change any you can't stand behind.
- **Contact:** only your email is shown. Add LinkedIn/GitHub links by editing the footer if you like.

## Editing

- Colours, sizes and spacing are CSS variables at the top of the `<style>` block (`--accent`, `--background`, ...).
- Experience cards are the four `<li>` blocks under `#experience`.
- The scrolling words are the `words` array in the script.
- Fonts (Anton, Onest) and the smooth-scroll library load from the internet; if either is unavailable the page
  falls back to system fonts / normal scrolling.
- Visitors with "reduce motion" turned on get the page with animations switched off.
