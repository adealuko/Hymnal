# Overcomers Hymnal: putting it on Android

This folder is the complete app. It works offline, and people can install it on their Android phones like any other app. You don't need to write any code. You only need to put these files online once, for free.

## What's in the folder

- `index.html` is the app itself.
- `manifest.webmanifest` gives Android the app's name, colors, and icon.
- `sw.js` lets the app open without an internet connection.
- `icons/` holds the app icons.

Keep all of these together. The app needs every file.

## Step 1: Put the app online with GitHub Pages (free)

1. Go to github.com and create a free account.
2. Select **New repository**. Name it `hymnal`, choose **Public**, and select **Create repository**.
3. On the next page, select **uploading an existing file**.
4. Unzip the folder on your computer, then drag everything inside it (`index.html`, `manifest.webmanifest`, `sw.js`, `README.md`, and the `icons` folder) into the upload box. Select **Commit changes**.
5. Open **Settings**, then **Pages**. Under **Branch**, choose `main` and select **Save**.
6. Wait a minute or two, then refresh. GitHub shows your app's address, which looks like `https://your-username.github.io/hymnal/`.

## Step 2: Install it on an Android phone

1. Open your app's address in **Chrome** on the phone.
2. Select **Install app** in the app, or open Chrome's menu (⋮) and choose **Install app** or **Add to Home screen**.
3. The Overcomers Hymnal icon appears on the home screen. It opens full screen and works offline after the first visit.

Share the address with your group by WhatsApp, text, or email so they can install it the same way.

## Step 3 (optional): Publish on the Google Play Store

1. Go to pwabuilder.com, paste your app's address, and select **Start**.
2. Select **Package for stores**, then **Android**, and download the package.
3. Create a Google Play Console developer account at play.google.com/console. Google charges a one-time registration fee.
4. Upload the package and complete the store listing. PWABuilder's download includes instructions for the final steps, including a small file (`assetlinks.json`) you add to your GitHub repository so the app opens without a browser address bar.

Before publishing publicly, check that every hymn in the app is in the public domain or that you have permission to publish it. The 37 built-in hymns are all public domain. A church CCLI license generally covers congregational use, not publishing lyrics in a public app.

## Updating the app later

Upload the new `index.html` to your repository, replacing the old one. Then open `sw.js`, change `hymnal-v1` to `hymnal-v2` (and so on each time), and upload it too. Phones get the update the next time they open the app with an internet connection.

## Good to know

Hymns and Yoruba versions added in this version are saved on each person's phone and are not shared with others. The claude.ai version of the hymnal still shares additions with your team. Syncing additions between phones would need an online database, such as a free Firebase account, which can be added later.
