# Denmark wind and carbon-intensity computational essay

This repository is prepared for sharing the FYS10XX computational essay draft:

**Denmark: did more wind power show up as cleaner electricity?**

Open `index.html` locally for the static preview, or publish the repository with GitHub Pages.

## What is included

- `index.html` - readable static preview
- `FYS10XX_computational_essay_example_denmark_wind.ipynb` - executable notebook
- `data/` - local teaching subset and data dictionary
- `.github/workflows/deploy-pages.yml` - GitHub Actions workflow that reruns the notebook and rebuilds the plotted figure before publishing
- `.nojekyll` - tells GitHub Pages to serve the files as plain static files

## Publish with GitHub Pages

1. Create a new GitHub repository, for example `fys10xx-denmark-essay`.
2. Upload all files from this folder to the repository.
3. Go to **Settings -> Pages**.
4. Under **Build and deployment**, choose **GitHub Actions** as the source.
5. Go to **Actions** and run **Build and publish computational essay** if it does not run automatically.
6. Share the Pages link, usually:

`https://YOUR-USERNAME.github.io/fys10xx-denmark-essay/`

## Command-line upload option

Replace `YOUR-USERNAME` and the repository name before running:

```powershell
git init
git add .
git commit -m "Publish Denmark computational essay"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/fys10xx-denmark-essay.git
git push -u origin main
```

After the push, open the repository on GitHub and set **Settings -> Pages -> Build and deployment -> Source** to **GitHub Actions**.

## Why the workflow is included

GitHub Pages serves static files. It does not run Python by itself. The workflow solves that by installing the notebook requirements, executing the notebook, regenerating the figure, converting the executed notebook to HTML, and publishing that HTML with GitHub Pages.

## Data sources cited in the essay

- Our World in Data Energy: https://ourworldindata.org/energy
- OWID energy-data repository: https://github.com/owid/energy-data
- Full OWID Energy CSV: https://owid-public.owid.io/data/energy/owid-energy-data.csv
- OWID Energy codebook: https://raw.githubusercontent.com/owid/energy-data/master/owid-energy-codebook.csv
- Ember Yearly Electricity Data: https://ember-energy.org/data/yearly-electricity-data/

## Suggested message

Hi Anja,

I prepared a small computational essay draft for FYS10XX. It uses Denmark's electricity data from 2010-2024 to ask whether wind growth shows up together with lower electricity carbon intensity. I tried to keep it realistic for a 5-credit introductory course: one focused question, one dataset, one main figure, interpretation and limitations.

I would especially like feedback on whether the scope and style fit what we want students to work toward.
