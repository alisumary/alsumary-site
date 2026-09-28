# alsumary.art

Your website. All text, links and photos live in `content/site.json`.
You never need to touch code — edit everything from the dashboard.

## Put it online (one time, ~20 minutes)

1. **GitHub** — make a free account at github.com. Click **New repository**, name it `alsumary-site`, set it **Public**, create it.
   Click **uploading an existing file**, drag in everything from this folder (including the hidden `.pages.yml` — on Mac press Cmd+Shift+. in Finder to see it), then **Commit changes**.
2. **Netlify** — make a free account at netlify.com (sign in with GitHub). **Add new site → Import an existing project → GitHub**,
   pick `alsumary-site`. Build command: *empty*. Publish directory: `.` Click **Deploy**.
   You get a test address like `something-12345.netlify.app`. Open it and check the site works.
3. **Domain (GoDaddy)** — in Netlify: **Domain management → Add a domain → `alsumary.art`**.
   Then in GoDaddy: **My Products → alsumary.art → DNS → Manage DNS**:
   - delete the parking records: the **A** record named `@` and the **CNAME** named `www`
   - add **A** — Name `@`, Value `75.2.60.5`, TTL 1 hour
   - add **CNAME** — Name `www`, Value `something-12345.netlify.app`
   Wait 10–60 minutes. Netlify adds free HTTPS by itself. Do NOT change the nameservers and do NOT use GoDaddy "Forwarding".

## Your dashboard

Open **app.pagescms.org**, sign in with GitHub, choose `alsumary-site`, then **My Website**.
Change anything → **Save**. The live site updates in about a minute.

- **Photos:** upload a photo, *or* paste a Google Drive link (file must be shared as "Anyone with the link").
  Uploading is faster and more reliable for your 6–8 selected photos.
- **Videos:** the site shows your latest YouTube uploads automatically. To show only your best,
  make a YouTube playlist and paste its ID, or paste single video links in *Featured videos*.
- Before uploading, export photos at about **2400 px wide, JPG quality 80** (under 1 MB each) so the site stays fast.
