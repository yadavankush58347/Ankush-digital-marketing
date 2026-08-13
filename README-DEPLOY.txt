ANKUSH DIGITAL MARKETING — Deployment guide (Hostinger / cPanel / Apache / VPS)

WHAT'S INSIDE
  index.html          main page (SEO meta, Open Graph, Schema markup)
  404.html            custom error page (wired in .htaccess)
  .htaccess           HTTPS + www redirects, GZIP, caching, security headers, SPA rewrite, file protection
  manifest.json       PWA / mobile web app manifest
  robots.txt          crawler rules + sitemap reference
  sitemap.xml         XML sitemap
  favicon.png         site icon
  assets/             hashed CSS, JS, images (long-term cacheable)
  videos/             CGI / UGC / promo MP4 clips

UPLOAD STEPS (cPanel / Hostinger File Manager)
  1. Open File Manager -> public_html
  2. Upload ankush-digital-marketing-website.zip and click "Extract"
  3. Everything above must sit DIRECTLY inside public_html (not in a sub-folder)
  4. Settings -> enable "Show Hidden Files (dotfiles)" so .htaccess is visible
  5. Open your domain — done. No Node.js, no database required.

BEFORE GOING LIVE — replace the placeholder domain
  Search & replace "https://ankushdigitalmarketing.com" with your real domain in:
    index.html (canonical + og:url), sitemap.xml, robots.txt

NOTES
  - .htaccess forces HTTPS and redirects www -> non-www. If SSL is not installed yet,
    comment out the two "Force HTTPS" RewriteCond/RewriteRule lines until it is.
  - Contact form opens WhatsApp (+91 91024 56010) with a pre-filled message.
    Email: ay9480122@gmail.com
  - Fonts load from Google Fonts (Plus Jakarta Sans); everything else is self-hosted.
  - Submit sitemap.xml in Google Search Console after launch.
