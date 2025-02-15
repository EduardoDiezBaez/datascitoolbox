﻿==================================================================
This codebook is related with the peer reviewed project of the course Getting and Cleaning Data.
The information include the original readme file from the authors of the dataset and the citation.

Aditionally is describe the variables for both files submited.
- FirstSubmissionDataset

- SecondSubmissionDataset

==================================================================


==================================================================
Human Activity Recognition Using Smartphones Dataset
Version 1.0
==================================================================
Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
Smartlab - Non Linear Complex Systems Laboratory
DITEN - Università degli Studi di Genova.
Via Opera Pia 11A, I-16145, Genoa, Italy.
activityrecognition@smartlab.ws
www.smartlab.ws
==================================================================

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

For each record it is provided:
======================================

- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.

The dataset includes the following files:
=========================================

- 'README.txt'

- 'features_info.txt': Shows information about the variables used on the feature vector.

- 'features.txt': List of all features.

- 'activity_labels.txt': Links the class labels with their activity name.

- 'train/X_train.txt': Training set.

- 'train/y_train.txt': Training labels.

- 'test/X_test.txt': Test set.

- 'test/y_test.txt': Test labels.

The following files are available for the train and test data. Their descriptions are equivalent. 

- 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30. 

- 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis. 

- 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration. 

- 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second. 

Notes: 
======
- Features are normalized and bounded within [-1,1].
- Each feature vector is a row on the text file.

For more information about this dataset contact: activityrecognition@smartlab.ws

License:
========
Use of this dataset in publications must be acknowledged by referencing the following publication [1] 

[1] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012

This dataset is distributed AS-IS and no responsibility implied or explicit can be addressed to the authors or their institutions for its use or misuse. Any commercial use is prohibited.

Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, Davide Anguita. November 2012.

Feature Selection 
=================

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag

The set of variables that were estimated from these signals are: 

mean(): Mean value
std(): Standard deviation
mad(): Median absolute deviation 
max(): Largest value in array
min(): Smallest value in array
sma(): Signal magnitude area
energy(): Energy measure. Sum of the squares divided by the number of values. 
iqr(): Interquartile range 
entropy(): Signal entropy
arCoeff(): Autorregresion coefficients with Burg order equal to 4
correlation(): correlation coefficient between two signals
maxInds(): index of the frequency component with largest magnitude
meanFreq(): Weighted average of the frequency components to obtain a mean frequency
skewness(): skewness of the frequency domain signal 
kurtosis(): kurtosis of the frequency domain signal 
bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
angle(): Angle between to vectors.

Additional vectors obtained by averaging the signals in a signal window sample. These are used on the angle() variable:

gravityMean
tBodyAccMean
tBodyAccJerkMean
tBodyGyroMean
tBodyGyroJerkMean

The complete list of variables of each feature vector is available in 'features.txt'


Activity labels 
=================

1 WALKING

2 WALKING_UPSTAIRS

3 WALKING_DOWNSTAIRS

4 SITTING

5 STANDING

6 LAYING


Features for the FirstSubmissionDatase 
=================

The dataset is basically a subset with only the variables that are mean or std of the measurements.

