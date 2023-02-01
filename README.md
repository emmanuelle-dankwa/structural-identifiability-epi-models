# Documentation

The input code in this repository reproduces the results in the manuscript:

Emmanuelle A. Dankwa, Andrew F. Brouwer, Christl A. Donnelly. Structural identifiability of compartmental models for infectious disease transmission is influenced by data type. Epidemics, Vol. 41 (2022), Article 100643 [Link to paper](https://www.sciencedirect.com/science/article/pii/S1755436522000834#sec0050).

In this work, we performed structural identifiability analysis of 26 compartmental models for infectious disease transmission uising the SIAN web application [(Hong et al., 2019)](#1): [https://maple.cloud/app/6509768948056064](https://maple.cloud/app/6509768948056064). The algorithm on which SIAN is based is explained by [Hong et al. (2020)](#2). 

The repository has four parent folders for the four main compartmental structures studied: 

* `SIR`: for the Suceptible-Infected-Recovered models
* `SLIR`: for the Suceptible-Latent-Infected-Recovered models
* `SLIRQ`: for the Suceptible-Latent-Infected-Recovered-Remission models
* `SLIR-SLI`: for the vector-borne disease transmission models with SLIR for hosts and SLI for vectors 

Each parent folder contains 

1)  an input file  `stucture_SIAN_input.txt`, where `structure` is one of `SIR`, `SLIR`, `SLIRQ` or `SLIR-SLI`: contains the text-based input code for analyses performed on `structure`-based models at all stages 

and 

2) four folders: 

* `stage_one`: contains outputs for analyses at stage one (single outputs, unknown parameters)
* `stage_two`: contains outputs for analyses at stage two (single outputs, natural history parameters assumed known)
* `stage_three`: contains outputs for analyses at stage three (multiple outputs, unknown parameters)
* `stage_four`: contains outputs for analyses at stage four (multiple outputs, natural history parameters assumed known)

# Reproduce results

To reproduce results, copy and paste the relevant input code in the input field in the SIAN web application and click "Determine".


# Queries

Queries and suggestions are always welcome. Please email Emmanuelle at emmanuelledankwa@gmail.com with such. 

# License

MIT License


## References
<a id="1">[1]</a> 
Hong, H., Ovchinnikov, A., Pogudin, G., Yap, C., 2019. SIAN: software for structural identifiability analysis of ODE models. Bioinformatics 35, 2873–2874. \
<a id="2">[2]</a>
Hong, H., Ovchinnikov, A., Pogudin, G., Yap, C., 2020. Global identifiability of differential models. Communications on Pure and Applied Mathematics 73, 1831–1879.
