# Lua IDE (Android)

A native Android app for writing and running Lua scripts on your phone:
- Syntax-highlighted code editor with line numbers
- Real Lua execution using LuaJ (no internet needed to run scripts)
- Console output panel
- Save/load multiple scripts on-device

## How to turn this into an APK (phone only, no PC)

1. **Create a free GitHub account** (github.com) if you don't have one.
2. **Create a new repository** (e.g. `lua-ide`), public or private, empty.
3. Using the GitHub app or mobile browser, **upload every file in this folder**,
   keeping the same folder structure (including the hidden `.github/workflows/build.yml`
   file — make sure it lands at that exact path).
4. Once uploaded, go to the **Actions** tab of your repo.
5. A workflow called **"Build APK"** will run automatically (takes ~2-4 minutes).
6. When it finishes (green checkmark), open the workflow run and scroll down to
   **Artifacts** → download **LuaIDE-debug-apk**.
7. Unzip that download — inside is `app-debug.apk`. Install it on your phone
   (you may need to allow "install unknown apps" for your browser/files app).

That's it — no compiling on-device, GitHub's servers do the build for you.

## Notes
- This is a debug build (unsigned, fine for personal use/testing).
- Scripts you write in the app are stored privately in the app's own storage.
- To rebuild after editing code, just push/upload changes again — Actions reruns automatically.
