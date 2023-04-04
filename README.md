# Inhibition of Hepatits B virus

The model uses ord2vec, a natural language processing technique to represent SMILES strings. The model was trained on over <4000 small molecules with associated experimental HBV inhibition data (IC50) to classify compounds as HBV inhibitors (IC50 <= 1 uM) or non-inhibitors. Data was gathered from the public repository ChEMBL.

## Identifiers

* EOS model ID: `eos8lok`
* Slug: `s2dv-hbv`

## Characteristics

* Input: `Compound`
* Input Shape: `Single`
* Task: `Classification`
* Output: `Experimental value`
* Output Type: `Float`
* Output Shape: `Single`
* Interpretation: Probability of inhibition of HBV

## References

* [Publication](https://pubmed.ncbi.nlm.nih.gov/35062019/)
* [Source Code](https://github.com/NTU-MedAI/S2DV)
* Ersilia contributor: [emmakodes](https://github.com/emmakodes)

## Citation

If you use this model, please cite the [original authors](https://pubmed.ncbi.nlm.nih.gov/35062019/) of the model and the [Ersilia Model Hub](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff).

## License

This package is licensed under a GPL-3.0 license. The model contained within this package is licensed under a Apache-2.0 license.

Notice: Ersilia grants access to these models 'as is' provided by the original authors, please refer to the original code repository and/or publication if you use the model in your research.

## About Us

The [Ersilia Open Source Initiative](https://ersilia.io) is a Non Profit Organization ([1192266](https://register-of-charities.charitycommission.gov.uk/charity-search/-/charity-details/5170657/full-print)) with the mission is to equip labs, universities and clinics in LMIC with AI/ML tools for infectious disease research.

[Help us](https://www.ersilia.io/donate) achieve our mission!