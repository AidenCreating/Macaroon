# To Do List Website

This is a 100% static download website for the Mac app **To Do List**.

The download buttons expect a file named `To Do List.dmg` beside `index.html`.
Use a DMG if you want the familiar Mac install window where users drag the app
into the Applications folder.

## Create the DMG

After exporting the Mac app, put `To Do List.app` in this folder and run:

```sh
./make-dmg.sh
```

That creates `To Do List.dmg` containing:

- `To Do List.app`
- an `Applications` shortcut

Users will open the DMG and drag `To Do List.app` onto `Applications`.

## How to publish on GitHub Pages

1. Put the generated `To Do List.dmg` file beside `index.html`.
2. Upload `index.html`, `style.css`, and `To Do List.dmg` to a GitHub repository.
3. Enable GitHub Pages for the repository in GitHub settings.
4. The website will then provide the download button for `To Do List.dmg`.

No backend, database, accounts, server-side code, or build tools are required.
