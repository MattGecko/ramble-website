# Ramble Website

Official marketing website for Ramble - Voice Notes Reimagined.

## About

This is a simple, static website built with HTML and CSS, hosted on GitHub Pages.

## Pages

- **Home** (`index.html`) - Landing page with features and download CTAs
- **Privacy Policy** (`privacy.html`) - Privacy policy and data handling practices
- **Terms of Service** (`terms.html`) - Terms and conditions for using Ramble
- **Contact** (`contact.html`) - Contact form and support information

## Setup

### GitHub Pages Deployment

1. Go to repository Settings
2. Navigate to Pages section
3. Under "Source", select "Deploy from a branch"
4. Select "main" branch and "/ (root)" folder
5. Click Save

Your site will be available at: `https://[username].github.io/ramble-website/`

### Contact Form Setup

The contact form uses Formspree. To enable it:

1. Sign up at [Formspree.io](https://formspree.io)
2. Create a new form
3. Copy your form endpoint
4. Replace `YOUR_FORM_ID` in `contact.html` (line 23) with your actual form ID

Example:
```html
<form class="contact-form" action="https://formspree.io/f/xyzabc123" method="POST">
```

### Custom Domain (Optional)

To use a custom domain:

1. Add a `CNAME` file to the root directory with your domain name
2. Configure your DNS settings with your domain provider
3. Update the URLs in the app's `Constants.swift` file

## Local Development

Simply open `index.html` in a web browser, or use a local server:

```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server

# Then visit http://localhost:8000
```

## Updating Content

- **Colors**: Edit CSS variables in `style.css` (lines 6-11)
- **Features**: Update feature cards in `index.html`
- **Legal Pages**: Update `privacy.html` and `terms.html` as needed
- **Contact Email**: Update email addresses in `privacy.html`, `terms.html`, and `contact.html`

## License

© 2024 Ramble. All rights reserved.
