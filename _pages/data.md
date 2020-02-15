---
layout: single
title: Data Description
permalink: /data_description/
date: 2020-01-08T00:00:00+09:00
---
The data has been collected using two smartphones (right arm and left hip), two smartwatches (both wrists) and one motion capture system with 29 markers. There were 4 subjects who prepared 3 recipes (sandwich, fruit salad, cereal) 5 times each. The subjects followed a script for each recipe but acted as naturally as possible.

*Important Notice*
We have updated the dataset, so the file names may have changed. The updated dataset contains timestamps (in milliseconds) for the data. The timestamp indicates the number of milliseconds since the segment started. You can now work with the missing data.

[Download the training data](https://ieee-dataport.org/open-access/cooking-activity-dataset-macro-and-micro-activities)

The following is a video example of one recording session during the sandwich recipe.
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/CuL029l5Vpg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The following is an example of the motion capture recording.
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9h4AwslZQ_o" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Data structure
The data has been separated into training data and test data. Training data contains data from 3 subjects and test data contains the fourth subject's data.

Each recording has been segmented into 30-second segments. Each segment was assigned a random identifier, so the order of the segments is unknown. Each sensor data is stored in a separate file with the segment-id used to identify related files. Each body part is represented by one folder. The following figure illustrates this process.

![one recording split into 30 seconds and many files per segment](/cook2020/assets/images/datastructure.png)


The training data folder contains five folders: left hip, right arm, right wrist, left wrist and mocap. Each folder contains the same number of files, one per segment. The name of the file identifies the subject and the segment id. The next figure shows the example of segment 9 represented in all five folders.

![folder structure shows 5 folders with one file in each](/cook2020/assets/images/folder_structure.png)

Remember that the number is random, so the order of the files is not the order of the segments.

The training data contains a labels.txt file. This file contains one row per file, and each row contains the file name, the macro activity and the micro activities all separated by commas. An example of a labels file is shown below showing three rows of the file.
```
subject1_file_939,fruitsalad,Take,Peel,
subject1_file_264,fruitsalad,Put,Cut,Peel,
subject1_file_975,fruitsalad,Take,Add,Mix,
```

Test data will become available in March 1st 2020.

[Make a submission](/cook2020/submit/)
