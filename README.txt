AT-PEN MAPPING FOR ANDROID

Option A: Install as an app from a web address (no Android Studio)
  1. Upload the contents of the "pwa" folder to any HTTPS host (GitHub Pages, Netlify, Cloudflare Pages).
  2. On the phone open that address in Chrome, allow Location, then menu > Install app (or Add to Home screen).
  GPS needs HTTPS, so it will not work from a file opened off the phone's storage.

Option B: Build an APK
  1. Install Android Studio. Choose File > Open and select the "android" folder.
  2. Let Gradle sync, then Build > Build APK(s). Or plug in the phone with USB debugging and press Run.
  3. The first launch asks for location permission. Exports go to the phone's Downloads folder.
  The app files are bundled inside the APK, so it works with no signal in the field.

MAP FILES
The app saves YARD_MAP.TXT in the same layout as the FI2 example: a comment header (feedyard, location, mapped by, mapped on), then one PEN line per pen with four corners.

SATELLITE VIEW AND GOOGLE EARTH
The Sat button on the map shows Esri World Imagery behind your pens. It needs an internet connection and
credits Esri on screen. Check Esri's terms if you use it commercially.
Save KML (Google Earth) on the Map file tab writes YARD_MAP.kml. Open it in Google Earth to see every pen
outline and bunk line on Google's imagery. This works offline.

UNITS
Distances show in feet by default. Switch to meters under Units on the Pens tab. Map files are not affected.
