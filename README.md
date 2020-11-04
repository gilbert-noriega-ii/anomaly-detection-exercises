# Anomaly Detection Repository

<img width="594" alt="Screen Shot 2020-11-03 at 8 34 54 PM" src="https://user-images.githubusercontent.com/68249276/98062654-1840a100-1e14-11eb-96f5-9ae3e6e9777b.png">

<br>

## Goals
- Use Statistical Methods to
    - Flag the data points that deviate from the expected, based on the statistical properties, such as mean, median, mode, and quantiles.
    - Define an anomalous data point as one that deviates by a certain standard deviation from the mean.
    - Use a simple or exponential moving average to smooth short-term fluctuations and highlight long-term ones.
- Support Vector Machine & Isolation Forest Anomaly Detection by using extensions to the supervised technique, such as OneClassSVM, that can be used to identify anomalies as an unsupervised problems 
- Identify Clustering-Based Anomaly Detection so we can design models such that the data points that do not fall into a cluster are the anomalies
- Identify Density-Based Anomaly Detection and use one of two algorithms, KNN(K-Nearest Neighbor) or LOF(Local Outlier Factor).

<br>

## Anomaly Vocabulary
- **Anomaly**: Anomalies are the unusual, unexpected, surprising patterns in the observed world. An anomalous data point is a deviation from a rule or from what is regarded as normal; an outlier. An anomaly is any event or measurement that is out of the ordinary regardless of whether it is exceptional or not.
- **Outlier**: An outlier is an observation that lies an abnormal distance from other values in a random sample from a population. In a sense, this definition leaves it up to the analyst (or a consensus process) to decide what will be considered abnormal. Before abnormal observations can be singled out, it is necessary to characterize normal observations.
- **Point Anomalies**: A single instance of data is anomalous if it's too far off from the rest. For example, detecting data exfiltration based on gigabytes leaving the network, detecting credit card fraud based on "amount spent", etc.
- **Contextual Anomalies**: The abnormality is context specific. This type of anomaly is common in time-series data. For example, accessing confidential files during work hours is normal, but in the middle of the night is odd.
- **Collective Anomalies**: A set of data instances collectively helps in detecting anomalies. For example, someone is trying to copy data form a remote machine to a local host unexpectedly, an anomaly that would be flagged as a potential cyber attack. The combination of the event from the remote machine and the event from the local host combine to detect the anomaly.
- **Anomalies vs. Noise Removal vs. Novelty Detection**: Novelty detection is concerned with identifying an unobserved pattern in new observations not included in training data — for instance, a sudden interest in a new channel on YouTube during Christmas. Noise Removal (NR) is the process of immunizing analysis from the occurrence of unwanted observations; in other words, removing noise from an otherwise meaningful signal.