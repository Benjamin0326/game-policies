# game-policies
Static privacy policies for games

## Tower Oops / 탑오정

The Korean and English pages are drafts awaiting Owner approval. Complete the
review below before pushing the policy to the public repository.

Proposed GitHub Pages URLs, pending deployment and verification

- [Korean](https://benjamin0326.github.io/game-policies/tower-oops/ko/)
- [English](https://benjamin0326.github.io/game-policies/tower-oops/en/)

The root `index.html` lists games. Each game has a directory named for its URL
slug, with an optional language selector, language subdirectories such as
`ko/index.html` and `en/index.html`, and its own assets. To add a game, create
its directory and add a relative link to the root list. Keep links between
pages relative so that they resolve under the GitHub Pages project path.
The root `.nojekyll` marker keeps the site build-free.

## Local preview

From the repository root, run `python3 -m http.server 8185 --bind 127.0.0.1`.
Open http://127.0.0.1:8185/ and follow the game and language links.

## Owner review before publication

### Policy decisions

| Owner confirmation | Proposed value or decision needed |
| --- | --- |
| Privacy and support contact | Use the confirmed address `benjamin0326.dev@gmail.com` in both policies and the Play listing. |
| Legal data controller | Confirm the legal name of the person or entity responsible for processing and any applicable contact or disclosure details. |
| Play developer display name | `Benjamin0326 Dev` is the T185/T187 proposal. Verify the exact name displayed in Play Console. |
| Effective date | Use the actual first public policy date, subject to Owner approval. |
| Target age groups | Select Play age groups based on the game and intended audience. |
| Children's privacy | Confirm how children's data is handled and which age or consent rules and Play Families requirements apply. [Google Play Families policies](https://support.google.com/googleplay/android-developer/answer/9893335) |
| Support retention and deletion | Confirm the retention period or criteria, when the period starts, deletion timing and methods, any exceptions, and the safeguards actually used. |
| Privacy rights | Use the confirmed email as the proposed request channel. Confirm applicable rights, how requests are verified and handled, and response timing. |
| Providers and international transfers | Confirm the roles of email, hosting and SDK providers. Identify any recipients or outsourced processors, what data they handle and why, and, where applicable, the destination, safeguards and required transfer disclosures. |

### Release evidence and Play Console

- The SDK inventory in T185's `docs/release/T185-play-policy-data-safety.md`
  identifies GMA Next-Gen 1.6.0 and UMP 4.0.0. T187 documents the SDK packaging
  and records AndroidX Startup and advertising identifier permission
  declarations in the manifest. The app's own SDK initialization, ad requests
  and UMP consent information updates are disabled in the reviewed candidate.
  Verify actual SDK initialization, identifier access and network activity in
  the final candidate, including on cold start. Use evidence for the included
  SDK versions and settings. Google's linked disclosure covers its latest SDK.
  [Google SDK disclosure](https://developers.google.com/admob/android/next-gen/privacy/play-data-disclosure)
- Check `allowBackup`, `fullBackupContent`, `dataExtractionRules` and the rules
  they reference in the final manifest. Verify which saves or settings are
  backed up or transferred and whether they return after reinstall or device
  migration. Update both policies with the verified result.
  [Android Auto Backup](https://developer.android.com/identity/data/autobackup)
- Use the verified release behavior to align both policies and Play Data safety
  on data access, collection, sharing, purposes, recipients, choices, security,
  retention and deletion. Confirm the ads declaration, Advertising ID, content
  rating and target audience in Play Console. T185 proposes reviewing **Yes**
  for the ads declaration first because the SDK and rewarded-ad UI are present.
  Leave that answer pending until the Owner verifies it against the candidate
  and Play guidance.
  [Google Play Data safety](https://support.google.com/googleplay/android-developer/answer/10787469)
  [Play Console app content](https://support.google.com/googleplay/android-developer/answer/9859455)
- Approve the same facts in both languages and resolve pending text. The
  approved publication change can then remove the draft notices and `noindex`
  tags from the Tower Oops pages. Verify that the final policy is available at a
  public HTTPS URL without login or geographic restrictions. Use the verified
  URL in Play Console and link to the policies in the installed app.
  [Google Play User Data policy](https://support.google.com/googleplay/android-developer/answer/10144311)

## GitHub Pages

After approval, push the approved changes. In the repository's **Settings →
Pages**, use **Deploy from a branch**, `main` and `/(root)`.
[GitHub Pages publishing instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

After deployment, test the two language URLs and the stylesheet over HTTPS in
a signed-out browser. Check the redirects, language navigation and indexing
headers. Use the verified policy URL in Play Console and the verified language
URLs in the app, then check the installed app's policy links.
