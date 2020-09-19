# Data License
Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012

This dataset is distributed AS-IS and no responsibility implied or explicit can be addressed to the authors or their institutions for its use or misuse. Any commercial use is prohibited.

Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, Davide Anguita. November 2012.

# Data Set Information
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

# Attribute Information:
For each record it is provided:
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.

# Variable list in `tidy_data.csv`
No |Column Name | Class | Range | Mean
|---|---			|---	  |---		|---   |
1 | PersonID | integer | 1  -  30 | Not available
2 | Activity | factor | LAYING, SITTING, STANDING, WALKING, WALKING_DOWNSTAIRS, WALKING_UPSTAIRS | Not available
3 | tBodyAcc-mean()-X | numeric | 0.242298449272727  -  0.279177960301325 | 0.273625706949098
4 | tBodyAcc-mean()-Y | numeric | -0.0316561370181818  -  -0.0144537072594949 | -0.0181506897285017
5 | tBodyAcc-mean()-Z | numeric | -0.118277180099383  -  -0.100985935692074 | -0.108983489335547
6 | tBodyAcc-std()-X | numeric | -0.99504124  -  0.0764832471304546 | -0.601304015955903
7 | tBodyAcc-std()-Y | numeric | -0.979413535862069  -  0.219952845181818 | -0.502368324101507
8 | tBodyAcc-std()-Z | numeric | -0.980976484137931  -  -0.0935184360181818 | -0.612658136083736
9 | tGravityAcc-mean()-X | numeric | 0.441236068541667  -  0.908399606896552 | 0.675087256248947
10 | tGravityAcc-mean()-Y | numeric | -0.350769156818182  -  0.2005691803125 | -0.0108779800499084
11 | tGravityAcc-mean()-Z | numeric | -0.278195591724138  -  0.266233413475819 | 0.0684117210693005
12 | tGravityAcc-std()-X | numeric | -0.993349445862069  -  -0.939673766818182 | -0.965289263871776
13 | tGravityAcc-std()-Y | numeric | -0.984760977241379  -  -0.901088770963325 | -0.954957188023449
14 | tGravityAcc-std()-Z | numeric | -0.98129168137931  -  -0.880682330706602 | -0.940102186573988
15 | tBodyAccJerk-mean()-X | numeric | 0.0686095366464646  -  0.105897183954545 | 0.0796709155688618
16 | tBodyAccJerk-mean()-Y | numeric | -0.00137201536971429  -  0.0320774996545455 | 0.00861445359001838
17 | tBodyAccJerk-mean()-Z | numeric | -0.0326983629140909  -  0.00364494866063107 | -0.00563142763570078
18 | tBodyAccJerk-std()-X | numeric | -0.994019934482759  -  0.0296014137090909 | -0.629710337628048
19 | tBodyAccJerk-std()-Y | numeric | -0.989158120689655  -  -0.0270976569090909 | -0.598078221055286
20 | tBodyAccJerk-std()-Z | numeric | -0.992004427241379  -  -0.444640860909091 | -0.761294256141813
21 | tBodyGyro-mean()-X | numeric | -0.0735291511680114  -  0.119614300727273 | -0.0271534683872472
22 | tBodyGyro-mean()-Y | numeric | -0.172162155445455  -  -0.0451436890589205 | -0.0767054085774151
23 | tBodyGyro-mean()-Z | numeric | -0.0046475084  -  0.109092913237986 | 0.085931620450104
24 | tBodyGyro-std()-X | numeric | -0.986979955517241  -  -0.377598602272727 | -0.717720720438609
25 | tBodyGyro-std()-Y | numeric | -0.985073170689655  -  -0.398959362766099 | -0.684230335974912
26 | tBodyGyro-std()-Z | numeric | -0.987937566551724  -  -0.1330599105 | -0.646846353814756
27 | tBodyGyroJerk-mean()-X | numeric | -0.119050870677727  -  -0.0731134377315625 | -0.0975868605682383
28 | tBodyGyroJerk-mean()-Y | numeric | -0.0593756069681818  -  -0.036876527389899 | -0.0428427061002085
29 | tBodyGyroJerk-mean()-Z | numeric | -0.0743422650272727  -  -0.0450693836894427 | -0.0555975269445795
30 | tBodyGyroJerk-std()-X | numeric | -0.991854138275862  -  -0.388955637727273 | -0.726931756997314
31 | tBodyGyroJerk-std()-Y | numeric | -0.993318104482759  -  -0.546043593651882 | -0.788013062813039
32 | tBodyGyroJerk-std()-Z | numeric | -0.993400307586207  -  -0.482172029090909 | -0.738597168075248
33 | tBodyAccMag-mean() | numeric | -0.985418968275862  -  0.194598717272727 | -0.541910425315789
34 | tBodyAccMag-std() | numeric | -0.986826527241379  -  -0.126888896863636 | -0.590709776501356
35 | tGravityAccMag-mean() | numeric | -0.985418968275862  -  0.194598717272727 | -0.541910425315789
36 | tGravityAccMag-std() | numeric | -0.986826527241379  -  -0.126888896863636 | -0.590709776501356
37 | tBodyAccJerkMag-mean() | numeric | -0.993245806206897  -  -0.0662072290227273 | -0.640904507249943
38 | tBodyAccJerkMag-std() | numeric | -0.993375015172414  -  -0.0363532663636364 | -0.620367369650529
39 | tBodyGyroMag-mean() | numeric | -0.983299607586207  -  -0.137333612554545 | -0.601557135632019
40 | tBodyGyroMag-std() | numeric | -0.981656969655172  -  -0.223751816518182 | -0.659833869530928
41 | tBodyGyroJerkMag-mean() | numeric | -0.994309820689655  -  -0.543885972272727 | -0.761445206305087
42 | tBodyGyroJerkMag-std() | numeric | -0.993276945862069  -  -0.573942888021613 | -0.780120455964607
43 | fBodyAcc-mean()-X | numeric | -0.994496322758621  -  -0.0414589456 | -0.616877881535588
44 | fBodyAcc-mean()-Y | numeric | -0.982367664137931  -  0.1231057773 | -0.529018110685255
45 | fBodyAcc-mean()-Z | numeric | -0.986495766206897  -  -0.198565773954545 | -0.663084795758664
46 | fBodyAcc-std()-X | numeric | -0.995250992758621  -  0.118339545340909 | -0.596658882741489
47 | fBodyAcc-std()-Y | numeric | -0.97835155862069  -  0.190673821868182 | -0.521377857526298
48 | fBodyAcc-std()-Z | numeric | -0.978759603793103  -  -0.1092913705 | -0.618103020546736
49 | fBodyAcc-meanFreq()-X | numeric | -0.319171141631269  -  -0.0209428055310345 | -0.209585252501383
50 | fBodyAcc-meanFreq()-Y | numeric | -0.15308350824613  -  0.128076957523023 | 0.0207348620212164
51 | fBodyAcc-meanFreq()-Z | numeric | -0.107844299474303  -  0.286965877634375 | 0.054742009569413
52 | fBodyAccJerk-mean()-X | numeric | -0.994117062068966  -  0.00774466264545455 | -0.646034358271534
53 | fBodyAccJerk-mean()-Y | numeric | -0.988820999655172  -  -0.042898966 | -0.618868327382891
54 | fBodyAccJerk-mean()-Z | numeric | -0.990597965172414  -  -0.38815349 | -0.741256896448463
55 | fBodyAccJerk-std()-X | numeric | -0.994459398275862  -  -0.0416593402068182 | -0.64647531373603
56 | fBodyAccJerk-std()-Y | numeric | -0.990414811034483  -  -0.0801154312545455 | -0.603353645905551
57 | fBodyAccJerk-std()-Z | numeric | -0.991935782413793  -  -0.500476129545455 | -0.780236495225755
58 | fBodyAccJerk-meanFreq()-X | numeric | -0.219176266215278  -  0.263820488655172 | -0.0300021463839075
59 | fBodyAccJerk-meanFreq()-Y | numeric | -0.347751351072054  -  0.108166523701034 | -0.201036260647769
60 | fBodyAccJerk-meanFreq()-Z | numeric | -0.290292303180208  -  0.129477226520833 | -0.112248557272945
61 | fBodyGyro-mean()-X | numeric | -0.985993540344828  -  -0.237124032272727 | -0.666637824815972
62 | fBodyGyro-mean()-Y | numeric | -0.987392253103448  -  -0.477139862384066 | -0.7069082167591
63 | fBodyGyro-mean()-Z | numeric | -0.988668107931034  -  -0.158548504727273 | -0.638376232316396
64 | fBodyGyro-std()-X | numeric | -0.987354722068966  -  -0.423153909545455 | -0.73562095976471
65 | fBodyGyro-std()-Y | numeric | -0.98380969137931  -  -0.348864187370186 | -0.676065261163996
66 | fBodyGyro-std()-Z | numeric | -0.988732922758621  -  -0.205526546681818 | -0.683836142215639
67 | fBodyGyro-meanFreq()-X | numeric | -0.241341060754489  -  0.0289087194733538 | -0.100135905573026
68 | fBodyGyro-meanFreq()-Y | numeric | -0.375332544565931  -  0.0737505451791667 | -0.166573403803166
69 | fBodyGyro-meanFreq()-Z | numeric | -0.212818474897214  -  0.101044783556 | -0.0468891970850598
70 | fBodyAccMag-mean() | numeric | -0.990007266206896  -  -0.0295832732681818 | -0.581480861365476
71 | fBodyAccMag-std() | numeric | -0.98628791137931  -  -0.323464307272727 | -0.661430799372623
72 | fBodyAccMag-meanFreq() | numeric | -0.0600681274123529  -  0.320082676954545 | 0.0926085889563971
73 | fBodyBodyAccJerkMag-mean() | numeric | -0.993005947241379  -  0.00382710664090909 | -0.611855760336072
74 | fBodyBodyAccJerkMag-std() | numeric | -0.992630932068965  -  -0.0977799986818182 | -0.634830225735499
75 | fBodyBodyAccJerkMag-meanFreq() | numeric | 0.0817046208143603  -  0.428727917586207 | 0.182338743368244
76 | fBodyBodyGyroMag-mean() | numeric | -0.986607555172414  -  -0.354449740454545 | -0.695629699907979
77 | fBodyBodyGyroMag-std() | numeric | -0.981446073103448  -  -0.2723853645 | -0.696922660106319
78 | fBodyBodyGyroMag-meanFreq() | numeric | -0.220820330447482  -  0.154723197790323 | -0.0424912941658357
79 | fBodyBodyGyroJerkMag-mean() | numeric | -0.99327833  -  -0.584111049810215 | -0.781305943586437
80 | fBodyBodyGyroJerkMag-std() | numeric | -0.993482856896552  -  -0.593735302105376 | -0.794908327002027
81 | fBodyBodyGyroJerkMag-meanFreq() | numeric | -0.0133907447233981  -  0.370064592413793 | 0.13553690099474
82 | angle(tBodyAccMean,gravity) | numeric | -0.0156791396750104  -  0.0760052372590909 | 0.00965936690964764
83 | angle(tBodyAccJerkMean),gravityMean) | numeric | -0.0954311007272727  -  0.0470369997647922 | -0.00274631176430712
84 | angle(tBodyGyroMean,gravityMean) | numeric | -0.276102217727273  -  0.118881574046188 | 0.0101549630157439
85 | angle(tBodyGyroJerkMean,gravityMean) | numeric | -0.06449492227475  -  0.0851886389585859 | -0.00520643921436258
86 | angle(X,gravityMean) | numeric | -0.670442528275862  -  -0.277273605729167 | -0.498910538075301
87 | angle(Y,gravityMean) | numeric | -0.0959038883229167  -  0.328083675454545 | 0.0743908291985821
88 | angle(Z,gravityMean) | numeric | -0.186281046709699  -  0.217081473103448 | -0.0354917789453627

