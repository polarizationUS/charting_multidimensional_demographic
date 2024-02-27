# Charting multidimensional ideological polarization across demographic groups in the United States


### System requirements
The code is written in Python 3.10.12. The required packages and version numbers are:
- pandas -- 2.2.1
- numpy -- 1.26.4
- matplotlib -- 3.8.3
- seaborn -- 0.13.2
- scikit-learn -- 1.4.1.post1
- scipy -- 1.12.0
- networkx -- 3.2.1
- tqdm -- 4.64.1
- tabulate -- 0.9.0


### Installation guide
The results shown in the paper can be reproduced by running the jupyter notebooks found in the 'notebooks' folder. In order to avoid variable definition errors, we strongly recommend executing the notebooks' cells in order of appearance.


### Instructions for use
The work relies on the empirical surveys conducted by the American National Election Studes (ANES) in the years 1992, 2000, 2008, 2016, 2020. All the code is well-commented and described in detail. Besides the different Figures of the paper, the expected outputs vary depending on the notebook:

1. 'preprocessing.ipynb': we preprocess the ANES dataset collected in the file 'ANESdataset.csv' according to our purposes. Combining the data with the demographic information of respondents classified in 'demography.csv', the notebook generates the new file 'combineddata.csv'.
2. 'embedding.ipynb': we compute the low-dimensional embedding of the respondents' opinions. As a result, the file 'embeddingISOMAP.csv' is generated.
3. 'polarization.ipynb': we study the polarization across the demographic groups and the ideological trajectories in time. We also provide the numerical results obtained from the 2-dimensional Kolmogorov-Smirnov test and the null model.

All the csv files are located in the 'csvfiles' folder. Although most cells of the notebooks are executed in a very short times, the run time is shown for the most computationally expensive code.
