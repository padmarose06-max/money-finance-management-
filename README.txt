MONEY FINANCE MANAGEMENT — FIREBASE CLOUD VERSION

1. Firebase Console > Authentication > Sign-in method: enable Email/Password.
2. Firebase Console > Authentication > Users > Add user. Enter your own email and a NEW STRONG password. Do NOT use 123456.
3. Firestore Database > Rules: paste the contents of firestore.rules and Publish.
4. Upload index.html to Netlify (put it inside a folder and deploy the folder, or zip the folder).
5. Firebase Authentication > Settings > Authorized domains: add your Netlify domain if needed.
6. Log in with the Firebase email and password. All devices signing in with an authorized account see the same data.

IMPORTANT: The rules allow ANY Firebase-authenticated account in this project to read/edit all customer records. Do not enable public registration; create only trusted accounts. For view-only sharing, separate roles and rules must be developed. The app uses one shared Firestore document, suitable for small datasets only (Firestore document size limit 1 MiB). Export JSON backups regularly. Old local browser data is NOT automatically migrated; use JSON Restore after login if you have a backup.
