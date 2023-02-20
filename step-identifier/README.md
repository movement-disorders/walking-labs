# Step Idenfifier experiment

**Disclaimer:** this experiment is focused on those people with both: a movement disorder, and walking ability (with or without a can).

Towards decyphering how to be able to assist an individual during a walking session, the need to recognize walking mechanics patterns becomes a must. In this multi-step experiment, the initial focus sits on recognizing the walking pattern. We see in multiple HAR (Human Activity Recognition) related literature *[references-here]* that it's possible to derive this info, in much or less specificity, by locating a set of sensors in the subject's body, and measure from there. Once understood, we'll test on feeding an ML algorithm with preprocessed data to train itself on recognizing walking patterns. A later step after validation, is to detect anomalies in real time and reacting to them (more on these  later).

## Why?
Advances were made in fall detection techniques and walking pattern analysis. Today these are performed by multi-purpose wearables. People with movement disorders would greatly benefit from applying AI to move a step further into the **prevention space**, to ensure a steady walk while being thoughtfully monitored when exercising.

> "Being a person with a movement disorder makes you appreciate the walking ability that the human body has imprinted within."

## How?
By analizing and real-time monitoring each walking session. Detailing progress and events to be reviewed by the individual and shared with care givers.

## What?
We want to come up with an AI+Sensors packed dedicated wearable, capable of providing real-time feedback, minimizing fall risk, and collecting data for later analysis, during the context of walking sessions, for individuals to use it as support on their physical training.

> The hardware side specs will also be published and accessible here, so anyone can hack it.

## Hypothesis
Using a single device integrating an Acc+Gyro combo located at a subjects lower back (Sacrum area), is enough to get readings about its activity (walking is what we're immediately after). We want to get Gait, Stride, Step, Cycle and Laterality data. All this data will be constantly gathered through the sensors and fed to a trained AI model, capable of detecting when things are about to turn wrong, providing either haptic and auditory feedback. Besides real time obtained results will be stored for later analysis.

## Selected approach
To support our initial hypothesis, we're planning to gather all the information required, from a single device, that will hold both an accelerometer + gyroscope, giving a total of "6 degrees of freedom". As we'll show in the companion notebook, that's required to recognize step occurrences during a walking session (accelerometer), and derive laterality as well (gyroscope). The device will be located at the Sacrum area, adhered to the subject's body through a belt or double sided tape, to ensure a "noise-free" data capture.

## Bits & pieces
This whole experiment encompasses different efforts: sampling data, model training, electronics design and manufacturing, embedded development, operate a working model in real time, testing, hacking an all in one device, etc. It definitely exceeds an isolated experiment as "Step-Id", but we needed a kickstart to tell you about this bigger result we're trying to achieve.

---
# References
### LSTMs for Human Activity Recognition Time Series Classification

> **Source** https://machinelearningmastery.com/how-to-develop-rnn-models-for-human-activity-recognition-time-series-classification/

---
### Dataset Source:

Jorge L. Reyes-Ortiz(1,2), Davide Anguita(1), Luca Oneto(1) and Xavier Parra(2) 
1 - Smartlab, DIBRIS - UniversitÃ  degli Studi di Genova, Genoa (16145), Italy. 
2 - CETpD - Universitat PolitÃ¨cnica de Catalunya. Vilanova i la GeltrÃº (08800), Spain 
har '@' smartlab.ws 
www.smartlab.ws

Since 2015, the UCI HAR Dataset this experiment (`uci-lstm.ipynb`) uses, is available for download with the raw data as well.
* Original (preprocessed): https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
* V2 (includes raw data): https://archive.ics.uci.edu/ml/datasets/Smartphone-Based+Recognition+of+Human+Activities+and+Postural+Transitions
