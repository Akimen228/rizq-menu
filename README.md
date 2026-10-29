# RIZQ menu
Plain HTML restaurant menu, ready for a static host or direct opening of `index.html`.
Run from the project root with Python 3.14, Pillow and Playwright already installed.
`python menu-site/make_images.py` rebuilds four optimised JPEGs from the original sources.
`python menu-site/qa.py` checks menu fidelity, page weight and layout in system Chrome.
Screenshots are saved in `menu-site/qa/phone.png` and `menu-site/qa/desktop.png`.
Google Fonts load at view time; serif and sans-serif fallbacks work offline.
GitHub Pages: run `gh repo create <name> --public --source menu-site --push`.
Then enable Pages in the repository settings from the `main` branch root.
Vercel: run `npx vercel --prod` from this folder; framework "Other", no build command.
Publish `index.html` and `img/`; Python scripts and QA screenshots are not needed on the host.
