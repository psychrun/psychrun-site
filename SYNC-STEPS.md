# psychrun.com — sync the new version

Seven files in this folder. Everything is done in the GitHub website; nothing to install.

## Step 1 — Upload (5 minutes)

1. Open github.com and go to your `psychrun-site` repository.
2. Click **Add file** (top right of the file list) → **Upload files**.
3. Drag all seven files onto the page:
   - index.html — the whole site (portrait, fuller experience, credentials section, SEO tags, analytics hook)
   - portrait.jpg — your photo, 360×360, shown above the headline
   - favicon.svg — browser tab icon
   - apple-touch-icon.png — home-screen icon on phones
   - og-image.png — preview card when the link is shared
   - robots.txt — search-engine permissions and sitemap pointer
   - sitemap.xml — page list for Google
4. Leave the commit message as is. Click **Commit changes**.

`index.html` replaces the old one because the name matches. `CNAME` is already in the repo — do not touch it.

## Step 2 — Check it (2 minutes)

1. Wait about two minutes.
2. Open https://psychrun.com and hard-refresh: Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac. On a phone, open it in a private tab.
3. You should see: the icon in the browser tab, your portrait above the headline, four roles under Experience, and a Credentials section before Contact.
4. If the old version still shows, wait another minute and refresh again. GitHub sometimes takes a moment.

## Step 3 — Share preview (2 minutes)

1. Go to https://www.linkedin.com/post-inspector/ and paste https://psychrun.com. This makes LinkedIn refresh its cached preview so the dark card appears when you share the link.
2. Optional: paste the link into a WhatsApp chat with yourself and confirm the card shows.

## Step 4 — Analytics (10 minutes, optional, any time)

1. Sign up at https://www.goatcounter.com. Pick a code such as `psychrun`.
2. In GitHub, open `index.html` → pencil icon. Use Ctrl+F to find `YOURCODE` and replace it with your code.
3. A few lines above that, delete the line beginning `<!-- Analytics: GoatCounter` and the two instruction lines under it; a few lines below the script tag, delete the line that is just `-->`. The script tag itself stays.
4. Commit changes. Visits appear at `psychrun.goatcounter.com` within a minute.

## Step 5 — Google Search Console (10 minutes, then wait a few days, optional)

1. Go to https://search.google.com/search-console, sign in with your psychrun.com Workspace account.
2. Add property → **Domain** → `psychrun.com`.
3. Copy the TXT record Google shows. Add it at your registrar's DNS: type TXT, host `@`, value as given. Save, wait a few minutes, click Verify.
4. Once verified: **Sitemaps** → enter `sitemap.xml` → Submit.
5. **URL Inspection** → `https://psychrun.com/` → **Request indexing**.

Searching your name should find the site within a week or so.

## Editing words later

Open `index.html` in GitHub → pencil icon → Ctrl+F for the sentence you want to change → edit → Commit. Live in about a minute. If a change breaks the layout, send me what you changed and I'll fix it.
