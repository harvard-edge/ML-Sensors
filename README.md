# Machine Learning Sensors
This repository contains resources related to the machine learning (ML) sensor datasheet. The ML sensor is a new paradigm for edge devices which segregates the sensor input data and ML processing from the wider system at the hardware level while providing a thin interface that mimics traditional sensors in functionality. An in-depth description of ML sensors is provided [here](https://arxiv.org/abs/2206.03266).

![ML_sensor](https://github.com/harvard-edge/ML-Sensors/blob/main/figs/mlsensor.png)

## Datasheet
The ML sensor datasheet, as outlined in "Datasheets for Machine Learning Sensors," provides an overview of both the ML and hardware characteristics relevant to the device. This builds upon prior work focusing on specific aspects of the model pipeline (e.g., [datasheets for datasets](https://arxiv.org/abs/1803.09010), [data nutrition labels](https://arxiv.org/abs/1805.03677), [model cards](https://arxiv.org/abs/1810.03993)), and the existing industry-standard for providing a datasheet for hardware sensors. Related works are summarized in the table below.

![related](https://github.com/harvard-edge/ML-Sensors/blob/main/figs/related.png)

The items listed within the proposed datasheet include but are not limited to: environmental impact, communication protocol, device diagrams, dataset attributes, model characteristics, end-to-end performance analysis, compliance and certifications, and hardware specifications. Including these details in an easy-to-digest datasheet provides many benefits as it provides transparency, explainability, and auditability. The ML sensor paradigm itself provides added privacy, security, and user-friendliness, which empowers end-users to more easily control their data, as well as for developers to more easily integrate ML capabilities into sensing devices without requiring ML expertise.

The proposed structure of the ML sensor datasheet is shown below.

![datasheet](https://github.com/harvard-edge/ML-Sensors/blob/main/figs/datasheet_template.png)

A full example datasheet for a person detection ML sensor is provided [here](https://github.com/harvard-edge/ML-Sensors/blob/main/open_source_datasheet.pdf).

If you use or reference an ML sensor datasheet in a publication, please cite:
```
@misc{stewart2023datasheets,
      title={Datasheets for Machine Learning Sensors}, 
      author={Matthew Stewart and Pete Warden and Yasmine Omri and Shvetank Prakash and Joao Santos and Shawn Hymel and Benjamin Brown and Jim MacArthur and Nat Jeffries and Brian Plancher and Vijay Janapa Reddi},
      year={2023},
      eprint={2306.08848},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```

If you use an ML sensor in a publication, please cite:
```
@misc{warden22MLSensors,
  doi = {10.48550/ARXIV.2206.03266},
  url = {https://arxiv.org/abs/2206.03266},
  author = {Warden, Pete and Stewart, Matthew and Plancher, Brian and Banbury, Colby and Prakash, Shvetank and Chen, Emma and Asgar, Zain and Katti, Sachin and Reddi, Vijay Janapa},
  keywords = {Machine Learning (cs.LG), Hardware Architecture (cs.AR), FOS: Computer and information sciences, FOS: Computer and information sciences},
  title = {Machine Learning Sensors},
  publisher = {arXiv},
  year = {2022},
  copyright = {Creative Commons Attribution 4.0 International}
}
```

To get involved, check out our [website](http://mlsensors.org) or join our [Google group](mailto:ml-sensors@googlegroups.com).
