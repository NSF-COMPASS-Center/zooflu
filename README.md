# ZooFlu Database

<img width="600" height="296" alt="ZooFluIcon_small" src="https://github.com/user-attachments/assets/64ec9fd1-eb97-47a7-a372-35c567ac4dca" />

---

NSF COMPASS Center

Author: Brian R. Wasik, Cornell University

v1.0.0 2026.04.27

Citation of use: https://zenodo.org/records/XXX

# Rationale

Influenza A viruses (IAV) are extremely successful avian-borne viruses that have frequently spilled over into mammalian hosts, resulting in a range of opportune infections, outbreaks, epidemics/epizootics, as well as global human pandemics. Six decades of molecular research has identified IAV mutations with phenotypic effects aligned with this consequential avian-mammal emergence. This broad scientific corpus of mutation signatures is scattered in primary literature, sequence repositories, and select curated databases. We have generated a current effort of a comprehensive 'IAV Emergence Risk' database.

This is an iterative/updated database of influenza A virus mutations of zoonotic risk, manually curated.

The dataset is informed and 'in conversation' with other existing influenza mutation databases, such as  'Flu-Mutation Explorer' (https://flu-gdb.cvr.gla.ac.uk/) and 'FluMut' (https://izsvenezie-virology.github.io/FluMut/docs/output).

An earlier draft database was used as the original 'ground truth' for VILLA analysis, an LLM-powered information extraction pipeline.

Reference for VILLA: https://arxiv.org/abs/2603.23849

GitHub for VILLA: https://github.com/NSF-COMPASS-Center/VILLA

# Format

Mutations are organized for each major/minor IAV viral protein in Comma-Separated Values files (.csv).

The full reference list is provided as both .ris and .bib files.

# Column Definitions

**Viral Protein:** the name of the viral protein product

**Consensus Positon:** the canonical amino acid position in the viral protein

**Reservoir/Neutral Residue:** the residue observed or infered as neutral to the described phenotypic effect, often as present in the avian reservoir lineage

**Risk Residue:** the residue oberserved as confering the phenotypic effect described in the study

**Mutation Anotation:** The numeric-alpha-numeric code for the amino acid residue mutation confering the phenotypic effect described in the study

**IAV Subtype:** the subtype of the IAV background strain observed or manipulated in the given study (when given)

**Study Design:** the framework of the study to define the mutation, e.g. observational, mouse adaptation, exp(erimental) mutagenesis

**Phenotype Summary:** the observed or defined phenotypic effect of the mutation

**Genetic Background:** the specific strain used in this study as background, e.g. a novel isolate, the strain used for mutational experiments, the strain put under passage

**Literature:** the shorthand study citation

**Literature PMID:** the PMID code for the study citation

**Literature doi:** the doi code for the study citation

**Notes:** any extraneous notes added by database currator as to this entry


_NA-specific Column Definitions_

**Consensus Position N2:** the canonical amino acid position based on the N2 alignment of NA

**Position reported:** the amino acid residue position as enumerated in the text of the study (which may not align with major consensus, etc)

# Note of Absence

A mutational database for the hemagglutinin (HA) protein is forthcoming. Literature annotations of HA mutations are fraught with inconsistent formatting and numbering schematics. This makes extraction difficult, and challenges the ability to organize tabular results in a way that may inform by convergence of similar mutations.

Draft _HA-specific column definitions_ to resolve these issues to include:

**HA1/HA2:** the location of the residue in the HA1 or HA2 domains of the HA, as 'position reported' may be HA2 numbering

**Position H1:** the residue position based on H1 number schematic, where applicable

**Position H3:** the residue position based on H3 number schematic, where applicable

**Position H5:** the residue position based on H5 number schematic, where applicable

**Position reported:** the amino acid residue position as enumerated in the text of the study (which may not align with major consensus, etc)

# Stats
v1.0.0

Total references: 374
