# BaySiCel
Single Cell Data Imputation using Bayesian statistics and kNN
Author: Abhishek N. Singh

Project on Bayes Theorem Application in Single-Cell Gene expression data Imputation

Email: abhishek.narain@iitdalumni.com

Date: 24th December 2020

ScriptName: BaySiCel (pronounced: Bicycle ) - Bayes theorem based Single Cell data imputation

Description: The script is written in Python. It takes in data as CSV file with rows as different values of cells and columns as different values of expression of genes such as mRNA-seq. The cell names have header name as Cell. The user is 1st suppose to sort the column as per cell-type, such that, cells with similar types share similar names which is captured by keeping the 1st alphabet after period '.' as same letter. As an example, cells with Id VZA00602.A03 and VZA00602.A06 belong to the same batch and the cells are thus suppose to have similarity in identity such as derived from the same tissue. The script works by first conducting a Bayesian Posterior probability calculation wherever possible to impute the missing values. Thereafter, if there are still any missing values as shown by 0s are imputed using kNN algorithm. t-SNE 2-D plots are generated before and after the imputation that give a comparison of the impact of imputation.
