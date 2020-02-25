---
layout: single
title: ""
permalink: /faq/
date: 2020-02-10T00:00:00+09:00
---

# Frequently Asked Questions

Submit your questions to abc at sozolab.jp with the subject *Cooking Challenge*.

**What is the sampling rate of each device?**

The sampling rate for the accelerometers is a little bit variable as we used Android to collect the samples. Android operates sensors on a “best effort” policy, meaning that even if we set a desired sampling rate, the actual sampling rate will vary during the application time depending on other factors such as battery level or free memory.

That said,  the average sampling rate for the smartwatches (on each wrist) was about 100Hz and for the smartphones (hip and arm) was about 50Hz. That is why you might get different number of samples on the segments but they all represent 1 minute.

The sampling rate of motion capture is 100Hz.

**I noticed that the new Timestamp field is not always ascending for some sensors. How can we interpret this?**

The data is provided as was collected. In this case, the smartwatch transmits via bluetooth to the smartphone and, in some cases, data is missed or arrives late. The timestamp is the time of the measurement, so you can re-order based on it.
Also, we noticed the left-wrist sensor has many missing data, so please consider it.

**Some files have not label associated. There are 516 files but only 288 rows in the labels file**

We had an error in the published dataset but it has now been corrected and updated. Please download the latest version of the dataset.

**There are some duplicated files in the training data**

We had an error in the published dataset but it has now been corrected and updated. Please download the latest version of the dataset. 
