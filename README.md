# Matt Roberts Music — Personal Website

Single-page portfolio site for Matt Roberts, a composer and music producer based in Southwest Florida. Dark cinematic aesthetic with gold accents, responsive design, and scroll animations.

## What's in here

- `index.html` — The entire site in one file (HTML + CSS + JS, no build step)
- Google Fonts loaded from CDN (Cormorant Garamond + Inter)
- YouTube embed for "The Return of Christ" ministry video
- Placeholder audio element ready for an MP3 upload
- Scroll-triggered fade-in animations via IntersectionObserver

## Adding the audio file

Open `index.html` and find the `<audio>` element. Uncomment the `<source>` tag and update the `src` to point to the hosted MP3:

```html
<source src="audio/inspirational-crescendo.mp3" type="audio/mpeg">
```

If self-hosting, drop the file in an `audio/` folder next to `index.html`.

## Deploying

### GitHub Pages
1. Create a repo (e.g. `matt-roberts-music`)
2. Push this folder to the `main` branch
3. Go to Settings → Pages → Source: `main` / root
4. Site goes live at `https://username.github.io/matt-roberts-music/`

### Netlify
1. Drag and drop the folder onto [app.netlify.com/drop](https://app.netlify.com/drop)
2. Done — get a `.netlify.app` URL instantly
3. Add a custom domain in site settings

### Vercel
1. `npx vercel` from this directory (or drag-drop at vercel.com)
2. Add custom domain in dashboard

### Custom domain
Point an A record or CNAME to whichever host you pick. Update the `og:url` meta tag in `index.html` to match.

## Contact info to update later
- Email is currently `matthew@potterhomes.com` — search and replace when he gets a dedicated music email
- Social links section has YouTube only; add more `<a>` elements as needed
