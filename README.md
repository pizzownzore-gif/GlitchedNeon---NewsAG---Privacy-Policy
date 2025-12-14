# NewsAG

NewsAG is a lightweight Android news reader app by GlitchedNeon. It displays news content and shows ads using Google AdMob. This repository contains the app source and a simple privacy policy you can host and link from your store listing.

Last updated: 2025-12-14  
Contact: pizzownzore@gmail.com

## Features
- Clean, minimal news reader UI
- Ad monetization via Google AdMob
- No sign-in required
- Does not collect personal data beyond standard advertising identifiers used by AdMob

## Privacy
A privacy policy is included as `privacy_policy.html` and `privacy_policy.md`. Host one of those files at a public HTTPS URL and add the URL to your Play Store / App Store listing.

If you need to host the policy quickly:
- GitHub Pages
  1. Create a public GitHub repository (or use this repo).
  2. Commit `privacy_policy.html` to the repository root (or to `docs/`).
  3. In the repository Settings → Pages, choose the branch and folder (`/ (root)` or `/docs`) and enable Pages.
  4. The policy will be available at: `https://<github-username>.github.io/<repo>/privacy_policy.html`

- Firebase Hosting
  1. Install Firebase CLI and run `firebase init hosting`.
  2. Place `privacy_policy.html` in the `public/` folder.
  3. Run `firebase deploy --only hosting` and use the provided HTTPS URL.

## Getting started (Android)
1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/<repo>.git
   cd <repo>
   ```

2. Open in Android Studio:
   - File → Open → select the project directory.

3. Configure AdMob:
   - Add your AdMob App ID to `AndroidManifest.xml` (replace the placeholder):
     ```xml
     <meta-data
       android:name="com.google.android.gms.ads.APPLICATION_ID"
       android:value="ca-app-pub-XXXXXXXXXXXXXXXX~YYYYYYYYYY"/>
     ```
   - Replace sample ad unit IDs in the code/layouts with your real ad unit IDs.

4. Build & Run:
   - Use a real device or emulator and Run the app from Android Studio.

Notes:
- Use test ad units while developing to avoid policy violations (see AdMob docs).
- Android Studio is the IDE used to develop the app; it is not a data-collection SDK.

## Project structure (example)
- app/                       — Android app module
- privacy_policy.html        — Ready-to-host HTML privacy policy
- privacy_policy.md          — Markdown privacy policy
- README.md                  — This file

## Privacy and compliance notes
- The app uses Google AdMob for advertising. AdMob may collect advertising identifiers, device and usage data, and approximate location to serve ads.
- The app does not require sign-in and does not collect personal data other than what AdMob may collect.
- You must link to the hosted privacy policy in your Play Store / App Store listing to comply with store requirements.

## Contributing
Contributions are welcome. Open an issue or submit a pull request with proposed changes.

## License
This project is licensed under the MIT License. See LICENSE for details.

## Contact
GlitchedNeon  
Email: pizzownzore@gmail.com
