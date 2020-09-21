# CATH-COVID19
Data and resources for CATH/Gene3D annotations on SARS-Cov2

As of now it includes:
 - Sequences for 1141 SARS-Cov2 from NCBI, 14 UniProt and 74 PDBe.
 - OrthoMCL clustering results
 - HMMER3 scan results (SARS-Cov-2 sequences vs CATH v4.3)
 - Paths to 4.3 FunFams, both locally and on the web
 - 3D Models from Phyre, DeepMind and I-TASSER
 
### Update 21/09/20
 
Collected GISAID proteins for ~104k SARS-CoV-2 strains. Separated into constituent FASTA files and aligned using MAFFT7.
The 'Original' SARS-CoV-2 strain is always at the top of the alignment.
 
E - 104,669

M - 104,671

N - 104,706

NS3 - 104,737

NS6 - 104,627

NS7a - 104,625

NS7b - 104,613

NS8 - 104,684

NSP1 - 104,578

NSP10 - 104,669

NSP11 - 104,668

NSP12 - 104,750

NSP13 - 104,670

NSP14 - 104,640

NSP15 - 104,628

NSP16 - 104,697

NSP2 - 104,647

NSP3 - 104,643

NSP4 - 104,681

NSP5 - 104,630

NSP6 - 104,629

NSP7 - 104,630

NSP8 - 104,629

NSP9 - 104,630

Spike - 104,979
 
### Update 27/5/20
 
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
