# FamilyOS releases

Built artifacts for the FamilyOS desktop app (source lives in a private
repo).

## Fresh install

1. Download the `.dmg` from the [latest release](https://github.com/danielucas/family-os-releases/releases/latest) and drag **FamilyOS** to Applications.
2. The app is ad-hoc signed, so macOS quarantines browser downloads and
   reports the app as "damaged". Clear it once:

   ```sh
   xattr -dr com.apple.quarantine /Applications/FamilyOS.app
   ```

3. Open the app, point it at the household server, sign in.

## Updates

Installed apps update themselves: a toast appears at launch when a new
version exists, and Settings → About → "Check for updates" installs in
place (no quarantine, no terminal).
