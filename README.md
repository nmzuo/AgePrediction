###### Description for the paper:　Gray Matter-Based Age Prediction Characterizes Different Regional Patterns
*Accepted by Neuroscience Bulletin (2020)*   </br>
By NM Zuo and TY Hu  </br>
Brainnetome Center & National Laboratory of Pattern Recognition  </br>
Institute of Automation, Chinese Academy of Science  </br>
Email: nmzuo@nlpr.ia.ac.cn  </br>
July, 2020  </br>


1. Run "Environment.m" first to addpath for MATLAB.
1. Directory "libPLS_1.98", "libsvm-weights-3.23", "ICC", "matlabTools" are libraries and some auxiliary functions, just ignore them if you are running Windows.
! If you want to run it on linux, perhaps you need to maually configure "libsvm-weights-3.23" first (see https://www.csie.ntu.edu.tw/~cjlin/libsvm/).
1. Directory "main": .m files are MATLAB scripts of our work, the main results can be obtained by running "Cam_vs_Cam_GM246_Age.m".
Directory "draw": The script "draw_weight.m" can draw weight pics using .nii.gz files, and the drawing process will produce some temporary files.
Directory "tifs": All the tif pics produced by MATLAB scripts will be stored here.
Directory "data": .mat files, .csv files and .txt files are data used in experiments.

Whole Directory:  </br>
├── Readme.txt </br>
├── Environment.m </br>
├── ICC </br>
├── libPLS_1.98 </br>
├── libsvm-weights-3.23 </br>
├── main </br>
│   ├── CamNKI_vs_CamNKI_GM246_Age.m  </br>
│   ├── Cam_vs_Cam_FA_Age.m  </br>
│   ├── Cam_vs_Cam_GM246_Age.m  </br>
│   ├── Cam_vs_Cam_GM246_AgeError_Intelligent_cv.m  </br>
│   ├── Cam_vs_Cam_GM246_Age_AAL3.m  </br>
│   ├── Cam_vs_Cam_GM246_Age_MorW.m  </br>
│   ├── Cam_vs_Cam_GM246_WM48_Age.m  </br>
│   ├── Cam_vs_Cam_GM246_WM48_MD_FA_Age.m  </br>
│   ├── Cam_vs_Cam_MD_Age.m  </br>
│   ├── Cam_vs_Cam_WM48_Age.m  </br>
│   ├── Cam_vs_NKI_GM246_Age.m  </br>
│   ├── data  </br>
│   │   ├── Cam_DWI_FA_2mm.mat  </br>
│   │   ├── Cam_DWI_MD_2mm.mat  </br>
│   │   ├── Cam_GM_AAL3.mat  </br>
│   │   ├── GM_1_246mean.mat  </br>
│   │   ├── ID_age.txt  </br>
│   │   ├── NKI_GM_1mm.mat  </br>
│   │   ├── NKI_T1_restCAP_matchCamCan.csv  </br>
│   │   ├── WM_1_48mean.mat  </br>
│   │   ├── recMat.mat  </br>
│   │   └── subj_list.txt  </br>
│   ├── draw  </br>
│   │   ├── BN_Atlas_246_1mm.nii.gz  </br>
│   │   ├── MNI152_T1_1mm_brain.nii.gz  </br>
│   │   ├── draw_weight.m  </br>
│   │   ├── raincloud.py  </br>
│   │   └── violin.mat  </br>
│   ├── mediation_AgeRes-Gender_gF.R  </br>
│   └── tifs  </br>
│   </br>
└── matlabTools  </br>

################ R language   </br>
The moderated mediation anlaysis was implemented by lavaan R-package  </br>

################ Python  </br>
The raincloud figure was plotted by Python main/draw/raincloud.py  </br>
