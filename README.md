# Avishi Mishra — Personal Brand Website (Self-Contained Version)

Every page (`index.html`, `about.html`, `content.html`, `press-kit.html`, `contact.html`) now has its CSS and JavaScript **built directly into the file** — there are no separate `css/style.css` or `js/script.js` files to link to anymore, so there's nothing that can go missing or 404.

The **only** folder this site still depends on is `images/`, holding the four photos. That folder worked correctly in your last upload, so the setup below should publish with zero broken links.

## Folder structure — must look exactly like this
```
Avishi-Mishra/              (your repo)
├── index.html
├── about.html
├── content.html
├── press-kit.html
├── contact.html
├── README.md
└── images/
    ├── selfie-candid.png
    ├── taj-portrait.png
    ├── campus-formal.png
    └── outdoor-formal.png
```

## How to upload (avoids the earlier issue)
1. Download and unzip `avishi-mishra-website.zip` on your computer.
2. Go to your GitHub repo → **Add file → Upload files**.
3. Drag in the 5 `.html` files and `README.md` **directly** (they sit at the root, no folder needed for these anymore).
4. Then drag in the entire `images` folder as one unit — most browsers support dragging a whole folder into GitHub's uploader and it will preserve the `images/` path automatically. If your browser doesn't support folder drag-and-drop, create the folder manually: click **Add file → Create new file**, type `images/selfie-candid.png` as the filename... actually, GitHub's web uploader doesn't accept image uploads through "create new file" (that's for text only) — so for images specifically, dragging the whole `images` folder (or each image one at a time while typing the path `images/filename.png` in the upload drop zone) is the reliable method.
5. Commit the changes.
6. Go to **Settings → Pages** → confirm **Source** is set to `Deploy from a branch`, branch `main`, folder `/ (root)`.
7. Give it 1–2 minutes, then hard-refresh your live URL (Ctrl+Shift+R / Cmd+Shift+R) — GitHub Pages caches aggressively, so a normal refresh sometimes still shows the old broken version right after a fix.

## If something still looks broken
Open the live site, press **F12** → **Network tab** → reload, and check for any red `404` entries. Since CSS/JS are now inline, the only thing that can 404 is a missing image — and if one does, the filename shown in the Network tab will tell you exactly which photo needs re-uploading.

## Notes carried over from the original build
- Social links point to the publicly listed YouTube (`youtube.com/@avishi`) and Instagram (`@avishimishh`) handles; the LinkedIn link is a placeholder (`#`) — replace with the real profile URL.
- The Contact page email is a placeholder — replace with a real inbox before actually using the form for outreach.
- Press-kit stats are intentionally qualitative rather than fabricated subscriber/engagement numbers, since that data isn't publicly available.
