# campusmind-files

PDFs served from the CampusMind website at **https://www.campusmind.ai/files/&lt;file-name&gt;.pdf**.

This repo is a Webflow Cloud static app attached to the CampusMind Webflow site and mounted at `/files`. Every push to `main` deploys automatically, usually within a minute or two. It doesn't publish the Webflow site and doesn't touch any pages.

## Add or replace a PDF

1. Name the file in lowercase with hyphens and no spaces, for example `retention-agent-pricing.pdf`.
2. On GitHub, open this repo and click **Add file → Upload files**. Drop the PDF into the top folder, not into `.github`.
3. Click **Commit changes**.
4. After the deploy finishes, the PDF opens at `https://www.campusmind.ai/files/<file-name>.pdf`.

To replace a PDF, upload a new file with **exactly the same name**. The link stays the same, so links already in emails, decks and QR codes keep working.

Deleting or renaming a file breaks its link.

## Good to know

- Every file in the top folder is public at `/files/`. Don't upload drafts or internal files.
- `.github/` and `webflow.json` are never published.
- `index.html` sends anyone who opens `/files/` on its own to the Resources page.
- Accessible versions get the main name. Print versions end in `-print`.

## Current files

| Link | What it is |
|---|---|
| /files/pdf-accessibility-guide.pdf | PDF Accessibility Guide |
| /files/accessibility-agent-pricing.pdf | Accessibility Agent pricing brochure |
| /files/retention-agent-pricing.pdf | Retention Agent pricing brochure |
| /files/recruitment-agent-pricing.pdf | Recruitment Agent pricing brochure |
| /files/virtual-teaching-assistant-pricing.pdf | Virtual Teaching Assistant pricing brochure |
| /files/ai-studio-pricing.pdf | AI Studio pricing brochure |
| /files/campus-chat-plus-pricing.pdf | Campus Chat Plus pricing brochure |
| /files/data-bridge-pricing.pdf | Data Bridge pricing brochure |

Each pricing brochure also has a print version at the same name ending in `-print.pdf`, for example `/files/retention-agent-pricing-print.pdf`.
