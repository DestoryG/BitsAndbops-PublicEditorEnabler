# PublicEditorEnabler

A BepInEx plugin that unlocks the hidden **Custom Mixtape Editor** in the Steam public branch of *Bits & Bops*. This allows users to access the editor without switching to the potentially unstable beta branch.

## ⚠️ Disclaimer

* **Not an Official Product:** This plugin is an unofficial modification and is **not** affiliated with or endorsed by **Tempo Labs**.
* **Use at Your Own Risk:** Enabling hidden features may lead to game instability or save data corruption.
* **No Official Support:** **DO NOT contact Tempo Labs** regarding any issues or bugs encountered while using this plugin.

## 🛠️ How To Use

### Prerequisites

* **Option A:** Download and install [BepInEx 5.4.x](https://github.com/BepInEx/BepInEx/releases).
* **Option B:** If you have [Riqmenu](https://riqs.kabir.au/) installed, BepInEx is already set up for you.

### Installation

1. Download the latest `PublicEditorEnabler.dll` from the [Releases](https://github.com/DestoryG/BitsAndbops-PublicEditorEnabler/releases) page.
2. Place the DLL into the `BepInEx/plugins` folder.
3. Launch the game.

### Activation

1. Navigate to the **Credits** menu from the main screen.
2. Press **`Ctrl + E`** while the credits are open.
3. The game will now load the `MixtapeEditor` scene.

## 🔍 How it Works

The plugin uses **HarmonyX** to patch the `CreditsScript.Update()` method. It bypasses the `SteamManager.Beta` check, allowing the `SceneKey.MixtapeEditor` to be loaded in the public release.

## 📄 License

This project is licensed under the **MIT License**.

---
