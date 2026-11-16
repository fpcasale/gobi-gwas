## install miniconda
https://docs.conda.io/en/latest/miniconda.html

## setup environment
```
conda create --name sysgen python=3.7
conda activate sysgen
conda install -y numpy scipy matplotlib pandas ipython scikit-learn statsmodels jupyterlab
pip install pandas-plink
pip install limix-lmm
```

## download data
* download https://www.dropbox.com/s/86fdj3i7ir3vap7/ALL.chr22_GRCh38.genotypes.20170504.zip?dl=0
* unzip files

## download notebooks and start tutorial part1
```
git clone https://github.com/fpcasale/gobi-gwas.git
cd gobi-gwas
cd notebooks
jupyter lab
```
## No Python on your laptop? Run the tutorial on Google Colab

For convenience, both notebooks are also available as Google Colab notebooks. Nothing has to be installed:
every notebook starts with a **Setup** cell that installs what is needed and downloads the data.

| Notebook | Open in Colab |
|---|---|
| 1 – Linear regression, LRT, power | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QuYftKfi5LjcRH-OiCaym6q3W3oSfScn) |
| 2 – GWAS on 1000 Genomes chr22 + GCTA | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1izU9V6HU7PT4cMVC3zm7FkooSaZRBxE6) |

1. Click the badge (you need a Google account).
2. **File → Save a copy in Drive**, so that your work is saved.
3. Run the Setup cell(s) at the top. Notebook 2 downloads the chromosome-22 data and the GCTA/PLINK
   binaries; this takes a few minutes the first time in a session.
4. Work through the notebook as usual. If Colab disconnects, just re-run the Setup cells.
