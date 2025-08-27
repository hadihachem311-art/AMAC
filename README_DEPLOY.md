# Launch AMAC Website (Official)

This folder contains:
- `index.html`
- `robots.txt`, `sitemap.xml`
- `favicon.svg`
- `404.html`

## Deploy options
- **Netlify**: https://app.netlify.com/drop → drag this whole folder.
- **Vercel**: Import Project → drag/upload this folder or connect a GitHub repo.
- **GitHub Pages**: Push to a repo → Settings → Pages → deploy from branch.

All will give you HTTPS automatically.

## Connect your domain
1. Buy a domain (Cloudflare Registrar, Namecheap, etc.).
2. In your host, add your domain.
3. Update DNS at your registrar:
   - Root/apex (`your-domain.com`): follow host docs (A/ALIAS).
   - `www`: CNAME to your host (e.g., your-site.netlify.app).
4. Update `sitemap.xml`, `robots.txt`, and the canonical link in `index.html` from `https://your-domain.com` to your real domain.
5. Submit `https://YOUR-DOMAIN.com/sitemap.xml` to Google Search Console.

## Tips
- Convert large images to WebP/AVIF; add `loading="lazy"` for non-hero images.
- Add privacy policy/contact details for trust.
- Check performance with Lighthouse.
