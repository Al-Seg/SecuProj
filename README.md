# CSI 4460/5460 — Network Scan Detection Website

A ready-to-upload, no-build website for the project **Detecting Network Scanning Activity Using Nmap and Wireshark**.

## Included files

- `index.html` — project homepage, timeline, research plan, and document links
- `proposal.html` — an editable proposal *draft* based on the selected project scope
- `styles.css` — all website styling; works on desktop and mobile

There is no package manager, framework, or deployment command. Open `index.html` to view locally.

## Publish with GitHub Pages (through the browser)

1. Sign into GitHub and create a new **public** repository, e.g. `network-scan-detection`.
2. Extract the ZIP. On your new repository's main page choose **Add file → Upload files**.
3. Upload **`index.html`, `proposal.html`, and `styles.css` into the repository ROOT** (not inside another nested directory). Commit the files.
4. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose the **main** branch and **/(root)** folder, then click **Save**.
6. Once GitHub reports that the site is live, open the published URL. The address will usually be `https://YOUR-USERNAME.github.io/network-scan-detection/`.
7. Test the proposal link, navigation, and mobile layout. Share the actual published URL in your course Google Sheet as requested.

**Important:** Upload the extracted individual files, not the ZIP itself. A public Pages site makes your name and documents publicly visible.

## Add your first progress report

1. Export your completed report to PDF (recommended for preserving formatting), for example `progress-report-1.pdf`.
2. Create a `docs` folder in the GitHub repository and upload it there (or use the repository root, and adjust the path).
3. In `index.html`, locate the block starting with:

   ```html
   <div class="doc-row pending"><span class="doc-symbol" aria-hidden="true">○</span><span class="doc-info"><strong>First progress report</strong>
   ```

4. Replace that entire block (through its matching `</div>`) with:

   ```html
   <a class="doc-row" href="docs/progress-report-1.pdf">
     <span class="doc-symbol" aria-hidden="true">↗</span>
     <span class="doc-info">
       <strong>First progress report</strong>
       <small>October 31, 2026</small>
     </span>
     <span class="doc-status available">View report</span>
     <span class="doc-arrow" aria-hidden="true">↗</span>
   </a>
   ```

5. Commit the change. Confirm the PDF link works on your public site. Do the same for later reports and slides.

**Alternative:** If you have the first report in Word, you can link a `.docx` file instead; PDF is easier for online readers.

## Before you publish

- Review the proposal draft in `proposal.html` to make sure it matches the proposal you actually submitted or the instructor approved. It is based on the project plan, not a recovered submitted proposal.
- The traffic chart is a CSS illustration, **not measured data**.
- The homepage deliberately lists future documents as "In preparation" or "Upcoming"; it does not link to nonexistent files.
- Update any milestones that change on Moodle or through professor announcements.
- Only run Nmap scans against systems you own or are explicitly authorized to test, preferably in an isolated lab.

## Editing the website

All site content is plain HTML. Open the file in VS Code or GitHub's built-in editor. Commit changes and GitHub Pages republishes the site. No server or extra software is required.
