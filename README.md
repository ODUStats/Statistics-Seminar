# ODU Department Seminar Series website

This is a Quarto starter for a public seminar website hosted with GitHub Pages. It includes a current schedule, individual seminar pages, a searchable archive, responsive styling, and automatic publishing.

## 1. Create the GitHub repository

1. Sign in to the GitHub account you want to own the site.
2. Create a **public** repository named `odu-seminars`.
3. Upload all files and folders from this starter, including `.github`.
4. In `_quarto.yml`, replace `YOUR-USERNAME` in `site-url` with the GitHub username that owns the repository.
5. Commit the files to the `main` branch.

## 2. Enable GitHub Pages

1. Open the repository's **Settings**.
2. Select **Pages**.
3. Under **Build and deployment**, set **Source** to **GitHub Actions**.
4. Open the **Actions** tab and wait for “Publish Quarto website” to finish.

The website address will normally be:

`https://YOUR-USERNAME.github.io/odu-seminars/`

## 3. Add a seminar

1. Duplicate `seminars/2026-fall/2026-09-11-example.qmd`.
2. Rename it using `YYYY-MM-DD-short-title.qmd`.
3. Replace the title, speaker, date, time, location, abstract, bio, and materials.
4. Commit the file. GitHub will rebuild the website automatically.

Use ISO dates (`YYYY-MM-DD`) so seminars sort correctly. Do not publish reusable Zoom passcodes on a public site; use a registration link or distribute access details separately.

## 4. Begin a new semester

1. Create a folder such as `seminars/2027-spring/`.
2. Copy `_metadata.yml` into it.
3. Change `contents` in `schedule.qmd` and `index.qmd` to the new folder.
4. Add new seminar files there.

The archive searches all semester folders, so earlier talks remain available automatically.

## 5. Add collaborators

In the repository, open **Settings → Collaborators → Add people** and invite colleagues by GitHub username or email address. In a personal-account repository, collaborators can read and write the repository, but only the account owner has the owner role. For more granular roles and easier departmental handoff, the repository can later be transferred to a GitHub organization.

## Customize before launch

- Replace the site title and description in `_quarto.yml`.
- Replace organizer and visitor details in `about.qmd`.
- Replace the sample seminar entry.
- Adjust colors in `styles.css` if desired.
- Add a department-approved logo only after confirming its permitted use.

## Preview locally

Install Quarto, open a terminal in this folder, and run:

```bash
quarto preview
```

Press `Ctrl+C` when finished. To build the complete site without previewing, run `quarto render`.
