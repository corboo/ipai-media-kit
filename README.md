# IPAI Media Kit

Advertiser-focused media kit for Inception Point AI.

## Live URL
https://corboo.github.io/ipai-media-kit/

## Updating Content

### Quick Stats Update
Edit the stats in `index.html` — find the `MEDIA_KIT_CONFIG` object at the bottom:

```javascript
const MEDIA_KIT_CONFIG = {
    stats: {
        shows: '5,000+',
        episodes: '200,000+',
        downloads: '13M+',
        monthly: '750K+'
    },
    // ...
};
```

### Full Content Update
1. Edit `index.html` directly
2. Commit and push to GitHub
3. Changes go live within minutes

## Visitor Tracking

### Built-in Tracking
The page stores visits to localStorage. To export:
1. Open the media kit in a browser
2. Open Developer Tools (F12)
3. In Console, run: `exportVisits()`

### Google Analytics
Replace `G-XXXXXXXXXX` in the `<head>` section with your actual GA4 property ID:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-YOUR-ID"></script>
<script>
    gtag('config', 'G-YOUR-ID');
</script>
```

## Data Source

Stats are derived from:
- Spreaker analytics (via Google Sheet)
- Source: https://docs.google.com/spreadsheets/d/1sNGZ03EeEtqqR4qgNmCpXgc4XebtUtjqCkctiax-uoA/

## Config Reference

See `config.json` for structured data that can be used to dynamically update the page via JavaScript.

## Branding

Current branding uses:
- Primary: `#4fc3f7` (cyan/teal)
- Accent: `#00e5ff` (bright cyan)
- Background: `#0a0a1a` (dark navy)
- Font: Inter

Update CSS variables in `:root` to change colors site-wide.