1	tBodyAcc-mean()-X
2	tBodyAcc-mean()-Y
3	tBodyAcc-mean()-Z
4	tBodyAcc-std()-X
5	tBodyAcc-std()-Y
6	tBodyAcc-std()-Z
7	tGravityAcc-mean()-X
8	tGravityAcc-mean()-Y
9	tGravityAcc-mean()-Z
10	tGravityAcc-std()-X
11	tGravityAcc-std()-Y
12	tGravityAcc-std()-Z
13	tBodyAccJerk-mean()-X
14	tBodyAccJerk-mean()-Y
15	tBodyAccJerk-mean()-Z
16	tBodyAccJerk-std()-X
17	tBodyAccJerk-std()-Y
18	tBodyAccJerk-std()-Z
19	tBodyGyro-mean()-X
20	tBodyGyro-mean()-Y
21	tBodyGyro-mean()-Z
22	tBodyGyro-std()-X
23	tBodyGyro-std()-Y
24	tBodyGyro-std()-Z
25	tBodyGyroJerk-mean()-X
26	tBodyGyroJerk-mean()-Y
27	tBodyGyroJerk-mean()-Z
28	tBodyGyroJerk-std()-X
29	tBodyGyroJerk-std()-Y
30	tBodyGyroJerk-std()-Z
31	tBodyAccMag-mean()
32	tBodyAccMag-std()
33	tGravityAccMag-mean()
34	tGravityAccMag-std()
35	tBodyAccJerkMag-mean()
36	tBodyAccJerkMag-std()
37	tBodyGyroMag-mean()
38	tBodyGyroMag-std()
39	tBodyGyroJerkMag-mean()
40	tBodyGyroJerkMag-std()
41	fBodyAcc-mean()-X
42	fBodyAcc-mean()-Y
43	fBodyAcc-mean()-Z
44	fBodyAcc-std()-X
45	fBodyAcc-std()-Y
46	fBodyAcc-std()-Z
47	fBodyAcc-meanFreq()-X
48	fBodyAcc-meanFreq()-Y
49	fBodyAcc-meanFreq()-Z
50	fBodyAccJerk-mean()-X
51	fBodyAccJerk-mean()-Y
52	fBodyAccJerk-mean()-Z
53	fBodyAccJerk-std()-X
54	fBodyAccJerk-std()-Y
55	fBodyAccJerk-std()-Z
56	fBodyAccJerk-meanFreq()-X
57	fBodyAccJerk-meanFreq()-Y
58	fBodyAccJerk-meanFreq()-Z
59	fBodyGyro-mean()-X
60	fBodyGyro-mean()-Y
61	fBodyGyro-mean()-Z
62	fBodyGyro-std()-X
63	fBodyGyro-std()-Y
64	fBodyGyro-std()-Z
65	fBodyGyro-meanFreq()-X
66	fBodyGyro-meanFreq()-Y
67	fBodyGyro-meanFreq()-Z
68	fBodyAccMag-mean()
69	fBodyAccMag-std()
70	fBodyAccMag-meanFreq()
71	fBodyBodyAccJerkMag-mean()
72	fBodyBodyAccJerkMag-std()
73	fBodyBodyAccJerkMag-meanFreq()
74	fBodyBodyGyroMag-mean()
75	fBodyBodyGyroMag-std()
76	fBodyBodyGyroMag-meanFreq()
77	fBodyBodyGyroJerkMag-mean()
78	fBodyBodyGyroJerkMag-std()
79	fBodyBodyGyroJerkMag-meanFreq()
80	angle(tBodyAccMean,gravity)
81	angle(tBodyAccJerkMean),gravityMean)
82	angle(tBodyGyroMean,gravityMean)
83	angle(tBodyGyroJerkMean,gravityMean)
84	angle(X,gravityMean)
85	angle(Y,gravityMean)
86	angle(Z,gravityMean)



Features for the SecondSubmissionDatase 
=================

The dataset have variables 1 and 2 adittional to the original and each value correspond to the mean for each volunter/subject at every activity. 

