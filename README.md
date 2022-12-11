## Anomaly detection on time series: Reinforcement learning from partially labeled data
This is an implementation of the anomaly detection algorithm proposed in this paper: ["Deep Reinforcement Learning for Unknown Anomaly Detection"](https://arxiv.org/pdf/2009.06847.pdf), but in other dataset 'NASA C-MAPSS'

## Dataset
* [NASA_C-MAPSS](https://data.nasa.gov/dataset/C-MAPSS-Aircraft-Engine-Simulator-Data/xaut-bemq)
    
## Experiment
* Set hyperparameters listed in the file `main.py`.
* Run `python main.py`.

## Training log files
* [anomaly_rate_1_log.out] Using the anomaly data rate as it is
* [anomaly_rate_0.5_log.out] Using the anomaly data rate reduced to 0.5
* [anomaly_rate_0.05_log.out] Using the anomaly data rate reduced to 0.05
