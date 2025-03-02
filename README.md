# Charting multidimensional ideological polarization across demographic groups in the United States


### System requirements
The code is written in Python 3.12.3. The required packages and version numbers are:
- pandas -- 2.2.3
- numpy -- 2.2.3
- matplotlib -- 3.10.0
- seaborn -- 0.13.2
- scikit-learn -- 1.6.1
- scipy -- 1.15.2
- networkx -- 3.4.2
- tqdm -- 4.67.1
- tabulate -- 0.9.0


### Installation guide
The results shown in the paper can be reproduced by running the jupyter notebooks found in the `notebooks` folder. In order to avoid variable definition errors, we strongly recommend executing the notebooks' cells in order of appearance.


### Instructions for use
The work relies on the empirical surveys conducted by the American National Election Studes (ANES) in the years 1992, 2000, 2008, 2016, and 2020. All the code is well-commented and described in detail. Besides the different Figures of the paper, the expected outputs vary depending on the notebook:

1. `preprocessing.ipynb`: We preprocess the ANES dataset collected in the file `ANESdataset.csv` according to our purposes. Combining the data with the demographic information of respondents classified in `demographics.csv`, the notebook generates the new file `combineddata.csv`.
2. `embedding.ipynb`: We compute the low-dimensional embedding of the respondents' opinions by implementing Isomap algorithm. As a result, the file `embeddingISOMAP.csv` is generated.
3. `polarization.ipynb`: We study the polarization across the demographic groups and the ideological trajectories in time. We also provide the numerical results obtained from the 2-dimensional Kolmogorov-Smirnov test and the null model.

All csv files are located in the `csvfiles` folder. Although most cells of the notebooks are executed in a very short times, the run time is shown for the most computationally expensive code.
