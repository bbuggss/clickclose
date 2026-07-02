# ClickClose — your website (plain HTML/CSS/JS, yours to edit)

Editable code for your site. No Framer, no build tools, no lock-in.
Open any `.html` file in a browser to preview. Edit in any text editor (VS Code recommended).

## Files
- `index.html` — Home
- `services.html` — Services & pricing
- `demos.html` — Live demos: AI chatbot, booking, SEO preview, ROI calculator
- `about.html` — About
- `contact.html` — Contact (working form)
- `styles.css` — Reference copy of the design system (the styles are ALSO inlined
  into each HTML file, so each page renders on its own with no dependency)

## Live/interactive pieces
- **AI chatbot** (bottom-right, every page): answers from a built-in knowledge base —
  no API key, no cost. To upgrade to a real Claude-API bot later, see the comment at the
  top of the chat script in each file and route it through your own backend. Never put an
  API key in these files.
- **Booking** (demos.html): full flow that ends with a real .ics calendar invite + email.
- **SEO preview** (demos.html): live Google-result + checklist.
- **ROI calculator** (demos.html, section id="roisec"): to REMOVE it, delete the whole
  `<section id="roisec">...</section>` block. Nothing else depends on it.

## Make it yours before launch
- Replace `hello@clickclose.com` everywhere with your real inbox (find-and-replace).
- Swap the booking link / add a Calendly or GoHighLevel link where noted in contact.html.
- Replace the 3 placeholder testimonials on index.html with real ones.
- Set your real domain in the JSON-LD `url` in each file's <head> for SEO.

## Connect the contact form (optional)
Right now it opens the visitor's email pre-filled (zero setup). To auto-collect leads:
- Formspree: change the form to `action="https://formspree.io/f/yourID" method="POST"` and
  remove the JS submit handler.
- GoHighLevel: embed your GHL form or point the form action at your GHL webhook.

## Put it online (free)
1. Netlify Drop — drag this folder onto app.netlify.com/drop. Live in seconds.
2. GitHub Pages — push to a repo, enable Pages.
Both support a free custom domain.
