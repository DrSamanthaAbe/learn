# learn.actuallysleeping.com — deploy in 15 minutes (nothing on ClickFunnels changes)

1. Cloudflare dashboard → Workers & Pages → Create → Pages → "Upload assets" → upload this `dist` folder. Project name: `learn-actuallysleeping`.
2. Custom domains → add `learn.actuallysleeping.com`. Cloudflare gives you a CNAME target.
3. Wherever actuallysleeping.com DNS lives: add CNAME `learn` → that target. (Adding a subdomain record does not touch www or the funnel.)
4. Bing Webmaster Tools → add site `learn.actuallysleeping.com` → verify via DNS TXT → submit `https://learn.actuallysleeping.com/sitemap.xml`. (ChatGPT search reads Bing.)
5. Google Search Console → add property → submit the same sitemap.
6. To update: edit `build.py`, run `python3 build.py`, re-upload `dist`.
