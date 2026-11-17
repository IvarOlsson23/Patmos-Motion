# Patmos Motion

Motion guidelines for the Patmos design system, plus a prototype for trying the motion out in a real context.

| Path | Contents |
| --- | --- |
| `index.html` | Motion page for the brand portal: easing, durations, the four patterns, tokens, components, sections and page transitions |
| `prototype/index.html` | Prototype site (Home, Contact, Support) that uses the same motion |

Both pages are standalone HTML files with no build step. CSS and JavaScript are inline; only the fonts load from Google Fonts.

## View locally

Open `index.html` in a browser, or start a local server:

```sh
python3 -m http.server
```

Then go to http://localhost:8000.

## GitHub Pages

Settings → Pages → Deploy from a branch → `main` / root. The motion page is then the start page, and the prototype is at `/prototype/`.

## Motion tokens

```css
--ease-standard: cubic-bezier(0.75, 0.02, 0.5, 1);
--ease-enter:    cubic-bezier(0, 0, 0.5, 1);
--ease-exit:     cubic-bezier(0.75, 0.02, 1, 1);

--duration-short-1: 150ms;   /* State change */
--duration-short-2: 200ms;   /* Exit */
--duration-medium-1: 250ms;  /* Enter */
--duration-medium-2: 300ms;  /* Change in place */
--delay-short: 50ms;         /* Delay before content fades in */
```
