# Changelog

User-visible changes, newest first.

## Unreleased

No change.

## 0.1.2 - 2026-10-25

- Google sign-in and the approval gate of the PocketBase server, with an offline choice, as in `pwa-wardrobe` (ACC-1 to ACC-10, `docs/spec/08-account.md`): `src/pocketbase.js`, `src/session.js`, `src/ui/account.js`. The app opens for an approved Google account or, after **Use offline**, with no account. Nothing syncs. Keys `pwa-tenant.session`, `pwa-tenant.offline` and `pwa-tenant.oauth` (`sessionStorage`). The shell cache is `pwa-tenant-shell-v2`.

## 0.1.1 - 2026-10-24

- First release, from pwa-template 0.1.2: offline shell, install, update toast, What's new, English and Spanish, light and dark themes. The notes demo stands in for the domain.
