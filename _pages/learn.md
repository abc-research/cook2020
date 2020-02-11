---
layout: single
title: About Cooking Activity Recognition Challenge
permalink: /learn/
date: 2019-04-14T00:00:00+09:00
---

Activity Recognition is the process of automatically inferring what a user is doing based on sensor observations. When your smartphone automatically identifies if you have been walking or running, it is doing activity recognition using the observations of its accelerometer sensor. Other applications of activity recognition include remote monitoring of daily activities for elders living alone and automatic record creation for nurses in hospitals. Although these applications only require the recognition of the activity being done, i.e.  cooking, such complex activities are usually made up of several smaller activities like ‘taking from the fridge’. Recognizing such steps can have several advantages.  For instance, in the scenario of an elder living alone recognizing the steps can be used to remind them of a missing step, or to ensure a healthy diet is being followed. In the scenario of the nursing record, recognizing the steps can be used for care quality assessment and for ensuring that safety protocols have been followed like washing the hands at the proper moments.

Current activity recognition systems focus on recognizing either the complex label (macro activity) or the small steps (micro activities) but their combined recognition is critical for analysis like the ones proposed. In fact, in a nursing scenario, washing the hands after taking blood is very different than doing it before, as it is mandatory. Therefore, in this challenge, we aim at the recognition of the macro and micro activities taking place during cooking sessions.

## Challenge Goal
The goal of the Cooking Activity Recognition Challenge is to recognize both the macro activity (recipe) and the micro activities taking place during a 30 second window based on motion data collected with accelerometer and motion capture sensors. [Read data description](/cook2020/data_description/).  

[Register to participate](/cook2020/how_to/).


[Get the data](/cook2020/data_description/).

The training dataset contains data about 3 subjects and contains all activity labels.
The test dataset contains data about the other subject and is not labeled.
Participants must submit their predicted macro and micro activities on the test dataset using their models.

[Make a submission](/cook2020/submit/)

## Evaluation
Submissions will be evaluated by the average of the accuracy of macro activity classification (ma) and the average accuracy of micro-activity classification (mi). That is (ma+mi)/2.

The average accuracy of micro-activity classification is based on the multi-label accuracy formula. The accuracy of one sample is given by the number of correct labels predicted divided by the number of total true and predicted labels (cardinality of the union). 


## Prizes
The winner of the challenge will be invited to a visit to our laboratory installations in Kitakyushu, Japan with travel costs supported.
Read the [prize rules](/cook2020/prize_rules/)
