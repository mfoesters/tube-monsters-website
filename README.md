# apps-website

Static site for Matthias Foesters' apps (GitHub Pages). Plain HTML/CSS: no cookies, no analytics, no external
scripts or fonts (Lilita One + Nunito are self-hosted, SIL OFL, licences in `assets/fonts/`).

| Path | File |
| --- | --- |
| `/` | `index.html` |
| `/tube-monsters/privacy/` | `tube-monsters/privacy/index.html` (English + Dutch) |
| `/tube-monsters/support/` | `tube-monsters/support/index.html` |
| `/app-ads.txt` | `app-ads.txt` (AdMob) |
| 404 | `404.html` (inline CSS; its "Go home" link is the full github.io URL: change it when you add a custom domain) |

Preview locally: `python3 -m http.server 5199` → http://localhost:5199

## To check / fill in

- [ ] **Custom domain**: none yet. When you have one, add a `CNAME` file containing just the domain
      (e.g. `apps.example.be`) and set it in repo Settings → Pages.
- [ ] **App Store link**: `index.html` has a disabled "Coming soon" button (search for `TODO`).
- [ ] **app-ads.txt**: line built from the publisher id in the AdMob app id (`pub-1732847173511258`) plus Google's
      standard certification id. Compare with AdMob → Apps → app-ads.txt → "How to set up app-ads.txt".
- [ ] Privacy policy, items marked `<!-- CHECK: … -->` in the HTML: GDPR legal bases, international-transfer wording,
      "ads not shown before the consent step", "English version prevails" line.
- [ ] Privacy policy: GDPR asks for the controller's identity + contact. Only name, country and email are listed.
      Decide if you want a postal address.
- [ ] Privacy policy, data list: check it against Google's AdMob "Data disclosure" page whenever the SDK is updated.
- [ ] Update the "Last updated" date whenever the policy changes.
