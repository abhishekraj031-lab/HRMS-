# HRMS prototypes

Two clickable, front-end-only prototypes. Plain HTML, CSS and JavaScript: no build step, no dependencies to install.

| Folder | What it is |
|---|---|
| `joining-checklist/` | Candidate pre-onboarding experience (desktop first, responsive). Invite email, OTP sign-in, welcome, checklist home, section pages with document upload states (uploaded, in review, needs changes, verified, adding later), all-submitted screen. Use the dark "Prototype" bar to jump between screens and switch Desktop/Mobile width. |
| `hrms-app/` | Mobile employee app "Kaveri People": punch in/out, leave balance, apply leave, leave calendar, salary slips with PDF download (jsPDF), profile. |

All names, companies and figures are sample data. Data you enter (punches, leave requests, uploads) is stored in your browser's localStorage only; uploaded files never leave the browser.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Publish with GitHub Pages

1. Push this folder to a GitHub repository (commands below).
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## External resources

- Fonts from Google Fonts (Albert Sans, Instrument Sans, IBM Plex Mono).
- `hrms-app` loads jsPDF 2.5.1 from cdnjs to generate payslip PDFs.
