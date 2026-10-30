# EyeSync website

This is the public [EyeSync](https://github.com/vexelbotrps-lgtm/EyeSync)
download website. It keeps the original visual style and browser face-tracking
demo, with direct Windows and developer downloads. The site is open source under
the [MIT License](LICENSE).

The Download page offers the latest Windows setup executable. Opening setup
installs EyeSync in the current user's app folder and creates an
**EyeSync** shortcut on the Desktop or in a chosen folder. Clicking
the shortcut starts nine-dot calibration on first launch, then opens the app.
The setup bundles Python 3.15.2 and does not need administrator rights.

Developers can download the application source ZIP from the same page. The
application's source and third-party notices are in the
[EyeSync repository](https://github.com/vexelbotrps-lgtm/EyeSync).

The Controls page lists all three face gestures, every supported voice-typing
editing phrase, and the six exact Command Panel phrases for the on-screen keyboard.

## Local preview

Run `python -m http.server 8000` in the repository root, then open
`http://localhost:8000/`. The site is static HTML, CSS and JavaScript.

## GitHub Pages

The workflow in `.github/workflows/pages.yml` publishes the site from the
repository root when `main` is pushed. `downloads/latest.json` names the
tested setup asset in the EyeSync GitHub Release, including its size. Update
that manifest after uploading a new release.

The optional browser demo needs camera permission and is separate from the
downloaded application. After installation, EyeSync runs without this website.
