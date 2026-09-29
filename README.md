# 1828 Leaderboard

A public leaderboard page for the 1828 ambassadors. Anyone with the link can view it; no login needed.

- `index.html` is the page. Edit the point values for "How to earn points" in the `EVENTS` list near the top of its script.
- `standings.txt` holds the standings. This is the only file you change to update the leaderboard.

## One-time setup (VS Code)

1. Unzip this folder and open it in VS Code (File > Open Folder).
2. Open the Source Control panel (the branch icon on the left) and click **Publish to GitHub**.
   Sign in when VS Code asks, then choose **Publish to GitHub public repository**.
   (Free GitHub Pages needs a public repository.)
3. On github.com, open the new repository, then go to **Settings > Pages**.
   Under "Build and deployment", set Source to **Deploy from a branch**, Branch to **main**, folder **/ (root)**, and click **Save**.
4. After a minute or two the page shows your link, something like
   `https://YOUR-USERNAME.github.io/1828-leaderboard/`. Send that link out.

## Updating the standings

1. In Excel, select your standings rows (rank, name, points, tours) and copy.
2. In VS Code, open `standings.txt`, select everything, and paste over it. Save.
3. In Source Control, type a message like "Update standings", click **Commit**, then **Sync Changes**.
4. The live page updates within a minute or two. If someone still sees old numbers, a refresh fixes it.

Ranks are worked out from the points, so ties are handled automatically.
A nickname in parentheses, like "Oluwatobiloba (Tobi) Clinton", shows as "Tobi Clinton".

## Previewing on your computer

Double-clicking `index.html` won't load the standings, because browsers block pages opened from your
files from reading other files. Install the **Live Server** extension in VS Code, right-click
`index.html`, and choose **Open with Live Server**.
