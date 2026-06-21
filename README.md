# Visual object ERP EEG dataset (Kaneshiro et al. 2015)

## Overview

A visual event-related potential (ERP) dataset comprising 124-channel EEG recordings from 10 healthy participants viewing photographs from six object categories (human body, human face, animal body, animal face, fruit/vegetable, and inanimate objects). The dataset contains 5,184 trials collected during a visual object recognition task with 72 images per category, each presented for 500 ms with a 750 ms interstimulus interval. Data were acquired at 62.5 Hz using a high-density geodesic sensor net and are suitable for investigating neural representations of object categories through single-trial EEG classification and representational similarity analysis.

## Dataset Summary

| Property | Value |
|---|---|
| Subjects | 10 |
| Channels | 124 |
| Classes | 6 |
| Trial length | 0.5 s |
| Sampling frequency | 62.5 Hz |
| Sessions | 1 |
| Total trials | 5184 |
| Paradigm | P300 |

## Data Collection Methods

EEG data were acquired from 10 healthy participants using a 124-channel EGI Net Amps 300 system with HydroCel Geodesic Sensor Net montage (GSN-HydroCel-128) at a sampling rate of 62.5 Hz with average reference. Participants viewed 72 photographs from six object categories presented for 500 ms each with a 750 ms interstimulus interval. Data were preprocessed and organized in BIDS format.

## How to Access via MOABB

Install MOABB and load this dataset directly:

```python
from moabb.datasets import Kaneshiro2015
from moabb.paradigms import P300
paradigm = P300()

dataset = Kaneshiro2015()
X, y, metadata = paradigm.get_data(dataset)
```

For more details see the [MOABB documentation](https://moabb.neurotechx.com/) and the
[MOABB dataset page](https://moabb.neurotechx.com/docs/generated/moabb.datasets.Kaneshiro2015.html).

## Citation

If you use this dataset please cite the primary publication:

> DOI: [10.1371/journal.pone.0135697](https://doi.org/10.1371/journal.pone.0135697)

## NEMAR / MOABB Benchmark Collection

This BIDS-formatted dataset was converted from the original data using the
[MOABB](https://moabb.neurotechx.com/) pipeline and re-hosted on
[NEMAR](https://nemar.org/) as part of the MOABB benchmark collection.
The original data and license terms apply — see `dataset_description.json` for details.
