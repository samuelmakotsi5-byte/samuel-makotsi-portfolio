# Samuel Makotsi portfolio

A portfolio website for Samuel Makotsi, built with HTML, CSS, and JavaScript, with a Vercel-ready serverless contact form.

## Features
- Responsive dark portfolio website
- Project showcase and service cards
- WhatsApp, email, and GitHub contact links
- Contact form with client-side validation and mailto fallback
- Vercel serverless API endpoint for sending emails with SMTP

## Local preview

```bash
npm install
npx serve .
```

Then open the local URL shown in the terminal.

## Vercel deployment

1. Push this repo to GitHub.
2. Import the repo into Vercel.
3. Add environment variables in the Vercel dashboard:

```env
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_SECURE=false
SMTP_USER=your-email@gmail.com
SMTP_PASS=your-app-password
EMAIL_TO=samuelmakotsi5@gmail.com
```

4. Deploy the project.

## Notes
- If SMTP is not configured, the site still works and the form falls back to opening the visitor’s email client.
- The form posts to `/api/contact` on the deployed site.
