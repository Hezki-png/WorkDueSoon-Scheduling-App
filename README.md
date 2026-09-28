# WorkDueSoon — offline assignment & test tracker for iPhone

WorkDueSoon is a web app that installs to your iPhone home screen. After the first
install it opens like a normal app and works fully offline. You can add, edit
and complete items with no internet, and your list is saved on your phone.

## One-time setup (about 5 minutes, free, no Mac needed)

The files need to be put online **once** so Safari can install the app. After
that, the app runs from your phone without internet.

### Option A — GitHub Pages (free, permanent, can be done entirely on your iPhone)
1. Unzip this file (on iPhone: tap it in the **Files** app).
2. Go to **github.com** in Safari and create a free account.
3. Tap **+ → New repository**. Name it `workduesoon`, set it to **Public**, tap **Create repository**.
4. Tap **uploading an existing file**, then choose all 7 files from the unzipped folder:
   `index.html`, `sw.js`, `manifest.webmanifest`, `icon-180.png`, `icon-192.png`, `icon-512.png`, `README.md`.
   Tap **Commit changes**.
5. Open **Settings → Pages**. Under *Branch*, choose **main**, then **/ (root)**, then **Save**.
6. Wait about a minute. Your app will be at `https://YOUR-USERNAME.github.io/workduesoon/`.

### Option B — Netlify Drop (fastest from a Windows PC)
Go to **app.netlify.com/drop** and drag the unzipped WorkDueSoon folder onto the page. Create a
free account when asked so the site isn't deleted after an hour.

## Install on your iPhone
1. Open your app's link in **Safari**. It must be Safari, not Chrome.
2. Tap **Share ⬆︎ → Add to Home Screen → Add**.
3. Open **WorkDueSoon** from the home screen once while you're online. From then on
   it works offline.

Always open it from the home-screen icon, not the Safari tab. The home-screen app
keeps its own saved data.

## Using it
- **+** adds an assignment, test or other activity.
- The due date and time are separate boxes. Type into either one, or tap its icon for a
  drop-down calendar or time list.
  - Dates you can type: `10/3`, `Oct 3`, `3 October 2026`, `2026-10-03`, `tomorrow`, `fri`,
    `next monday`, `in 2 weeks`. Number order follows your phone's region (month/day in the US,
    day/month elsewhere).
  - Times you can type: `9pm`, `930pm`, `9:30 am`, `21:30`, `noon`, `midnight`.
- Items stay in Upcoming until you mark them done. Once the due time passes, an item moves
  to an **Overdue** section at the top, turns red, gets a red **DUE** tag and shows how long
  it's overdue (for example "Overdue by 2d 5h").
- Items are grouped by day. The countdown turns orange under 3 days and red under 24 hours.
- Tap the **circle** and it asks first: **Mark as done** moves the item to History, **Delete**
  removes it completely after a second confirmation, and **Cancel** leaves it alone.
- Tap an item to edit it, mark it done or delete it.
- **History** shows everything you've completed, labelled *On time* or *Late*. Tap an entry to see its
  details, move it back to Upcoming with a new due date, or delete it.
  **Clear History** at the bottom empties the list.
- Use the chips at the top to show all items, only assignments, only tests or only other.
- The **moon/sun button** switches between light and dark mode. **⋯ → Appearance** also has
  *Automatic*, which follows your iPhone's setting.
- **⋯ → Save backup file** exports your list. **Restore from backup** brings it back.
  Save a backup now and then, because deleting the app deletes its data.

## Limitations
- There are no push reminders. iPhone web apps can't schedule notifications offline.
- Data lives on this one phone and doesn't sync to other devices.

## Updating the app later
Replace the files on GitHub or Netlify, and change `duesoon-v1` in `sw.js` to
`duesoon-v2`. Open the app twice while online to pick up the new version.
