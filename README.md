# Steven's Travel Penang: channel website

A one-page website that shows every video from the YouTube channel and links each card to its video.
Channel: https://www.youtube.com/@stevenstravelpenang7832

## What is in this folder

- `index.html`: the website (this is the page GitHub shows)
- `images/`: one thumbnail per video, named by publish date
- `.nojekyll`: tells GitHub to serve the files as they are (keep it)

## Put it online with GitHub Pages (free)

1. Unzip the download. GitHub cannot read a zip, so you upload the files inside it.
2. Sign in at github.com and create a **New repository**. Choose **Public**. Name it anything, for example `stevens-travel-penang`.
3. On the new repository page, choose **uploading an existing file**. Drag in `index.html`, `.nojekyll` and the whole `images` folder, then **Commit changes**.
   - If `.nojekyll` is hidden on your computer, skip it. The site works without it.
4. Open the repository **Settings**, then **Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
5. Wait one to two minutes. Your site will be at `https://YOUR-GITHUB-USERNAME.github.io/REPOSITORY-NAME/`.
   - If you name the repository `YOUR-GITHUB-USERNAME.github.io`, the address is just `https://YOUR-GITHUB-USERNAME.github.io/`.

Put this link in your YouTube channel About section, video descriptions and social bios.

## Add a new video

1. Save the thumbnail in `images/` as `2026-10-20.jpg` (year-month-day). Use a 16:9 picture, around 760 px wide.
2. Open `index.html` and find the line that starts `var V=[`. Add your video at the very start of the list, newest first:
   `["20 Oct","YOUR_VIDEO_ID"],`
   The video ID is the part after `youtu.be/` in the share link. Use the same month spelling as the other entries: Oct, Sept, Aug, July, June. For a new month, also add it to the `M` list just above (for example `Nov:"November"`).
3. In the block that starts `var X=`, add one entry at the top:
   `"YOUR_VIDEO_ID": ["Your video title", "images/2026-10-20.jpg"],`
4. Upload the new image and the edited `index.html` to the repository. The newest video is shown big at the top automatically.

## Use your own domain (optional)

Buy a domain, then in **Settings > Pages** enter it under **Custom domain** and follow GitHub's DNS instructions.
