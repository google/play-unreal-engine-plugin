# Google Play Unreal Engine Plugin

> [!IMPORTANT]
> This plugin is for Android apps & games only.

This repository enables you to use the Google Play plugin in Unreal Engine.

This Google Play plugin provides C++ and Blueprint interfaces for accessing Google Play in-game features at runtime from within the Unreal Engine. The plugin streamlines the integration process of the Play features by using the Native SDK.

With this plugin, you can integrate one or more of the following features into your game:

- **Play Integrity & Licensing:** Check that your game is unmodified, installed by Google Play, and running on a genuine Android device (or a genuine instance of Google Play Games for PC). Your game’s backend server can respond when you detect risky traffic to prevent unauthorized access and cheating. Refer to the [documentation](https://developer.android.com/google/play/integrity) and [Runtime API reference](https://developer.android.com/reference/unreal-engine/play/core/group/play-integrity) for more information.
- **Play In-App Updates:** Prompt users to update to the latest version of your game, when a new version is available, without the user needing to visit the Play Store. Refer to the [documentation](https://developer.android.com/guide/playcore/in-app-updates/unreal-engine) and [Runtime API reference](https://developer.android.com/reference/unreal-engine/play/core/group/play-in-app-updates) for more information.
- **Play In-App Reviews:** Prompt users to submit Play Store ratings and reviews without leaving your game. Refer to the [documentation](https://developer.android.com/guide/playcore/in-app-review/unreal-engine) and [Runtime API reference](https://developer.android.com/reference/unreal-engine/play/core/group/play-in-app-reviews) for more information.

## Supported Unreal Engine versions
The plugin supports Unreal Engine 5.0 and all subsequent versions.

## Setup
1.  Copy the `GooglePlay` folder inside your `Plugins` folder in your Unreal
    Engine project.

2.  Open your **Unreal Engine** project and click **Edit → Plugins**.

3.  Search for **Google Play** and check the **Enabled** checkbox.

4.  Restart the game project and trigger a build.

5.  Open your project's `Build.cs` file and add the `{{ module_name }}` module
    to `PublicDependencyModuleNames`.

## Support

To request features or report issues with the plugin, please use the [GitHub issue tracker](https://github.com/google/play-unreal-engine-plugin/issues).

You can find more resources and support options in the official documentation for [Play Integrity API](https://developer.android.com/google/play/integrity/overview), [Play In-App Reviews](https://developer.android.com/guide/playcore/in-app-review) and [Play In-App Updates](https://developer.android.com/guide/playcore/in-app-updates).

## Data Collection

When you upload a game using this plugin to Google Play, Google collects the following data to help improve our products and services:

- Package name
- Version number
- Play Plugin version number

To opt-out of this data collection, remove the `.metadata.jar` files found under the `ThirdParty/play-core-native-sdk/tracking`.

> [!NOTE]
> This data collection is independent of Google’s collection of library dependencies declared in Gradle when you upload your game to Google Play.