## Artemisia tridentata mixed-ploidy SNP calling 

This notebook is all my notes for attempting SNPcalling on mixed ploidy populations using ARTR

#### Steps / Thoughts:

- Match fq names to Bryce's names on ARTR_pop: *nameMatch_readCount.ipynb*
- Assess read count in each fq and assess across subspecies and ploidy: *nameMatch_readCount.ipynb*
    - 4n should have double reads but coverage should be the same as 2n after snp call
    - Cite *Jighly 2021, Mol Ecol Res.* 
- install GATK and make notes on how to do it and different options: *0-installing-GATK-and-notes.ipynb*
- map fq to draft assembly (Melton et al 2021, Ecol&Evol) using bwa-concensus: 3mapping_sagebrush.ipynb
- call variants with GATK: 
- filter snps (need to really think about this): 
- run mixed-ploidy entropy: *6entropy_sagebrush.ipynb* 

#### post snp calling and entropy:
- adjust genotype liklihoods based off simulations: *examples/mixed_ploidy_sim.html*
- download env data: CWD and Bryce's code
- use RF to predict ssp and ploidy based off env data alone
