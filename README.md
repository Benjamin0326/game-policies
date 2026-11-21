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

The intended audience is **ages 13 and older**. Both drafts use the confirmed
privacy and support contact `benjamin0326.dev@gmail.com`. The published Play
listing should use that address as well. See the [T187 privacy review](tower-oops/release-privacy-review.md)
for the manifest and SDK evidence, regional requirements, and what belongs
in the policy and the Play Data safety form.

| Owner decision | What needs confirmation |
| --- | --- |
| Operator and public identity | Confirm the legal data controller, applicable privacy contact or officer details, and the Play developer display name. `Benjamin0326 Dev` is the proposed display name. |
| Distribution and children's privacy | Confirm country lists for closed testing and public release. Decide how each covered processing activity will handle minors, including verified legal-representative consent where legally required and the support process for players and their representatives. Confirm the Play age groups and applicable Families requirements using the game and listings. |
| Final release processing and Play declarations | Approve the SDK and permission configuration for submission after checking the final candidate's startup, identifier access and data flows. Confirm the separate Data safety, ads and Advertising ID declarations against those results. |
| Support records and rights requests | Confirm actual retention criteria, when the period starts, deletion timing and methods, exceptions, safeguards, and how privacy and deletion requests are verified, handled and answered. |
| Processors and international transfers | Confirm the legal bases, recipients and roles for email, hosting and SDK services. Identify applicable outsourcing or transfer disclosures, including the data, purposes, destinations, safeguards and retention. |
| Publication | Approve both languages, the actual effective date, the public HTTPS host and URLs. Resolve pending statements before removing the draft notices and `noindex` tags. The published policy must be accessible without login or geographic restrictions. [Play User Data policy](https://support.google.com/googleplay/android-developer/answer/10144311) |

## GitHub Pages

After approval, push the approved changes. In the repository's **Settings →
Pages**, use **Deploy from a branch**, `main` and `/(root)`.
[GitHub Pages publishing instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

After deployment, test the two language URLs and the stylesheet over HTTPS in
a signed-out browser. Check the redirects, language navigation and indexing
headers. Use the verified policy URL in Play Console and the verified language
URLs in the app, then check the installed app's policy links.
