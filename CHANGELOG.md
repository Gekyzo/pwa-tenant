# Changelog

User-visible changes, newest first.

## Unreleased

- **Delete all data** in Settings › Backup, as in pwa-shopping-list (SET-2): `resetAll` in `src/storage.js` removes each `localStorage` key of the app, `<slug>.*`, and no key of another app of the origin; the page loads again as a new install. With a session the question says that it also logs out (`signedIn` of `src/ui/account.js`). Keys `settings.reset`, `reset.confirm`, `reset.confirmLocal`, `error.resetFailed`.

## 0.1.3 - 2026-10-29

- New app icon: a house with a bell and a calendar. `icons/source.png` is the new art (1254 px, converted to RGBA with its near-white background set to pure white); `npm run icons` wrote `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` and `logo.png` again. The shell cache is `pwa-tenant-shell-v3`, so installed apps fetch the new icons.

## 0.1.2 - 2026-10-25

- Google sign-in and the approval gate of the PocketBase server, with an offline choice, as in `pwa-wardrobe` (ACC-1 to ACC-10, `docs/spec/08-account.md`): `src/pocketbase.js`, `src/session.js`, `src/ui/account.js`. The app opens for an approved Google account or, after **Use offline**, with no account. Nothing syncs. Keys `pwa-tenant.session`, `pwa-tenant.offline` and `pwa-tenant.oauth` (`sessionStorage`). The shell cache is `pwa-tenant-shell-v2`.

## 0.1.1 - 2026-10-24

- First release, from pwa-template 0.1.2: offline shell, install, update toast, What's new, English and Spanish, light and dark themes. The notes demo stands in for the domain.
