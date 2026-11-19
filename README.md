# tsune-card-site

Link page for my NFC business card. Plain HTML, no build step.

## Before uploading: fill in 4 things
1. `index.html`: replace `PORTFOLIO_URL` with your portfolio link (e.g. your Framer site).
2. `index.html`: replace `LINKEDIN_URL` with your LinkedIn profile URL.
3. `index.html` and `contact.vcf`: replace `YOUR_DOMAIN` with your domain (e.g. `tsunemasa.com`).
4. Add your résumé to this folder, named exactly `resume.pdf`.

## Put it on GitHub
1. Go to github.com → **New repository** → name it `tsune-card-site` → **Public** → Create.
2. On the new repo page, click **uploading an existing file**.
3. Drag in everything from this folder (`index.html`, `contact.vcf`, `vercel.json`, `resume.pdf`, and the `assets` folder) → **Commit changes**.

## Deploy on Vercel
1. Go to vercel.com → sign up / log in **with GitHub**.
2. **Add New → Project** → pick `tsune-card-site` → **Deploy** (no settings to change).
3. You get a `*.vercel.app` link. Open it on your phone to check.

## Connect your domain
1. In the Vercel project: **Settings → Domains** → add your domain (and `www.` version).
2. Vercel shows DNS records (an `A` record and/or a `CNAME`). Add them at the company where you bought the domain.
3. Wait until Vercel shows **Valid Configuration** (minutes to a few hours). HTTPS is automatic.

## Write the NFC chip
- Write `https://YOUR_DOMAIN/card` to the chip (`/card` redirects to the home page, so you can point it elsewhere later without rewriting the chip).
- Test with an iPhone and an Android phone, then lock the chip.

## Keep it alive
- Domain: auto-renew ON, multi-year registration.
- Free uptime monitor (e.g. UptimeRobot) on `https://YOUR_DOMAIN/card`.
- To update the page later: edit the file on GitHub → Vercel redeploys automatically.
