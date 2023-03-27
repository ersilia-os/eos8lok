# Inhibition of Hepatits B virus

The model adopts a natural language processing technique to analyze compound SMILES strings, enabling an accurate representation of the relationship between compounds and their substructures. This technique helps the model predict inhibitory effects on HBV, verified by wet-lab experiments. This model provides a new perspective on the prediction of compound properties for anti-HBV drugs to improve hepatitis B diagnosis and human health in the future.

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
* Interpretation: This model receives smiles as input and returns as output the probability of the inhibitory effect of compounds on Hepatitis B Virus. 

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