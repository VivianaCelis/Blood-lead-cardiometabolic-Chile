# Blood Lead and Cardiometabolic Markers in Chilean Adults

Code and results accompanying the article **“Association between blood lead concentration and cardiometabolic markers in Chilean adults: a cross-sectional study based on the 2016–2017 Chilean National Health Survey”**.

## Files

- **`ens2016_2017_pb_cardiometabolic_analysis.ipynb`**: notebook containing data preparation, statistical analyses, and table exports.
- **`resultsENS_Analysis_Tables.xlsx`**: reference results and software versions.
- **`LICENSE`**: code license.

## Data

Download the dataset from the [Department of Epidemiology, Chilean Ministry of Health](https://epi.minsal.cl/bases-de-datos/), selecting:

**“(a.2) Base Formulario 1-Formulario 2 y exámenes – Metales Pesados (SPSS)”**.

The data are not redistributed in this repository.

## Running in Google Colab

1. Download the `.ipynb` file from this repository.
2. Open [Google Colab](https://colab.research.google.com/) and select **File → Upload notebook**.
3. Run the cells in order, starting with dependency installation and imports.
4. When prompted, upload the `.sav` dataset or a ZIP containing a single `.sav` file.
5. Run through the final cell to download **`ENS_Analysis_Tables.xlsx`**.

The mixture analysis performs 200 bootstrap resamples per outcome and may take several minutes. The workbook included in this repository is named `resultsENS_Analysis_Tables.xlsx`.

## Reading the Results

The workbook contains a separate sheet for each analysis. `SBP` and `DBP` denote systolic and diastolic blood pressure (`PAS` and `PAD` in the code).

In the individual lead models, coefficients represent the estimated change associated with a doubling of blood lead concentration. The mixture analysis is exploratory and has a different interpretation, described in the notebook and article.

The **`Manuscript_Comparison`** sheet compares six core blood pressure results with manuscript reference values. A `True` indicates agreement at the reported rounding precision; this check does not assess all tables. **`Software_Versions`** records the versions used during execution.

## Citation and License

If you use the methods or findings of this work, please cite the associated article. The final bibliographic reference will be added when available.

The code is distributed under the MIT license. This license does not cover the dataset or manuscript.
