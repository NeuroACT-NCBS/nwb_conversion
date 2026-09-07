# NWB conversion Workflow

This repository contains the workflow, example metadata, and notebooks for converting trodes recordings to NWB format.

The actual NWB conversion is performed using the
[`LorenFrankLab/trodes_to_nwb`](https://github.com/LorenFrankLab/trodes_to_nwb)
package.

This repo has been created mainly a reference labeling and organising format need to
prepare metadata YAML files and convert recording sessions to NWB using the
same format and workflow that we currently follow.

## What is included

### Example metadata

`20250818_na20_metadata.yml`

An example YAML file showing the metadata format currently used for our
recordings.

It can be used as a reference when preparing metadata for new sessions.

### Notebooks

The `notebook/` folder contains notebooks for different stages of the workflow:

- `NWb_conversion.ipynb`  
  Convert Trodes recording data to NWB.

- `nwb_timestamps_mapping.ipynb`  
  Compare epoch and video timestamps and correct timestamp alignment when
  required.

- `setup.ipynb`  
  Setup required before inserting NWB files into Spyglass.

- `Trial_for_spyglass_insertion.ipynb`  
  Insert NWB files into Spyglass and check the inserted data.

## Metadata preparation

The metadata YAML contains information related to the recording session,
including:

- experiment and session information
- animal information
- camera information
- task and epoch information
- StateScript log files
- video files
- behavioural events

The example YAML in this repository can be used as a starting reference for
the expected format and naming conventions.

## NWB conversion

NWB creation is performed using the
[`LorenFrankLab/trodes_to_nwb`](https://github.com/LorenFrankLab/trodes_to_nwb)
package.

Please refer to the original repository for installation instructions and
details about the conversion package.


