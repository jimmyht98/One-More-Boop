# One More Boop

A deliberately pointless, touch-friendly web app for iOS and Android. Tap the button, build short streaks, unlock color themes, and enjoy small celebrations for achieving absolutely nothing.

## Run locally

You need Node.js 22.13 or newer.

```bash
npm install
npm run dev
```

Open the local URL printed in the terminal, normally `http://localhost:3000`.

## Useful commands

```bash
npm run dev       # Start the development server
npm run build     # Create a production build
npm run lint      # Run the linter
npm run format    # Format the code
```

## Where to make changes

- `app/page.tsx` contains the app behavior, streak rules, unlocks, sound, haptics, dark mode, and interface markup.
- `app/globals.css` contains the complete light/dark theme, responsive layout, button glow, and celebration animations.
- `app/layout.tsx` contains the page title, description, and mobile app metadata.
- `public/manifest.webmanifest` controls the installable mobile web app details.
- `public/favicon.svg` is the app icon.

The app saves progress and preferences in the browser using `localStorage`. It does not need a database or account.

## Editing the rewards

The `skins` array near the top of `app/page.tsx` controls each collectible color, unlock requirement, and label. Streak celebrations currently trigger at 3 taps, 5 taps, and every 10 taps inside the `boop()` function.

## Restore the Git repository

If you received the `.bundle` file, clone it with:

```bash
git clone one-more-boop.git.bundle one-more-boop

cd one-more-boop
npm install
npm run dev
```
## Credits

Utilized GPT 5.6 Sol for creating this app, while also learning by doing diagnostics, fixing bugs, and implementing new things.
