## About The Project
Having an interest in computational neuroscience and biopsychology, I thought that it would be interesting to embark on some data analysis with EEG and iEEG data. This project thus far has taught me things like bandpass filtering, conducting independent component analysis, epoching, and conducting time-frequency analysis. 

This project is still a work in progress as the modular pipeline for the data is still in progress, using autoreject. Currently, only the [single session analysis](https://github.com/ethancqy/portfolio/blob/main/Working%20Memory%20Load%20Analysis%20via%20EEG%20and%20iEEG%20Signals%20in%20Sternberg%20Task/Single%20Session%20Analysis.ipynb) is available, detailing some limitations as well which could hinder more positive success markers.

## Dataset
The dataset was taken from [OpenNeuro](https://openneuro.org/datasets/ds004752/versions/1.0.1) and is structured as such:

```
ds004752/
├── CHANGES
├── dataset_description.json
├── derivatives/
│   ├── sub-01/
│   │   └── beamforming/
│   │       └── sub-01-task-verbalWM-LCMVsources.mat
│   └── ...
├── participants.json
├── participants.tsv
├── README
├── sub-01/
│   ├── ses-01/
│   │   ├── eeg/
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_channels.tsv
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_eeg.edf
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_eeg.json
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_events.json
│   │   │   └── sub-01_ses-01_task-verbalWM_run-01_events.tsv
│   │   ├── ieeg/
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_channels.tsv
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_electrodes.json
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_electrodes.tsv
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_events.json
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_events.tsv
│   │   │   ├── sub-01_ses-01_task-verbalWM_run-01_ieeg.edf
│   │   │   └── sub-01_ses-01_task-verbalWM_run-01_ieeg.json
│   │   └── sub-01_ses-01_scans.tsv
│   ├── ...
│   └── sub-01_sessions.tsv
└── ...
```

The dataset description, extracted from the README, is as follows:

> We present an electrophysiological dataset recorded from fifteen subjects during a verbal working memory task. Subjects were epilepsy patients undergoing intracranial monitoring for localization of epileptic seizures. Subjects performed a modified Sternberg task in which the encoding of memory items, maintenance, and recall were temporally separated. The dataset includes simultaneously recorded scalp EEG with the 10-20 system, intracranial EEG (iEEG) recorded with depth electrodes, waveforms, and the MNI coordinates and anatomical labels of all intracranial electrodes. The dataset includes also reconstructed virtual sensor data that were created by performing LCMV beamforming on the EEG at specific brain regions including, temporal superior lobe, lateral prefrontal cortex, occipital cortex, posterior parietal cortex, and Broca. Subject characteristics and information on sessions (set size, match/mismatch, correct/incorrect, response, response time for each trial) are also provided. This dataset enables the investigation of working memory by providing simultaneous scalp EEG and iEEG recordings, which can be used for connectivity analysis, alongside reconstructed beamforming EEG sources that can enable further cognitive analysis such as replay of memory items.

## Project Structure
Currently, the project is structured very simply with only a jupyter notebook that conducts exploratory data analysis on the dataset.

```
Working Memory Load Analysis via EEG and iEEG Signals in Sternberg Task/
├── README.md
└── Single Session Analysis.ipynb
```

## Notes
While the notebook indicates that there will be a separate project with a pipeline, it is still a work in progress.
