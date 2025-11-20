# Required Images for Portfolio Site

This directory should contain the following images for optimal SEO and branding:

## Favicon Files
Place these favicon files in the `static` directory (one level up):

- **favicon.ico** (32x32px or 16x16px)
  - Classic favicon for browser tabs
  - Can be generated from a PNG using online tools like favicon.io

- **favicon-16x16.png** (16x16px)
  - Small size favicon for older browsers

- **favicon-32x32.png** (32x32px)
  - Standard size favicon

- **apple-touch-icon.png** (180x180px)
  - For iOS home screen bookmarks
  - Should have your logo/brand on a solid background

## Open Graph / Social Sharing Image

- **og-image.jpg** (1200x630px)
  - Used when sharing your site on Facebook, LinkedIn, Twitter
  - Should include:
    - Your name/brand
    - Tagline: "Expert Azure & Terraform DevOps Engineer"
    - Professional background matching site theme (#0B0F19)
    - High contrast text for readability
  - Referenced in `layouts/partials/head.html`

## Design Recommendations

- **Color scheme**: Match the site's dark theme (#0B0F19 background)
- **Brand colors**: Blue (#3b82f6) and Cyan (#06b6d4) gradient
- **Typography**: Use Inter or JetBrains Mono fonts if possible
- **Logo**: Consider a terminal/code icon to match the "DEVOPS.ARCHITECT" brand

## Quick Generation Tools

- **Favicon**: https://favicon.io or https://realfavicongenerator.net
- **OG Image**: https://www.canva.com (use 1200x630 template)
- **Icons**: https://fontawesome.com (already integrated in site)

## After Adding Images

Update `layouts/partials/head.html` to add favicon links:

```html
<link rel="icon" type="image/x-icon" href="/favicon.ico">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
```
