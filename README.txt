We provide a set of 5 jupyter notebooks:

1 - ANN_JC_AA_n2v.ipynb
2 - LightGBM_JC_AA_n2v_no_omiss_links.ipynb
3 - LogReg_JC_AA.ipynb
4 - XGBoost_JC_AA_n2v.ipynb
5 - LightGBM_JC_AA_n2v_with_omiss_links.ipynb

Our models will run with a modified version of the dataset. The only difference is that we added the edges from the testing set that were not in the training set in the bottom of train.txt file (we did it by hard coding). We called the new file as train-mod.txt. The list of those edges can be found at the bottom of this readme file.

Jupyter notebook files need to be in the same folder as the modified dataset for the models to run.

All models contain an optimizer function for achieving the best parameters:

1 - ANN model uses Talos package for optimizing parameters. This model can be run from top to bottom with no need of changing parameters for obtaining results.

2 - LightGBM and XGBoost models use Optuna package for optimizing parameters. Cells of this model can be run up to the optimizing function. Once best parameters are obtained they need to be copied and pasted into the subsequent cell for the model to be trained with the best parameters.

3 - LogReg model uses GridSearchCV package for optimizing parameters. A similar process to the above step can be followed to run this model, as best parameters need to be fed into the model for training purposes.

After setting best parameters, all models are to produce a csv output file with AUC scores required for the Kaggle competition.

Each Jupyter notebook file contains a list of required packages at the first cell.

10 1864
321 2977
356 2259
358 1741
396 816
437 1902
462 3811
466 1897
497 747
619 2050
628 1590
664 3179
802 1394
998 4006
1079 2318
1103 3685
1221 2340
1236 2259
1278 2849
1318 1607
1368 3590
1458 3356
1465 2708
1543 3294
1566 2242
1590 3188
1716 1994
1739 1860
1792 3703
1803 1925
1803 2904
1929 3910
1951 3736
1993 2467
2004 3834
2085 2226
2141 2885
2175 3802
2211 3819
2380 2867
2611 3136
2625 3539
2879 3849
2885 3018
2957 3754
3045 3354
3205 3994
3487 3888
3629 3981
3674 3945
3811 3955