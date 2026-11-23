Firebase consent-based live-location starter

1) Replace OWNER_UID in firebase-config.js and database.rules.json with YOUR dashboard account's Firebase Auth UID.
2) Deploy database.rules.json in Firebase Console > Realtime Database > Rules.
3) Put share.html, dashboard.html, firebase-config.js in your hosting folder (GitHub Pages supports module files).
4) Sender opens share.html, signs into their own account, reads recipient notice, checks consent, then taps Start sharing. Stop deletes the share record.
5) Dashboard owner signs into dashboard.html with their account.

Important: sender creates/controls their own account and credentials. This starter is a minimal example, not production-ready. Restrict permitted sender accounts further before production, add rate limiting/expiry and privacy controls, and test rules in Firebase Rules Playground. Sharing stops on page close/sign-out; explicit Stop deletes the current record.
