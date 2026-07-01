# Vhira — your website (plain HTML/CSS, yours to edit)

This is your full site as editable code. No Framer, no build tools, no lock-in.
Open any `.html` file in a browser to preview it. Edit in any text editor (VS Code is great).

## Files
- `index.html` — Home
- `services.html` — Services & pricing
- `about.html` — About
- `contact.html` — Contact (with working form)
- `styles.css` — All design/colors/fonts (edit once, applies to every page)

## Editing the basics
- **Colors & fonts:** top of `styles.css`, in the `:root` block. Change the hex values once.
- **Text:** just edit the words inside each `.html` file. The nav and footer are copied into
  every page — if you change a nav link, change it in all four files (search for `<nav` and `<footer`).
- **Email address:** replace `hello@vhira.co` everywhere (find-and-replace across all files).

## Making the contact form actually collect leads
Right now the form opens the visitor's email app with everything pre-filled — works with zero setup.
To collect submissions automatically, pick one:
- **Formspree (easiest):** create a form at formspree.io, then in `contact.html` change the form to
  `<form action="https://formspree.io/f/yourID" method="POST">` and delete the JS submit handler at the bottom.
- **GoHighLevel:** embed your GHL form, or point the form `action` at your GHL webhook.
- **Booking link:** in `contact.html`, replace the `mailto:` on the "Request a time" button with your
  Calendly or GoHighLevel scheduling link.

## Putting it online (free options)
1. **Netlify Drop** — go to app.netlify.com/drop and drag this whole folder in. Live in seconds.
2. **GitHub Pages** — push the folder to a repo, enable Pages in settings.
3. **Your own domain** — point it at whichever host above; both support custom domains free.

## Notes
- Fonts load from Google Fonts (Bricolage Grotesque + Inter) — needs internet on first load.
- Fully responsive, keyboard-accessible, and respects reduced-motion settings.
- The animated "signal ripple" in the hero is pure CSS — no images, nothing to break.
