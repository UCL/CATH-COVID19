# CATH-COVID19
Data and resources for CATH/Gene3D annotations on SARS-Cov2

As of now it includes:
 - Sequences for 1141 SARS-Cov2 from NCBI, 14 UniProt and 74 PDBe.
 - OrthoMCL clustering results
 - HMMER3 scan results (SARS-Cov-2 sequences vs CATH v4.3)
 - Paths to 4.3 FunFams, both locally and on the web
 - 3D Models from Phyre, DeepMind and I-TASSER
 
 ### New (27/5/20)
 
 COVID_interactors HMMER3 and cath-resolve-hits results. Results in COVID_interactors and new wikipage [`here`](https://github.com/UCL/CATH-COVID19/wiki/COVID-Interactors)

## HMMER3 Scans

You can find HMMER3 results of protein sequences against v4.3 FunFams (seed) for each of the sequence datasets (NCBI, UniProt, PDBe), eg:

```
PDBe/pdbe_covid_sequences.fasta      - sequence files
PDBe/covid_pdbe_seed.crh             - cath-resolve-hits to CATH v4.3 seed alignments
PDBe/covid_pdbe_4.3_filtered_tc.crh  - same as above; only considering hits within inclusion threshold
```

See [`cath-resolve-hits`](https://cath-tools.readthedocs.io/en/latest/tools/cath-resolve-hits/) pages for more details on that tool and data format.


## NCBI: 
Strains divided by country of origin:
- Australia
- Belgium
- China
- India
- Iran
- Italy
- Malaysia
- Nigeria
- Philippines
- Thailand
- USA
- Brazil
- Finland
- Japan
- Nepal
- South_Korea
- Spain
- Sweden
- Taiwan
- Viet_Nam

UniProt has pre-release sequences for 14 ORFs (pre-protease cutting).

PDBe contains 74 protein structures from 25/03/20.


## CATH

### 4.3 FunFams

On the web: [ftp://orengoftp.biochem.ucl.ac.uk/ucbtnb4/](ftp://orengoftp.biochem.ucl.ac.uk/ucbtnb4/)

On the group NIS server: 

```
/cath/people2/ucbtnb4/funfams-4.3/
```

Example: 

```
/cath/people2/ucbtnb4/funfams-4.3/1.20.5.10/
-seed_alignments
-full_alignments
```

In each folder

```
1.20.5.10-FF-000001.faa		
1.20.5.10-FF-000001.faa_nogaps	(Unique to seed_alignments for now)
1.20.5.10-FF-000001.inct_hmm

.faa - FunFam alignment
.faa_nogaps - Unaligned FunFam
.inct_hmm - HMM for the FunFam with inclusion threshold
```
