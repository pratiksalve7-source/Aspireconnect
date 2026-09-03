# Aspire Connect — Vercel Website

A dependency-free, responsive 5-page website designed for GitHub + Vercel.
No Node.js, npm, React, or build step is required.

## Files
- index.html — Home
- services/index.html — What We Do
- industries/index.html — Industries
- about/index.html — About
- contact/index.html — Contact
- styles.css — shared design system
- vercel.json — clean URL configuration
- robots.txt
- sitemap.xml

## Deploy with GitHub + Vercel

### 1. Create GitHub repository
Go to GitHub and create a new repository, for example:
`aspire-connect`

Choose Private or Public as you prefer.

### 2. Upload these files
Upload the CONTENTS of this folder into the repository root.
The repository should look like:

aspire-connect/
  index.html
  styles.css
  vercel.json
  robots.txt
  sitemap.xml
  services/
    index.html
  industries/
    index.html
  about/
    index.html
  contact/
    index.html

Do NOT upload the ZIP inside the repository as the website itself.

### 3. Import into Vercel
1. Sign in to Vercel using GitHub.
2. Add New → Project.
3. Import the `aspire-connect` repository.
4. Framework Preset: Other / no framework.
5. Build Command: leave empty.
6. Output Directory: leave empty.
7. Deploy.

Vercel will give you a temporary `.vercel.app` URL. Test all five pages first.

### 4. Connect aspireconnect.in
In the Vercel project:
Project → Settings → Domains → Add Domain
Enter:
`aspireconnect.in`

Vercel will show the DNS records required for your GoDaddy domain.

### 5. Update GoDaddy DNS
In GoDaddy:
Domain → DNS / Manage DNS

Use ONLY the DNS records Vercel tells you to use. Do not delete email/MX records if you use the domain for email.

After DNS propagation, Vercel will automatically provision HTTPS.

## Important before launch
1. Replace the mailto contact form with a proper form service/CRM. The current form opens the visitor's email app and is fine for testing but not ideal for lead generation.
2. Add a Privacy Policy and Terms page before running serious advertising or collecting prospect data.
3. Add a professional email such as `pratik@aspireconnect.in`.
4. Add Google Search Console after the domain is live.
5. Consider adding dedicated landing pages:
   - /international-companies/ — EU/US companies looking for India
   - /indian-manufacturers/ — Indian companies seeking global business

## Updating the website later
Edit the relevant HTML/CSS files in GitHub and commit the change. Vercel automatically redeploys the site.

## Domain note
The GoDaddy domain can remain registered with GoDaddy. You do NOT need to transfer the domain to Vercel. You only point its DNS to Vercel.
