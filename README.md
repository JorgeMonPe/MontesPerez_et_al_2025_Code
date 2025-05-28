# Reproduce this analysis

This repository contains the code to reproduce the results of the article: **Naturalization of Artificial Urban Ponds Alters Greenhouse Gas Dynamics - Montes-Pérez et al., 2025**.

The R Markdown file will automatically download the data from the [Environmental Data Initiative (EDI) repository](https://edirepository.org/).

If you prefer to download the data manually, you can access it here: [https://portal.edirepository.org/nis/mapbrowse?packageid=edi.1927.1](https://portal.edirepository.org/nis/mapbrowse?packageid=edi.1927.1)

## Requirements

- Install [R](https://cran.r-project.org/) (version 4.4.2 or higher).
- Install [RStudio](https://posit.co/download/rstudio/) (optional, but recommended).
- Git (optional, if you want to clone the repository).

## Download the repository

You can download the repository files in two ways:

### Option 1: Clone the repository
```bash
git clone https://github.com/user/repository-name.git
```

### Option 2: Download as a ZIP file
- Click the green **Code** button (top right).
- Select **Download ZIP** and extract the files on your computer.

##  Install dependencies

This project uses [`renv`](https://rstudio.github.io/renv/) for package management. Once you have downloaded the repository, follow these steps in R or RStudio:

```r
# Install renv if you don't have it yet
install.packages("renv")

# Activate the project environment and restore packages
renv::restore()
```

This will automatically install the exact package versions used in the project.

##  How to run the analysis

Once the environment is restored, you can run the main R Markdown file with:

```r
rmarkdown::render("MontesPerez_et_al_2025_Code.Rmd")
```

Alternatively, in RStudio:
1. Open the file `MontesPerez_et_al_2025_Code.Rmd`.
2. Click the **Knit** button to generate the full report.

## Output

The result will be an `.html` file with all the results, figures, and tables from the analysis.