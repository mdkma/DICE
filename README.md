# DICE: Data-Efficient Clinical Event Extraction with Generative Models

Source code and data for ACL 2023 main conference paper [DICE: Data-Efficient Clinical Event Extraction with Generative Models](https://derek.ma/DICE).

## Quick Start

```
# Training 
sh scripts/train.sh

# Evaluating a saved model
sh scritps/eval.sh
```

Use the following config file in the scripts for corresponding experiment:
* `config/config_multitask_maccrobat_ET`: train standalone mention identification module with slding window
* `config/config_multitask_maccrobat_ET-ED`: train event detection module with aux mention identification module and mention marker
* `config/config_multitask_maccrobat_ET-EAE`: train event argument extraction module with aux mention identification module and mention marker

## Dataset: MACCROBAT-EE

Check `maccrobat/Data` folder for the entire event extraction dataset with argument annotation.

## Environment

```
# Install conda environment
conda env create -f env.yml
```

## Cite

```
@inproceedings{ma-etal-2023-dice,
    title = "DICE: Data-Efficient Clinical Event Extraction with Generative Models",
    author = "Ma, Mingyu Derek and Taylor, Alexander K. and Wang, Wei and Peng, Nanyun",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://arxiv.org/abs/2208.07989",
}
```