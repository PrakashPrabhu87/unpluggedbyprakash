# Unplugged by Prakash — GitHub Pages website

## Upload to GitHub
Upload `index.html`, `reviews.json`, and the entire `assets/` folder to the **root** of your existing GitHub Pages repository. Keep your existing `CNAME` file if GitHub created one for your custom domain. Do not upload only the ZIP file.

## Add or change reviews without touching HTML
1. In GitHub, open `reviews.json` in the root of your repository.
2. Click the pencil icon (**Edit this file**).
3. Add another review object inside the square brackets, separated from the preceding object by a comma:

```json
{
  "name": "Customer name",
  "quote": "Their actual feedback goes here.",
  "detail": "Private event"
}
```

4. Click **Commit changes**. GitHub Pages will publish the updated reviews automatically. Refresh the website after deployment.

The file currently includes five **fictional sample reviews** for layout testing (Ajith, Deep, Shankar, Divya, Shikha). Each is labeled `Sample review — replace before publishing`. Replace them with genuine feedback and obtain permission to publish names. Do not present invented quotes as real testimonials.

**Tip:** JSON requires double quotes around keys and strings; no trailing comma after the final review.

## Contact form
The website is configured for Formspree endpoint `https://formspree.io/f/mppqdbwj`. Set your notification email in Formspree and test delivery.

## Local preview
The reviews load when the website is served over HTTP/HTTPS (including GitHub Pages). Double-clicking `index.html` directly on your computer (`file://`) may prevent loading `reviews.json` because of browser security rules.
