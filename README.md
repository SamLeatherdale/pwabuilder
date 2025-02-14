# PWA Builder

Builds Android Apps for websites that don't yet have a PWA.

# Add new app

To create a new app:

1. Generate a manifest. You can build one using the UI at [pwabuilder.com](https://www.pwabuilder.com/)
2. Host the manifest locally using `http-server` - required for the next step.
3. Create a new app using `bubblewrap init` - see package.json for examples
   1. Optionally create a higher quality vector icon for the app in a `drawable/ic_launcher.xml` file, and reference it in the `AndroidManifest.xml`
4. Build the app using `bubblewrap build`
5. Install the app using `adb install app-release-signed.apk` or `bubblewrap install`

To see a full list of available commands, check out [@bubblewrap/cli/src/lib/cmds/help.ts](https://github.com/GoogleChromeLabs/bubblewrap/blob/main/packages/cli/src/lib/cmds/help.ts)
