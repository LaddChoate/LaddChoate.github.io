# Ladd Choate ePortfolio (Quarto + GitHub Pages)

## Before you publish, change these 4 things
1. **Headshot:** replace `resources/headshot.jpg` with your photo (keep the same file name).
2. **LinkedIn:** already set to linkedin.com/in/ladd-choate-550122430.
3. **Resume:** open `Ladd_Choate_Resume.docx`, fill in the yellow highlighted parts, remove the highlight, then
   File > Save As > PDF named `Ladd_Choate_Resume.pdf`, and put it in `resources/` (replace the old one).
4. **About text:** edit the paragraphs in `index.qmd` if you want.

## Publish
1. On github.com/new, create a **public** repo named exactly `LaddChoate.github.io`.
2. In RStudio: File > New Project > Version Control > Git, paste the repo URL, and create the project.
3. Copy everything in this folder into that project folder.
4. In RStudio's **Terminal** tab, run:
   ```
   quarto render
   git add .
   git commit -m "Publish ePortfolio"
   git push
   ```
5. On GitHub, open the repo and go to Settings > Pages. Set Source to "Deploy from a branch", Branch `main`, Folder `/docs`, and click Save.
6. After 1-2 minutes, your site is live at `https://LaddChoate.github.io`. Submit that link.

Any time you change something: run `quarto render`, then add, commit and push again.
