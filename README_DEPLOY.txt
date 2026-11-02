TRANSWISATA SCHEDULE FIREBASE V27

1. Firebase Console -> transwisata-egr -> Build -> Firestore Database -> Create database (production mode).
2. Firestore -> Rules: paste firestore.rules and Publish.
3. Authentication -> Sign-in method -> enable Email/Password.
4. Authentication -> Users -> create user transwisataprimaops@gmail.com with your own strong password, and verify email (the rules require verified email).
5. Firestore -> Data -> after verified admin login, click Initialize Fleet to create six default aircraft in Firestore.
6. Hosting: upload index.html and icon/manifest files to GitHub Pages or Firebase Hosting over HTTPS.
7. Firebase API key is a public client config, not a secret. Firestore Rules protect writes.
8. This version synchronizes fleet data via Firestore, and admin email reminder settings via Firestore. Automatic email sending requires a separately deployed Cloud Function + scheduler and sender authorization.
9. Do not use a local file URL for full PWA features.
