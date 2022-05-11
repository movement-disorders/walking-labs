## Disclaimer area

Based on: https://towardsdatascience.com/feature-engineering-on-time-series-data-transforming-signal-data-of-a-smartphone-accelerometer-for-72cbe34b8a60

**Source Paper:** Jennifer R. Kwapisz, Gary M. Weiss and Samuel A. Moore (2010). 
Activity Recognition using Cell Phone Accelerometers, 
Proceedings of the Fourth International Workshop on Knowledge 
Discovery from Sensor Data (at KDD-10), Washington DC. https://www.cis.fordham.edu/wisdm/includes/files/sensorKDD-2010.pdf

**Getting the dataset:** https://www.cis.fordham.edu/wisdm/dataset.php

---

# Step by step: Feature Engineering on Time-Series Data for Human Activity Recognition, by Pratik Nabriya [[source](https://towardsdatascience.com/feature-engineering-on-time-series-data-transforming-signal-data-of-a-smartphone-accelerometer-for-72cbe34b8a60)]

A step towards focusing discretely on Walking. We want to be able to recognize a single step pattern, considering left and right origin. From there, we'll dig deep for [Step & Stride Length](http://www.clinicalgaitanalysis.com/teach-in/step/)[^1]. Moving up from there, other gait subtleties interest us besides measuring & analizing. We'd like to come up with a waist portable device that can warn when a movement can suddenly put an individual in harm's way (more on this in *[a specific folder to be pointed at]*).

This study helps on analyzing real data captured with an accelerometer, then massaged and finally turned into a prediction model as actionable data. It's an interesting training to take.

[^1]: Unencrypted link. Use just for reading please. Do not fill any data. Although, you shouldn't be asked to anyway.
