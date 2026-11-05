# MySplitIt website

The website for **MySplitIt**, an Android app for splitting group expenses on trips and outings.

**Visit:** https://mysplitit.github.io

The site has:
- the features
- step-by-step guides
- a video walkthrough
- security and privacy details
- an FAQ
- a contact form

**Download the app:** [latest MySplitIt.apk](https://github.com/MySplitIt/mysplitit.github.io/releases/latest/download/MySplitIt.apk) (Android 8.0 or newer).

This repository holds the website and MySplitIt Web (the browser version). The Android app's source code is not published here.

## Files
- `index.html`: the main page.
- `privacy.html`: the privacy policy.
- `assets/`: styles, script, app icon, screenshots and the demo video.
- `app/`: **MySplitIt Web**, the browser version (https://mysplitit.github.io/app/). It signs in with Google and syncs live with the Android app through the same Firebase project. Access is enforced by Firestore security rules.
- `tests/`: checks that the web app splits money exactly like the Android app (`node --test tests/*.test.mjs`).

It's a static site with no build step, served by GitHub Pages from the `main` branch.
