## DPLAN-Implementation
This is an implementation of the anomaly detecion algorithm proposed in this paper: ["Deep Reinforcement Learning for Unknown Anomaly Detection"](https://arxiv.org/pdf/2009.06847.pdf). Please let me know if there are any bugs in my code. Thank you:)

## Dataset
* [NASA_C-MAPSS](https://data.nasa.gov/dataset/C-MAPSS-Aircraft-Engine-Simulator-Data/xaut-bemq)

## Loading Dataset
* Datasets are preprocessed in the same way that described in the original paper.
* One raw dataset will generate a set of unknown anomaly detection dataset, according to different known anomaly classes in the training dataset.
  * For example, UNSW-NB15:
    
    [![](https://mermaid.ink/img/eyJjb2RlIjoiZ3JhcGggTFJcbiAgICBzdGFydFtVTlNXLU5CMTVdLS0-dHJhaW5bVHJhaW4gRGF0YXNldF1cbiAgICBzdGFydC0tPnRlc3RbVGVzdCBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IEFuYWx5c2lzLS0-QW5hbHlzaXNbQW5hbHlzaXMgVW5rbm93biBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IEJhY2tkb29yLS0-QmFja2Rvb3JbQmFja2Rvb3IgVW5rbm93biBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IERvUy0tPkRvU1tEb1MgVW5rbm93biBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IE90aGVyLS0-Li4uIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZ3JhcGggTFJcbiAgICBzdGFydFtVTlNXLU5CMTVdLS0-dHJhaW5bVHJhaW4gRGF0YXNldF1cbiAgICBzdGFydC0tPnRlc3RbVGVzdCBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IEFuYWx5c2lzLS0-QW5hbHlzaXNbQW5hbHlzaXMgVW5rbm93biBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IEJhY2tkb29yLS0-QmFja2Rvb3JbQmFja2Rvb3IgVW5rbm93biBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IERvUy0tPkRvU1tEb1MgVW5rbm93biBEYXRhc2V0XVxuICAgIHRyYWluLS1Lbm93IE90aGVyLS0-Li4uIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifSwidXBkYXRlRWRpdG9yIjpmYWxzZX0)

  * Accordingly, the paths of datasets to be loaded are set in the following way:
    
[![](https://mermaid.ink/img/eyJjb2RlIjoiZ3JhcGggVEQ7XG4gICAgc3RhcnRbZGF0YV9wYXRoXS0tPmRzMVtVTlNXLU5CMTVdXG4gICAgc3RhcnQtLT5kczJbQ292ZXJUeXBlXVxuICAgIHN0YXJ0LS0-ZHM0Wy4uLl1cbiAgICBkczEtLT5BbmFseXNpc1xuICAgIGRzMS0tPkJhY2tkb29yXG4gICAgZHMxLS0-Li4uXG4gICAgZHMxLS0-dDFbdGVzdCBkYXRhc2V0XVxuICAgIGRzMi0tPmNvdHRvbndvb2RcbiAgICBkczItLT5kb3VnbGFzLWZpclxuICAgIGRzMi0tPnQyW3Rlc3QgZGF0YXNldF0iLCJtZXJtYWlkIjp7InRoZW1lIjoiZGVmYXVsdCJ9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlfQ)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoiZ3JhcGggVEQ7XG4gICAgc3RhcnRbZGF0YV9wYXRoXS0tPmRzMVtVTlNXLU5CMTVdXG4gICAgc3RhcnQtLT5kczJbQ292ZXJUeXBlXVxuICAgIHN0YXJ0LS0-ZHM0Wy4uLl1cbiAgICBkczEtLT5BbmFseXNpc1xuICAgIGRzMS0tPkJhY2tkb29yXG4gICAgZHMxLS0-Li4uXG4gICAgZHMxLS0-dDFbdGVzdCBkYXRhc2V0XVxuICAgIGRzMi0tPmNvdHRvbndvb2RcbiAgICBkczItLT5kb3VnbGFzLWZpclxuICAgIGRzMi0tPnQyW3Rlc3QgZGF0YXNldF0iLCJtZXJtYWlkIjp7InRoZW1lIjoiZGVmYXVsdCJ9LCJ1cGRhdGVFZGl0b3IiOmZhbHNlfQ)
    
## Experiment
* Set hyperparameters listed in the file `main.py`.
* Run `python main.py`.

## Training log files
* [anomaly_rate_1_log.out] Using the anomaly data rate as it is
* [anomaly_rate_0.5_log.out] Using the anomaly data rate reduced to 0.5
* [anomaly_rate_0.05_log.out] Using the anomaly data rate reduced to 0.05
