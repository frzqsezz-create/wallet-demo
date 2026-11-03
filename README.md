# Wallet Demo — iPhone Safari PWA

A fictional wallet simulator based on the original SwiftUI prototype. It does not connect to Apple Wallet, payment networks, banks, or Apple Pay.

## iPhone-only publishing with GitHub Pages (free)

1. In Safari, sign in or create an account at https://github.com .
2. Go to https://github.com/new and create a **Public** repository, for example `wallet-demo`. Do not put real financial information in it.
3. Download `WalletDemo-PWA.zip` from ChatGPT. Open the Files app, go to Downloads, and tap the ZIP to extract its folder.
4. Open your new repository on github.com in Safari. Tap **Add file → Upload files**. If the menu is hard to find, use Safari's **aA / page menu → Request Desktop Website**.
5. Upload all SIX files from *inside* the extracted `WalletDemo-PWA` folder, not the enclosing folder: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-180.png`, `icon-192.png`, and `icon-512.png`. The repository root must contain `index.html`. On iPhone, GitHub's file picker may require selecting the files one by one. Commit the changes.
6. In the repository, open **Settings → Pages** (may need desktop view). Under **Build and deployment**, choose **Deploy from a branch**; choose **main** and **/(root)**, then Save.
7. Wait a few minutes for publishing. Your URL will look like `https://YOUR-USERNAME.github.io/wallet-demo/` (use the exact URL GitHub Pages shows).
8. Open that URL in **Safari** on your iPhone. Tap **Share → Add to Home Screen → Add**. On some iOS versions you may need to scroll down the Share sheet. Choose **Open as Web App** if that option appears.
9. Open **Wallet Demo** from your Home Screen. Tap a card or swipe left/right to switch cards, tap **Simulate** to add a fictional purchase, or **Reset demo data** to restore initial balances.

## Notes

- GitHub Pages hosting requires a public repository on the free plan. **Anyone with the link can see the demo source**. No private information should be uploaded.
- Your fictional purchases are stored locally in your browser's localStorage; they are **not uploaded to GitHub**. Storage can be lost if Safari site data is cleared, or the app is reinstalled; Safari and Home Screen installations may have separate storage.
- The first visit requires internet; subsequent visits can work offline once the service worker finishes caching, subject to browser storage policies.
- This is a standalone website, not a native App Store app or Apple Wallet extension. It cannot make payments or add real payment cards.
- If the web app doesn't update after a new upload, close and reopen it or refresh Safari to pick up the updated cached version.

## Gold-style update
All three cards now use distinct metallic gold finishes. Existing local demo balances and transactions are preserved after replacing the site files. These are fictional gold-inspired cards, not American Express-issued cards.
