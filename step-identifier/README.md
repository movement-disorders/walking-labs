# Step Idenfifier experiment

Towards decyphering how to be able to assist an individual during a walking session, the need to be able to recognize some mechanics becomes apparent. In this experiment, the focus sits on recognizing the walking pattern. We see in multiple HAR (Human Activity Recognition) related literature *[references-here]* that it's possible to derive this info, in much or less specificity, by locating a set of sensors in the subject's body, and measure from there.

## Selected approach
To support our initial hypothesis, we're planning to gather all the information required, from a single device, that will hold both an accelerometer + gyroscope, giving a total of "6 degrees of freedom". As we'll show in the companion notebook, that's required to recognize step occurrences during a walking session (accelerometer), and derive laterality as well (gyroscope). The device will be located in the Sacrum area, adhered to the subject's body as much as possible, to avoid "noise" at data capture time.

## Why?
Our initial idea is to come up with an intelligent device, capable of providing real time feedback, minimizing fall risk, and collecting data for off-line analysis, during the context of walking sessions, so afflicted individuals make use of it to support their physical training.

> The hardware side specs will also be published and accessible here, so anyone can hack it.

## Bits & pieces
This whole experiment encompasses different efforts: sampling data, model training, electronics design and manufacturing (sounds bigger than it actually is), embedded development, operate a working model in real time, testing, hacking an all in one device, etc. It definitely exceeds an isolated experiment as "Step-Id", but we needed a kickstart to tell you about this bigger result we're trying to achieve.