1	volunter
2	activity
3	tBodyAcc-mean()-X
4	tBodyAcc-mean()-Y
5	tBodyAcc-mean()-Z
6	tBodyAcc-std()-X
7	tBodyAcc-std()-Y
8	tBodyAcc-std()-Z
9	tBodyAcc-mad()-X
10	tBodyAcc-mad()-Y
11	tBodyAcc-mad()-Z
12	tBodyAcc-max()-X
13	tBodyAcc-max()-Y
14	tBodyAcc-max()-Z
15	tBodyAcc-min()-X
16	tBodyAcc-min()-Y
17	tBodyAcc-min()-Z
18	tBodyAcc-sma()
19	tBodyAcc-energy()-X
20	tBodyAcc-energy()-Y
21	tBodyAcc-energy()-Z
22	tBodyAcc-iqr()-X
23	tBodyAcc-iqr()-Y
24	tBodyAcc-iqr()-Z
25	tBodyAcc-entropy()-X
26	tBodyAcc-entropy()-Y
27	tBodyAcc-entropy()-Z
28	tBodyAcc-arCoeff()-X,1
29	tBodyAcc-arCoeff()-X,2
30	tBodyAcc-arCoeff()-X,3
31	tBodyAcc-arCoeff()-X,4
32	tBodyAcc-arCoeff()-Y,1
33	tBodyAcc-arCoeff()-Y,2
34	tBodyAcc-arCoeff()-Y,3
35	tBodyAcc-arCoeff()-Y,4
36	tBodyAcc-arCoeff()-Z,1
37	tBodyAcc-arCoeff()-Z,2
38	tBodyAcc-arCoeff()-Z,3
39	tBodyAcc-arCoeff()-Z,4
40	tBodyAcc-correlation()-X,Y
41	tBodyAcc-correlation()-X,Z
42	tBodyAcc-correlation()-Y,Z
43	tGravityAcc-mean()-X
44	tGravityAcc-mean()-Y
45	tGravityAcc-mean()-Z
46	tGravityAcc-std()-X
47	tGravityAcc-std()-Y
48	tGravityAcc-std()-Z
49	tGravityAcc-mad()-X
50	tGravityAcc-mad()-Y
51	tGravityAcc-mad()-Z
52	tGravityAcc-max()-X
53	tGravityAcc-max()-Y
54	tGravityAcc-max()-Z
55	tGravityAcc-min()-X
56	tGravityAcc-min()-Y
57	tGravityAcc-min()-Z
58	tGravityAcc-sma()
59	tGravityAcc-energy()-X
60	tGravityAcc-energy()-Y
61	tGravityAcc-energy()-Z
62	tGravityAcc-iqr()-X
63	tGravityAcc-iqr()-Y
64	tGravityAcc-iqr()-Z
65	tGravityAcc-entropy()-X
66	tGravityAcc-entropy()-Y
67	tGravityAcc-entropy()-Z
68	tGravityAcc-arCoeff()-X,1
69	tGravityAcc-arCoeff()-X,2
70	tGravityAcc-arCoeff()-X,3
71	tGravityAcc-arCoeff()-X,4
72	tGravityAcc-arCoeff()-Y,1
73	tGravityAcc-arCoeff()-Y,2
74	tGravityAcc-arCoeff()-Y,3
75	tGravityAcc-arCoeff()-Y,4
76	tGravityAcc-arCoeff()-Z,1
77	tGravityAcc-arCoeff()-Z,2
78	tGravityAcc-arCoeff()-Z,3
79	tGravityAcc-arCoeff()-Z,4
80	tGravityAcc-correlation()-X,Y
81	tGravityAcc-correlation()-X,Z
82	tGravityAcc-correlation()-Y,Z
83	tBodyAccJerk-mean()-X
84	tBodyAccJerk-mean()-Y
85	tBodyAccJerk-mean()-Z
86	tBodyAccJerk-std()-X
87	tBodyAccJerk-std()-Y
88	tBodyAccJerk-std()-Z
89	tBodyAccJerk-mad()-X
90	tBodyAccJerk-mad()-Y
91	tBodyAccJerk-mad()-Z
92	tBodyAccJerk-max()-X
93	tBodyAccJerk-max()-Y
94	tBodyAccJerk-max()-Z
95	tBodyAccJerk-min()-X
96	tBodyAccJerk-min()-Y
97	tBodyAccJerk-min()-Z
98	tBodyAccJerk-sma()
99	tBodyAccJerk-energy()-X
100	tBodyAccJerk-energy()-Y
101	tBodyAccJerk-energy()-Z
102	tBodyAccJerk-iqr()-X
103	tBodyAccJerk-iqr()-Y
104	tBodyAccJerk-iqr()-Z
105	tBodyAccJerk-entropy()-X
106	tBodyAccJerk-entropy()-Y
107	tBodyAccJerk-entropy()-Z
108	tBodyAccJerk-arCoeff()-X,1
109	tBodyAccJerk-arCoeff()-X,2
110	tBodyAccJerk-arCoeff()-X,3
111	tBodyAccJerk-arCoeff()-X,4
112	tBodyAccJerk-arCoeff()-Y,1
113	tBodyAccJerk-arCoeff()-Y,2
114	tBodyAccJerk-arCoeff()-Y,3
115	tBodyAccJerk-arCoeff()-Y,4
116	tBodyAccJerk-arCoeff()-Z,1
117	tBodyAccJerk-arCoeff()-Z,2
118	tBodyAccJerk-arCoeff()-Z,3
119	tBodyAccJerk-arCoeff()-Z,4
120	tBodyAccJerk-correlation()-X,Y
121	tBodyAccJerk-correlation()-X,Z
122	tBodyAccJerk-correlation()-Y,Z
123	tBodyGyro-mean()-X
124	tBodyGyro-mean()-Y
125	tBodyGyro-mean()-Z
126	tBodyGyro-std()-X
127	tBodyGyro-std()-Y
128	tBodyGyro-std()-Z
129	tBodyGyro-mad()-X
130	tBodyGyro-mad()-Y
131	tBodyGyro-mad()-Z
132	tBodyGyro-max()-X
133	tBodyGyro-max()-Y
134	tBodyGyro-max()-Z
135	tBodyGyro-min()-X
136	tBodyGyro-min()-Y
137	tBodyGyro-min()-Z
138	tBodyGyro-sma()
139	tBodyGyro-energy()-X
140	tBodyGyro-energy()-Y
141	tBodyGyro-energy()-Z
142	tBodyGyro-iqr()-X
143	tBodyGyro-iqr()-Y
144	tBodyGyro-iqr()-Z
145	tBodyGyro-entropy()-X
146	tBodyGyro-entropy()-Y
147	tBodyGyro-entropy()-Z
148	tBodyGyro-arCoeff()-X,1
149	tBodyGyro-arCoeff()-X,2
150	tBodyGyro-arCoeff()-X,3
151	tBodyGyro-arCoeff()-X,4
152	tBodyGyro-arCoeff()-Y,1
153	tBodyGyro-arCoeff()-Y,2
154	tBodyGyro-arCoeff()-Y,3
155	tBodyGyro-arCoeff()-Y,4
156	tBodyGyro-arCoeff()-Z,1
157	tBodyGyro-arCoeff()-Z,2
158	tBodyGyro-arCoeff()-Z,3
159	tBodyGyro-arCoeff()-Z,4
160	tBodyGyro-correlation()-X,Y
161	tBodyGyro-correlation()-X,Z
162	tBodyGyro-correlation()-Y,Z
163	tBodyGyroJerk-mean()-X
164	tBodyGyroJerk-mean()-Y
165	tBodyGyroJerk-mean()-Z
166	tBodyGyroJerk-std()-X
167	tBodyGyroJerk-std()-Y
168	tBodyGyroJerk-std()-Z
169	tBodyGyroJerk-mad()-X
170	tBodyGyroJerk-mad()-Y
171	tBodyGyroJerk-mad()-Z
172	tBodyGyroJerk-max()-X
173	tBodyGyroJerk-max()-Y
174	tBodyGyroJerk-max()-Z
175	tBodyGyroJerk-min()-X
176	tBodyGyroJerk-min()-Y
177	tBodyGyroJerk-min()-Z
178	tBodyGyroJerk-sma()
179	tBodyGyroJerk-energy()-X
180	tBodyGyroJerk-energy()-Y
181	tBodyGyroJerk-energy()-Z
182	tBodyGyroJerk-iqr()-X
183	tBodyGyroJerk-iqr()-Y
184	tBodyGyroJerk-iqr()-Z
185	tBodyGyroJerk-entropy()-X
186	tBodyGyroJerk-entropy()-Y
187	tBodyGyroJerk-entropy()-Z
188	tBodyGyroJerk-arCoeff()-X,1
189	tBodyGyroJerk-arCoeff()-X,2
190	tBodyGyroJerk-arCoeff()-X,3
191	tBodyGyroJerk-arCoeff()-X,4
192	tBodyGyroJerk-arCoeff()-Y,1
193	tBodyGyroJerk-arCoeff()-Y,2
194	tBodyGyroJerk-arCoeff()-Y,3
195	tBodyGyroJerk-arCoeff()-Y,4
196	tBodyGyroJerk-arCoeff()-Z,1
197	tBodyGyroJerk-arCoeff()-Z,2
198	tBodyGyroJerk-arCoeff()-Z,3
199	tBodyGyroJerk-arCoeff()-Z,4
200	tBodyGyroJerk-correlation()-X,Y
201	tBodyGyroJerk-correlation()-X,Z
202	tBodyGyroJerk-correlation()-Y,Z
203	tBodyAccMag-mean()
204	tBodyAccMag-std()
205	tBodyAccMag-mad()
206	tBodyAccMag-max()
207	tBodyAccMag-min()
208	tBodyAccMag-sma()
209	tBodyAccMag-energy()
210	tBodyAccMag-iqr()
211	tBodyAccMag-entropy()
212	tBodyAccMag-arCoeff()1
213	tBodyAccMag-arCoeff()2
214	tBodyAccMag-arCoeff()3
215	tBodyAccMag-arCoeff()4
216	tGravityAccMag-mean()
217	tGravityAccMag-std()
218	tGravityAccMag-mad()
219	tGravityAccMag-max()
220	tGravityAccMag-min()
221	tGravityAccMag-sma()
222	tGravityAccMag-energy()
223	tGravityAccMag-iqr()
224	tGravityAccMag-entropy()
225	tGravityAccMag-arCoeff()1
226	tGravityAccMag-arCoeff()2
227	tGravityAccMag-arCoeff()3
228	tGravityAccMag-arCoeff()4
229	tBodyAccJerkMag-mean()
230	tBodyAccJerkMag-std()
231	tBodyAccJerkMag-mad()
232	tBodyAccJerkMag-max()
233	tBodyAccJerkMag-min()
234	tBodyAccJerkMag-sma()
235	tBodyAccJerkMag-energy()
236	tBodyAccJerkMag-iqr()
237	tBodyAccJerkMag-entropy()
238	tBodyAccJerkMag-arCoeff()1
239	tBodyAccJerkMag-arCoeff()2
240	tBodyAccJerkMag-arCoeff()3
241	tBodyAccJerkMag-arCoeff()4
242	tBodyGyroMag-mean()
243	tBodyGyroMag-std()
244	tBodyGyroMag-mad()
245	tBodyGyroMag-max()
246	tBodyGyroMag-min()
247	tBodyGyroMag-sma()
248	tBodyGyroMag-energy()
249	tBodyGyroMag-iqr()
250	tBodyGyroMag-entropy()
251	tBodyGyroMag-arCoeff()1
252	tBodyGyroMag-arCoeff()2
253	tBodyGyroMag-arCoeff()3
254	tBodyGyroMag-arCoeff()4
255	tBodyGyroJerkMag-mean()
256	tBodyGyroJerkMag-std()
257	tBodyGyroJerkMag-mad()
258	tBodyGyroJerkMag-max()
259	tBodyGyroJerkMag-min()
260	tBodyGyroJerkMag-sma()
261	tBodyGyroJerkMag-energy()
262	tBodyGyroJerkMag-iqr()
263	tBodyGyroJerkMag-entropy()
264	tBodyGyroJerkMag-arCoeff()1
265	tBodyGyroJerkMag-arCoeff()2
266	tBodyGyroJerkMag-arCoeff()3
267	tBodyGyroJerkMag-arCoeff()4
268	fBodyAcc-mean()-X
269	fBodyAcc-mean()-Y
270	fBodyAcc-mean()-Z
271	fBodyAcc-std()-X
272	fBodyAcc-std()-Y
273	fBodyAcc-std()-Z
274	fBodyAcc-mad()-X
275	fBodyAcc-mad()-Y
276	fBodyAcc-mad()-Z
277	fBodyAcc-max()-X
278	fBodyAcc-max()-Y
279	fBodyAcc-max()-Z
280	fBodyAcc-min()-X
281	fBodyAcc-min()-Y
282	fBodyAcc-min()-Z
283	fBodyAcc-sma()
284	fBodyAcc-energy()-X
285	fBodyAcc-energy()-Y
286	fBodyAcc-energy()-Z
287	fBodyAcc-iqr()-X
288	fBodyAcc-iqr()-Y
289	fBodyAcc-iqr()-Z
290	fBodyAcc-entropy()-X
291	fBodyAcc-entropy()-Y
292	fBodyAcc-entropy()-Z
293	fBodyAcc-maxInds-X
294	fBodyAcc-maxInds-Y
295	fBodyAcc-maxInds-Z
296	fBodyAcc-meanFreq()-X
297	fBodyAcc-meanFreq()-Y
298	fBodyAcc-meanFreq()-Z
299	fBodyAcc-skewness()-X
300	fBodyAcc-kurtosis()-X
301	fBodyAcc-skewness()-Y
302	fBodyAcc-kurtosis()-Y
303	fBodyAcc-skewness()-Z
304	fBodyAcc-kurtosis()-Z
305	fBodyAcc-bandsEnergy()-1,8
306	fBodyAcc-bandsEnergy()-9,16
307	fBodyAcc-bandsEnergy()-17,24
308	fBodyAcc-bandsEnergy()-25,32
309	fBodyAcc-bandsEnergy()-33,40
310	fBodyAcc-bandsEnergy()-41,48
311	fBodyAcc-bandsEnergy()-49,56
312	fBodyAcc-bandsEnergy()-57,64
313	fBodyAcc-bandsEnergy()-1,16
314	fBodyAcc-bandsEnergy()-17,32
315	fBodyAcc-bandsEnergy()-33,48
316	fBodyAcc-bandsEnergy()-49,64
317	fBodyAcc-bandsEnergy()-1,24
318	fBodyAcc-bandsEnergy()-25,48
319	fBodyAcc-bandsEnergy()-1,8.1
320	fBodyAcc-bandsEnergy()-9,16.1
321	fBodyAcc-bandsEnergy()-17,24.1
322	fBodyAcc-bandsEnergy()-25,32.1
323	fBodyAcc-bandsEnergy()-33,40.1
324	fBodyAcc-bandsEnergy()-41,48.1
325	fBodyAcc-bandsEnergy()-49,56.1
326	fBodyAcc-bandsEnergy()-57,64.1
327	fBodyAcc-bandsEnergy()-1,16.1
328	fBodyAcc-bandsEnergy()-17,32.1
329	fBodyAcc-bandsEnergy()-33,48.1
330	fBodyAcc-bandsEnergy()-49,64.1
331	fBodyAcc-bandsEnergy()-1,24.1
332	fBodyAcc-bandsEnergy()-25,48.1
333	fBodyAcc-bandsEnergy()-1,8.2
334	fBodyAcc-bandsEnergy()-9,16.2
335	fBodyAcc-bandsEnergy()-17,24.2
336	fBodyAcc-bandsEnergy()-25,32.2
337	fBodyAcc-bandsEnergy()-33,40.2
338	fBodyAcc-bandsEnergy()-41,48.2
339	fBodyAcc-bandsEnergy()-49,56.2
340	fBodyAcc-bandsEnergy()-57,64.2
341	fBodyAcc-bandsEnergy()-1,16.2
342	fBodyAcc-bandsEnergy()-17,32.2
343	fBodyAcc-bandsEnergy()-33,48.2
344	fBodyAcc-bandsEnergy()-49,64.2
345	fBodyAcc-bandsEnergy()-1,24.2
346	fBodyAcc-bandsEnergy()-25,48.2
347	fBodyAccJerk-mean()-X
348	fBodyAccJerk-mean()-Y
349	fBodyAccJerk-mean()-Z
350	fBodyAccJerk-std()-X
351	fBodyAccJerk-std()-Y
352	fBodyAccJerk-std()-Z
353	fBodyAccJerk-mad()-X
354	fBodyAccJerk-mad()-Y
355	fBodyAccJerk-mad()-Z
356	fBodyAccJerk-max()-X
357	fBodyAccJerk-max()-Y
358	fBodyAccJerk-max()-Z
359	fBodyAccJerk-min()-X
360	fBodyAccJerk-min()-Y
361	fBodyAccJerk-min()-Z
362	fBodyAccJerk-sma()
363	fBodyAccJerk-energy()-X
364	fBodyAccJerk-energy()-Y
365	fBodyAccJerk-energy()-Z
366	fBodyAccJerk-iqr()-X
367	fBodyAccJerk-iqr()-Y
368	fBodyAccJerk-iqr()-Z
369	fBodyAccJerk-entropy()-X
370	fBodyAccJerk-entropy()-Y
371	fBodyAccJerk-entropy()-Z
372	fBodyAccJerk-maxInds-X
373	fBodyAccJerk-maxInds-Y
374	fBodyAccJerk-maxInds-Z
375	fBodyAccJerk-meanFreq()-X
376	fBodyAccJerk-meanFreq()-Y
377	fBodyAccJerk-meanFreq()-Z
378	fBodyAccJerk-skewness()-X
379	fBodyAccJerk-kurtosis()-X
380	fBodyAccJerk-skewness()-Y
381	fBodyAccJerk-kurtosis()-Y
382	fBodyAccJerk-skewness()-Z
383	fBodyAccJerk-kurtosis()-Z
384	fBodyAccJerk-bandsEnergy()-1,8
385	fBodyAccJerk-bandsEnergy()-9,16
386	fBodyAccJerk-bandsEnergy()-17,24
387	fBodyAccJerk-bandsEnergy()-25,32
388	fBodyAccJerk-bandsEnergy()-33,40
389	fBodyAccJerk-bandsEnergy()-41,48
390	fBodyAccJerk-bandsEnergy()-49,56
391	fBodyAccJerk-bandsEnergy()-57,64
392	fBodyAccJerk-bandsEnergy()-1,16
393	fBodyAccJerk-bandsEnergy()-17,32
394	fBodyAccJerk-bandsEnergy()-33,48
395	fBodyAccJerk-bandsEnergy()-49,64
396	fBodyAccJerk-bandsEnergy()-1,24
397	fBodyAccJerk-bandsEnergy()-25,48
398	fBodyAccJerk-bandsEnergy()-1,8.1
399	fBodyAccJerk-bandsEnergy()-9,16.1
400	fBodyAccJerk-bandsEnergy()-17,24.1
401	fBodyAccJerk-bandsEnergy()-25,32.1
402	fBodyAccJerk-bandsEnergy()-33,40.1
403	fBodyAccJerk-bandsEnergy()-41,48.1
404	fBodyAccJerk-bandsEnergy()-49,56.1
405	fBodyAccJerk-bandsEnergy()-57,64.1
406	fBodyAccJerk-bandsEnergy()-1,16.1
407	fBodyAccJerk-bandsEnergy()-17,32.1
408	fBodyAccJerk-bandsEnergy()-33,48.1
409	fBodyAccJerk-bandsEnergy()-49,64.1
410	fBodyAccJerk-bandsEnergy()-1,24.1
411	fBodyAccJerk-bandsEnergy()-25,48.1
412	fBodyAccJerk-bandsEnergy()-1,8.2
413	fBodyAccJerk-bandsEnergy()-9,16.2
414	fBodyAccJerk-bandsEnergy()-17,24.2
415	fBodyAccJerk-bandsEnergy()-25,32.2
416	fBodyAccJerk-bandsEnergy()-33,40.2
417	fBodyAccJerk-bandsEnergy()-41,48.2
418	fBodyAccJerk-bandsEnergy()-49,56.2
419	fBodyAccJerk-bandsEnergy()-57,64.2
420	fBodyAccJerk-bandsEnergy()-1,16.2
421	fBodyAccJerk-bandsEnergy()-17,32.2
422	fBodyAccJerk-bandsEnergy()-33,48.2
423	fBodyAccJerk-bandsEnergy()-49,64.2
424	fBodyAccJerk-bandsEnergy()-1,24.2
425	fBodyAccJerk-bandsEnergy()-25,48.2
426	fBodyGyro-mean()-X
427	fBodyGyro-mean()-Y
428	fBodyGyro-mean()-Z
429	fBodyGyro-std()-X
430	fBodyGyro-std()-Y
431	fBodyGyro-std()-Z
432	fBodyGyro-mad()-X
433	fBodyGyro-mad()-Y
434	fBodyGyro-mad()-Z
435	fBodyGyro-max()-X
436	fBodyGyro-max()-Y
437	fBodyGyro-max()-Z
438	fBodyGyro-min()-X
439	fBodyGyro-min()-Y
440	fBodyGyro-min()-Z
441	fBodyGyro-sma()
442	fBodyGyro-energy()-X
443	fBodyGyro-energy()-Y
444	fBodyGyro-energy()-Z
445	fBodyGyro-iqr()-X
446	fBodyGyro-iqr()-Y
447	fBodyGyro-iqr()-Z
448	fBodyGyro-entropy()-X
449	fBodyGyro-entropy()-Y
450	fBodyGyro-entropy()-Z
451	fBodyGyro-maxInds-X
452	fBodyGyro-maxInds-Y
453	fBodyGyro-maxInds-Z
454	fBodyGyro-meanFreq()-X
455	fBodyGyro-meanFreq()-Y
456	fBodyGyro-meanFreq()-Z
457	fBodyGyro-skewness()-X
458	fBodyGyro-kurtosis()-X
459	fBodyGyro-skewness()-Y
460	fBodyGyro-kurtosis()-Y
461	fBodyGyro-skewness()-Z
462	fBodyGyro-kurtosis()-Z
463	fBodyGyro-bandsEnergy()-1,8
464	fBodyGyro-bandsEnergy()-9,16
465	fBodyGyro-bandsEnergy()-17,24
466	fBodyGyro-bandsEnergy()-25,32
467	fBodyGyro-bandsEnergy()-33,40
468	fBodyGyro-bandsEnergy()-41,48
469	fBodyGyro-bandsEnergy()-49,56
470	fBodyGyro-bandsEnergy()-57,64
471	fBodyGyro-bandsEnergy()-1,16
472	fBodyGyro-bandsEnergy()-17,32
473	fBodyGyro-bandsEnergy()-33,48
474	fBodyGyro-bandsEnergy()-49,64
475	fBodyGyro-bandsEnergy()-1,24
476	fBodyGyro-bandsEnergy()-25,48
477	fBodyGyro-bandsEnergy()-1,8.1
478	fBodyGyro-bandsEnergy()-9,16.1
479	fBodyGyro-bandsEnergy()-17,24.1
480	fBodyGyro-bandsEnergy()-25,32.1
481	fBodyGyro-bandsEnergy()-33,40.1
482	fBodyGyro-bandsEnergy()-41,48.1
483	fBodyGyro-bandsEnergy()-49,56.1
484	fBodyGyro-bandsEnergy()-57,64.1
485	fBodyGyro-bandsEnergy()-1,16.1
486	fBodyGyro-bandsEnergy()-17,32.1
487	fBodyGyro-bandsEnergy()-33,48.1
488	fBodyGyro-bandsEnergy()-49,64.1
489	fBodyGyro-bandsEnergy()-1,24.1
490	fBodyGyro-bandsEnergy()-25,48.1
491	fBodyGyro-bandsEnergy()-1,8.2
492	fBodyGyro-bandsEnergy()-9,16.2
493	fBodyGyro-bandsEnergy()-17,24.2
494	fBodyGyro-bandsEnergy()-25,32.2
495	fBodyGyro-bandsEnergy()-33,40.2
496	fBodyGyro-bandsEnergy()-41,48.2
497	fBodyGyro-bandsEnergy()-49,56.2
498	fBodyGyro-bandsEnergy()-57,64.2
499	fBodyGyro-bandsEnergy()-1,16.2
500	fBodyGyro-bandsEnergy()-17,32.2
501	fBodyGyro-bandsEnergy()-33,48.2
502	fBodyGyro-bandsEnergy()-49,64.2
503	fBodyGyro-bandsEnergy()-1,24.2
504	fBodyGyro-bandsEnergy()-25,48.2
505	fBodyAccMag-mean()
506	fBodyAccMag-std()
507	fBodyAccMag-mad()
508	fBodyAccMag-max()
509	fBodyAccMag-min()
510	fBodyAccMag-sma()
511	fBodyAccMag-energy()
512	fBodyAccMag-iqr()
513	fBodyAccMag-entropy()
514	fBodyAccMag-maxInds
515	fBodyAccMag-meanFreq()
516	fBodyAccMag-skewness()
517	fBodyAccMag-kurtosis()
518	fBodyBodyAccJerkMag-mean()
519	fBodyBodyAccJerkMag-std()
520	fBodyBodyAccJerkMag-mad()
521	fBodyBodyAccJerkMag-max()
522	fBodyBodyAccJerkMag-min()
523	fBodyBodyAccJerkMag-sma()
524	fBodyBodyAccJerkMag-energy()
525	fBodyBodyAccJerkMag-iqr()
526	fBodyBodyAccJerkMag-entropy()
527	fBodyBodyAccJerkMag-maxInds
528	fBodyBodyAccJerkMag-meanFreq()
529	fBodyBodyAccJerkMag-skewness()
530	fBodyBodyAccJerkMag-kurtosis()
531	fBodyBodyGyroMag-mean()
532	fBodyBodyGyroMag-std()
533	fBodyBodyGyroMag-mad()
534	fBodyBodyGyroMag-max()
535	fBodyBodyGyroMag-min()
536	fBodyBodyGyroMag-sma()
537	fBodyBodyGyroMag-energy()
538	fBodyBodyGyroMag-iqr()
539	fBodyBodyGyroMag-entropy()
540	fBodyBodyGyroMag-maxInds
541	fBodyBodyGyroMag-meanFreq()
542	fBodyBodyGyroMag-skewness()
543	fBodyBodyGyroMag-kurtosis()
544	fBodyBodyGyroJerkMag-mean()
545	fBodyBodyGyroJerkMag-std()
546	fBodyBodyGyroJerkMag-mad()
547	fBodyBodyGyroJerkMag-max()
548	fBodyBodyGyroJerkMag-min()
549	fBodyBodyGyroJerkMag-sma()
550	fBodyBodyGyroJerkMag-energy()
551	fBodyBodyGyroJerkMag-iqr()
552	fBodyBodyGyroJerkMag-entropy()
553	fBodyBodyGyroJerkMag-maxInds
554	fBodyBodyGyroJerkMag-meanFreq()
555	fBodyBodyGyroJerkMag-skewness()
556	fBodyBodyGyroJerkMag-kurtosis()
557	angle(tBodyAccMean,gravity)
558	angle(tBodyAccJerkMean),gravityMean)
559	angle(tBodyGyroMean,gravityMean)
560	angle(tBodyGyroJerkMean,gravityMean)
561	angle(X,gravityMean)
562	angle(Y,gravityMean)
563	angle(Z,gravityMean)
