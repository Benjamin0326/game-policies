# game-policies
Privacy policies for Benjamin0326 Dev games

## Tower Oops / 탑오정

The Korean and English pages are drafts awaiting Owner approval. Complete the
review below before pushing the policy to the public repository.

Expected GitHub Pages URLs after publication

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

- Confirm the legal data controller, Play developer display name, effective
  date, target audience, children's privacy and applicable legal notices.
- Confirm what information is handled, for which purposes and by whom,
  including support email and hosting. Confirm security measures, retention,
  deletion, privacy rights procedures and any applicable international transfers.
  The confirmed contact is `benjamin0326.dev@gmail.com`.
- Verify actual SDK initialization, identifier access and network activity in
  the release configuration. Align both policies with the verified SDK data
  collection, sharing, choices and safeguards, as well as Play Data safety,
  ads, content rating and target audience declarations. Google's disclosure
  covers the latest advertising SDK, so check the version in the release.
  [Google SDK disclosure](https://developers.google.com/admob/android/next-gen/privacy/play-data-disclosure)
- After reviewing both translations, replace all pending policy text with the
  approved details. Remove the draft notices and `noindex` tags from the Tower
  Oops pages in the same approved change before publishing.
  [Google Play User Data policy](https://support.google.com/googleplay/android-developer/answer/10144311)

## GitHub Pages

After approval, push the approved changes. In the repository's **Settings →
Pages**, use **Deploy from a branch**, `main` and `/(root)`.
[GitHub Pages publishing instructions](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

After deployment, test the two language URLs and the stylesheet over HTTPS in
a signed-out browser. Check the redirects, language navigation and indexing
headers. Use the verified policy URL in Play Console and the verified language
URLs in the app, then check the installed app's policy links.
