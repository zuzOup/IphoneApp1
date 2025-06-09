

workflow :
1. expo -> npx expo start

than -> expo export:web 


i need pwa support :
app.json {
  "expo": {
    "web": {
      "favicon": "./assets/favicon.png",
      "manifest": {
        "name": "My App",
        "short_name": "App",
        "start_url": ".",
        "display": "standalone",
        "background_color": "#ffffff",
        "theme_color": "#000000"
      }
    }
  }
}
Also ensure you have:
service-worker.js automatically generated
Your browser supports PWAs (Safari)

Add to Home Screen on iPhone

Open Safari on your iPhone
Go to your app URL (e.g., https://my-app.vercel.app)
Tap the Share button (square with arrow)
Scroll down and tap Add to Home Screen
Give it a name and tap Add


 Tips for Better UX
 Add an icon.png in assets/ and reference it in the manifest
Use HTTPS (required for service workers and PWA install)
Configure offline.html or enable offline support via service workers if needed
