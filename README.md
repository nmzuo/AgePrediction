###### Description for the paper:　Gray Matter-Based Age Prediction Characterizes Different Regional Patterns
*Accepted by Neuroscience Bulletin (2020)*
By NM Zuo and TY Hu
Brainnetome Center & National Laboratory of Pattern Recognition
Institute of Automation, Chinese Academy of Science
Email: nmzuo@nlpr.ia.ac.cn
July, 2020


1. Run "Environment.m" first to addpath for MATLAB.
1. Directory "libPLS_1.98", "libsvm-weights-3.23", "ICC", "matlabTools" are libraries and some auxiliary functions, just ignore them if you are running Windows.
! If you want to run it on linux, perhaps you need to maually configure "libsvm-weights-3.23" first (see https://www.csie.ntu.edu.tw/~cjlin/libsvm/).
3. Directory "main": .m files are MATLAB scripts of our work, the main results can be obtained by running "Cam_vs_Cam_GM246_Age.m".
Directory "draw": The script "draw_weight.m" can draw weight pics using .nii.gz files, and the drawing process will produce some temporary files.
Directory "tifs": All the tif pics produced by MATLAB scripts will be stored here.
Directory "data": .mat files, .csv files and .txt files are data used in experiments.

> Whole Directory:
> ├── Readme.txt
> ├── Environment.m
> ├── ICC
> ├── libPLS_1.98
├── libsvm-weights-3.23
├── main
│   ├── CamNKI_vs_CamNKI_GM246_Age.m
│   ├── Cam_vs_Cam_FA_Age.m
│   ├── Cam_vs_Cam_GM246_Age.m
│   ├── Cam_vs_Cam_GM246_AgeError_Intelligent_cv.m
│   ├── Cam_vs_Cam_GM246_Age_AAL3.m
│   ├── Cam_vs_Cam_GM246_Age_MorW.m
│   ├── Cam_vs_Cam_GM246_WM48_Age.m
│   ├── Cam_vs_Cam_GM246_WM48_MD_FA_Age.m
│   ├── Cam_vs_Cam_MD_Age.m
│   ├── Cam_vs_Cam_WM48_Age.m
│   ├── Cam_vs_NKI_GM246_Age.m
│   ├── data
│   │   ├── Cam_DWI_FA_2mm.mat
│   │   ├── Cam_DWI_MD_2mm.mat
│   │   ├── Cam_GM_AAL3.mat
│   │   ├── GM_1_246mean.mat
│   │   ├── ID_age.txt
│   │   ├── NKI_GM_1mm.mat
│   │   ├── NKI_T1_restCAP_matchCamCan.csv
│   │   ├── WM_1_48mean.mat
│   │   ├── recMat.mat
│   │   └── subj_list.txt
│   ├── draw
│   │   ├── BN_Atlas_246_1mm.nii.gz
│   │   ├── MNI152_T1_1mm_brain.nii.gz
│   │   ├── draw_weight.m
│   │   ├── raincloud.py
│   │   └── violin.mat
│   ├── mediation_AgeRes-Gender_gF.R
│   └── tifs
│ 
└── matlabTools

################ R language
The moderated mediation anlaysis was implemented by lavaan R-package

################ Python
The raincloud figure was plotted by Python main/draw/raincloud.py
