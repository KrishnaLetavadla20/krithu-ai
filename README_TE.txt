KRITHU AI — Starter Prototype v0.1
==================================

ఈ మొదటి versionలో:
- తెలుగు text chat (rule-based demo; పూర్తి AI model కాదు)
- Browser support ఉంటే microphone speech recognition
- తెలుగు text-to-speech (deviceలో Telugu voice ఉంటే)
- Browser localStorageలో memory
- App తెరిచి ఉన్నప్పుడు reminders
- PWA manifest/service worker

ఇది ఏమీ చేయదు:
- మీ accountsలో login అవదు
- WhatsApp/YouTube/SMVJని access చేయదు
- App పూర్తిగా మూసివేసినప్పుడు reminders తప్పకుండా పంపదు
- ప్రస్తుతం ChatGPT/LLM APIకి కనెక్ట్ కాలేదు

Androidలో పరీక్ష:
1. ZIP extract చేయండి.
2. index.htmlని నేరుగా తెరిస్తే కొన్ని browser features పనిచేయకపోవచ్చు.
3. PWA install, service worker, microphone కోసం HTTPS hosting లేదా localhost అవసరం.
4. ఉచిత ఎంపిక: GitHubలో కొత్త repository సృష్టించి ఈ మూడు files (index.html, manifest.json, sw.js) upload చేయండి.
5. Repository Settings → Pages → Deploy from branch → main / root → Save.
6. GitHub Pages ఇచ్చిన HTTPS URLని Android Chromeలో తెరవండి.
7. Chrome menu → Add to Home screen / Install app.
8. Microphone అనుమతి ఇవ్వండి. Speech recognitionకు internet అవసరమవచ్చు.

Computerలో పరీక్ష:
- అదే HTTPS URL Chrome లేదా Edgeలో తెరవండి.
- Local testing కోసం Python install ఉంటే project folderలో terminal తెరిచి:
    python -m http.server 8000
  ఆపై http://localhost:8000 తెరవండి.

Privacy:
- Memory/reminders ఆ browser/device localStorageలోనే ఉంటాయి.
- Browser data clear చేస్తే అవి పోవచ్చు. Export buttonతో JSON backup తీసుకోండి.
- Shared/public computerలో వ్యక్తిగత సమాచారం save చేయకండి.

తర్వాతి అభివృద్ధి దశలు:
1. Real AI brain (local model లేదా API; ఖర్చు/పరికర సామర్థ్యం పరిశీలించాలి)
2. Backend + encrypted/synced memory
3. Reliable scheduled notifications/push
4. Android native features and permissions
5. SMVJ, EarnVerse Telugu కోసం ప్రత్యేక connectors — స్పష్టమైన అనుమతితో మాత్రమే.
