# Step-by-step guide to share the essay on GitHub

## 1. Use the correct final folder

Use this folder:

`C:\Users\mamay\Documents\Codex\2026-06-21\f\outputs\github_pages_denmark_essay`

It contains:

- `index.html` - preview page
- `FYS10XX_computational_essay_example_denmark_wind.ipynb` - notebook
- `data/` - data files
- `requirements.txt` - Python packages for GitHub
- `.github/workflows/deploy-pages.yml` - workflow that reruns the notebook and rebuilds the figure

## 2. Create a GitHub repository

1. Go to https://github.com
2. Sign in.
3. Click the `+` button in the top right.
4. Click `New repository`.
5. Repository name: `fys10xx-denmark-essay`
6. Visibility: choose `Public` if you want GitHub Pages to work on a free account.
7. Do not worry if GitHub adds a README; the prepared folder already has one.
8. Click `Create repository`.

## 3. Upload the prepared files

1. Open the new repository on GitHub.
2. Click `Add file`.
3. Click `Upload files`.
4. Drag everything inside `github_pages_denmark_essay` into the upload area.
5. Make sure the upload includes `.github/workflows/deploy-pages.yml`.
6. Scroll down.
7. Commit message: `Publish Denmark computational essay`
8. Click `Commit changes`.

## 4. Enable GitHub Pages

1. In the repository, click `Settings`.
2. In the left sidebar, click `Pages`.
3. Under `Build and deployment`, choose `GitHub Actions`.
4. If GitHub asks you to confirm Pages, confirm it.

## 5. Run the workflow

1. Click the `Actions` tab.
2. Open `Build and publish computational essay`.
3. If it has not started, click `Run workflow`.
4. Wait until it has a green checkmark.

This workflow installs Python, reruns the notebook, rebuilds the plot, converts the notebook to HTML, and publishes the page.

## 6. Find the public link

1. Go back to `Settings`.
2. Click `Pages`.
3. Click `Visit site`.

The link should look like:

`https://YOUR-USERNAME.github.io/fys10xx-denmark-essay/`

## 7. Message to send Anja

Hi Anja,

I prepared a small computational essay draft for FYS10XX and published it here:

`PASTE-GITHUB-PAGES-LINK-HERE`

It uses Denmark's electricity data from 2010-2024 to ask whether wind growth shows up together with lower electricity carbon intensity. I tried to keep it realistic for a 5-credit introductory course: one focused question, one dataset, one main figure, interpretation and limitations.

I would especially like feedback on whether the scope and style fit what we want students to work toward.

Best,

`YOUR NAME`

## If GitHub Pages does not work

Use the zip file instead:

`C:\Users\mamay\Documents\Codex\2026-06-21\f\outputs\FYS10XX_github_pages_denmark_essay.zip`

Upload it to Google Drive or OneDrive and share the link.
