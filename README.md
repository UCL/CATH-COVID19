# CATH-COVID19
Data and resources for CATH/Gene3D annotations on SARS-Cov2

As of now it includes:
 - Sequences for 1141 SARS-Cov2 from NCBI, 14 UniProt and 74 PDBe.
 - OrthoMCL clustering results
 - Paths to 4.3 FunFams, both locally and on the web

## CATH

### 4.3 FunFams

On the web: 

[ftp://orengoftp.biochem.ucl.ac.uk/ucbtnb4/](ftp://orengoftp.biochem.ucl.ac.uk/ucbtnb4/)

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
