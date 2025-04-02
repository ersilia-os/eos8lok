# Inhibition of Hepatits B virus

The model uses Word2Vec, a natural language processing technique to represent SMILES strings. The model was trained on over <4000 small molecules with associated experimental HBV inhibition data (IC50) to classify compounds as HBV inhibitors (IC50 <= 1 uM) or non-inhibitors. Data was gathered from the public repository ChEMBL.

This model was incorporated on 2023-03-24.

## Information
### Identifiers
- **Ersilia Identifier:** `eos8lok`
- **Slug:** `s2dv-hbv`

### Domain
- **Task:** `Annotation`
- **Subtask:** `Activity prediction`
- **Biomedical Area:** `Hepatitis B`
- **Target Organism:** `Hepatitis B virus`
- **Tags:** `Antiviral activity`, `IC50`, `HBV`, `ChEMBL`

### Input
- **Input:** `Compound`
- **Input Dimension:** `1`

### Output
- **Output Dimension:** `1`
- **Output Consistency:** `Fixed`
- **Interpretation:** Probability of inhibition of HBV (IC50 < 1uM)

Below are the **Output Columns** of the model:
| Name | Type | Direction | Description |
|------|------|-----------|-------------|
| hbv_prob | float | high | Probability that a compound inhibits the Hepatitis B virus |


### Source and Deployment
- **Source:** `Local`
- **Source Type:** `External`
- **DockerHub**: [https://hub.docker.com/r/ersiliaos/eos8lok](https://hub.docker.com/r/ersiliaos/eos8lok)
- **Docker Architecture:** `AMD64`, `ARM64`
- **S3 Storage**: [https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos8lok.zip](https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos8lok.zip)

### Resource Consumption


### References
- **Source Code**: [https://github.com/NTU-MedAI/S2DV](https://github.com/NTU-MedAI/S2DV)
- **Publication**: [https://pubmed.ncbi.nlm.nih.gov/35062019/](https://pubmed.ncbi.nlm.nih.gov/35062019/)
- **Publication Type:** `Peer reviewed`
- **Publication Year:** `2022`
- **Ersilia Contributor:** [emmakodes](https://github.com/emmakodes)

### License
This package is licensed under a [GPL-3.0](https://github.com/ersilia-os/ersilia/blob/master/LICENSE) license. The model contained within this package is licensed under a [Apache-2.0](LICENSE) license.

**Notice**: Ersilia grants access to models _as is_, directly from the original authors, please refer to the original code repository and/or publication if you use the model in your research.


## Use
To use this model locally, you need to have the [Ersilia CLI](https://github.com/ersilia-os/ersilia) installed.
The model can be **fetched** using the following command:
```bash
# fetch model from the Ersilia Model Hub
ersilia fetch eos8lok
```
Then, you can **serve**, **run** and **close** the model as follows:
```bash
# serve the model
ersilia serve eos8lok
# generate an example file
ersilia example -n 3 -f my_input.csv
# run the model
ersilia run -i my_input.csv -o my_output.csv
# close the model
ersilia close
```

## About Ersilia
The [Ersilia Open Source Initiative](https://ersilia.io) is a tech non-profit organization fueling sustainable research in the Global South.
Please [cite](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff) the Ersilia Model Hub if you've found this model to be useful. Always [let us know](https://github.com/ersilia-os/ersilia/issues) if you experience any issues while trying to run it.
If you want to contribute to our mission, consider [donating](https://www.ersilia.io/donate) to Ersilia!
