# Prakash Prabhu — personal music website

A minimal, warm, responsive static site ready for GitHub Pages.

## Publish free on GitHub Pages

1. Create a public GitHub repository (e.g. `yourusername.github.io`).
2. Upload `index.html` and the entire `assets/` folder, preserving folder names.
3. In repository Settings → Pages, choose **Deploy from a branch**, `main`, root (`/`).
4. Wait for GitHub Pages to publish your site.
5. Optionally add your custom `.com` domain in Settings → Pages and configure the DNS records at Cloudflare according to GitHub's instructions.

## Activate the contact form (required)

The form is intentionally **not active** until you configure it. This prevents false claims of delivery.

1. Sign up at https://formspree.io/ and create a new form.
2. Set the form's recipient/notification email to your private inbox and verify it through Formspree.
3. Copy the form endpoint, shaped like `https://formspree.io/f/xxxxxxxx`.
4. Open `index.html`, find `REPLACE_WITH_YOUR_FORMSPREE_ENDPOINT`, and replace it with that endpoint.
5. Upload the updated `index.html` and submit a test message to verify email delivery.

**Privacy:** The recipient email is never included in this website's HTML, JavaScript, or visible content. Visitors inspecting the browser *will* see the public Formspree form endpoint, which is expected and does not reveal your recipient address. Your address is stored in Formspree's private dashboard. This is not a guarantee of complete anonymity: third-party service behavior, public domain records, or any information you publish elsewhere can disclose details. Enable Formspree spam protection as appropriate. Never embed secret API keys or email passwords in a static website.

## Add genuine reviews

In `index.html`, find `const REVIEWS = [];` and replace it with e.g.:

```js
const REVIEWS = [
  { quote: 'A wonderful performance!', name: 'Jane D.', detail: 'Private event' },
  { quote: 'The music made our night.', name: 'Alex M.', detail: 'Audience member' }
];
```

These are fictional examples for formatting only; publish only authentic reviews with permission. Until then the site shows “Audience and client reviews coming soon.”

## Photos

Photos are stored locally in `assets/`. You can swap them while retaining the same filenames. Motion effects respect visitors' reduced-motion preferences.

## Instagram
The Instagram links in the Contact section and footer point to https://www.instagram.com/unpluggedbyprakash/ and open in a new tab. The icon is inline SVG, so no external icon library is needed.

## Latest design update
- Original musical-note brand mark at top left.
- Artistic Cormorant Garamond display typography and prominent Prakash Prabhu hero name.
- Hero photo uses full-height containment on desktop and a separate portrait zone on mobile, avoiding the previous aggressive crop.
- Contact form requires a Formspree endpoint before email delivery works.

## Contact form configured

The contact form in `index.html` is configured with the Formspree endpoint:
`https://formspree.io/f/mppqdbwj`

In your Formspree dashboard, verify the form's notification recipient is
`contact@unpluggedbyprakash.com` (or your desired verified inbox).
Cloudflare routing can then forward it to your Gmail. Form submissions require
an internet connection and should be tested on the deployed website.
