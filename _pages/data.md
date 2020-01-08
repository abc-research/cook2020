---
layout: single
permalink: /data_description/
date: 2019-04-14T00:00:00+09:00
---
## Data Description

The data has been collected using two smartphones (right arm and left hip), two smartwatches (both wrists) and one motion capture system with 29 markers. There were 4 subjects who prepared 3 recipes (sandwich, fruit salad, cereal) 5 times each following a script but acting as naturally as possible.

[Download the training data](https://drive.google.com/open?id=1qesNRRpV-xbRzhdnPhcPY8MtZ-2wKUxe)

The training data consists of segments each representing 30 seconds of activity. For each segment, a file for each sensor used is given. The data is organized in five folders, one for each sensor. All files belonging to the same segment have the same name. The labels.txt file contains one row per file, and each row contains the file name, the macro activity and the micro activities all separated by commas. The labels file has the same format as the submission expected.
Figure 1 shows an example of the file structure, where the same segment is represented in all 5 sensor types.

![folder structure shows 5 folders with one file in each](/assets/images/folder_structure.png)

An example of a labels file is shown below
```
subject1_file_939,fruitsalad,Take,Peel,
subject1_file_264,fruitsalad,Put,Cut,Peel,
subject1_file_975,fruitsalad,Take,Add,Mix,
```

Training data corresponds to the data of three subjects.
The test data corresponds to the fourth subject’s data.

Test data will become available in March 1st 2020.

[Make a submission](/submit/)
