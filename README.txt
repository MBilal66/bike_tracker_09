BIKE TRACKER PRO — PWA PACKAGE

This package uses the supplied Bike_Tracker_15 (1).html as its app source and adds:
- PWA manifest for an installable, standalone app experience
- Custom sporty racing-style 192px and 512px app icons
- Service worker for app-shell caching and basic same-origin offline loading

DEPLOY WITH GITHUB PAGES
1. Extract this ZIP.
2. Create or open a GitHub repository.
3. Upload all six files from this folder to the repository's publishing root.
4. In repository Settings > Pages, enable deployment from the main branch and root folder.
5. Open the published HTTPS URL in Chrome on Android.
6. Use Chrome's menu > Install app (or Add to Home screen, depending on version).

IMPORTANT LIMITATIONS
- Installability and service workers require HTTPS (localhost is also supported for testing).
- The app currently loads Google Fonts and the XLSX library from external CDNs. Those resources may not be available offline unless cached separately; basic app-shell files are cached.
- A PWA does not guarantee continuous GPS/trip recording while the screen is off. Android browser background restrictions may pause tracking. Reliable background tracking generally needs a native Android implementation with the appropriate location permissions and foreground service.
- The app's existing data is stored by its own browser origin. Moving from a local HTML file to a hosted PWA may not automatically transfer data; export/backup from the old version first if the app provides that option.
