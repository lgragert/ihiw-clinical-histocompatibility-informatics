# ihiw-clinical-histocompatibility-informatics
IHIW Clinical Histocompatibility Laboratory Informatics project


The key objective of this project is to develop a benchmark of well-vetted antibody analysis cases for grading of human and algorithm performance.

The motivation for this project are multicenter research studies that could benefit from standardized analysis of large-scale raw antibody data from single antigen bead (SAB) panels across centers.

This will have demonstrate an important use case for the HLA antibody markup language (HAML) data standard.

https://github.com/immunomath/haml

Contributors to this project would start with identifying interesting or challenging antibody analysis cases that could compose this benckmark.

HAML converters from CSV exports of antibody assay vendor software (OLI Fusion and Werfen MatchIT) are available at:

https://github.com/IHIW/Converters/tree/master/HAMLConverterPy

This HAML file would contain the raw MFI data and the bead classifications (pos/equiv/neg) made in the vendor software.

Next the participants would based on their analysis (either human expert or automated algorithm) add a second bead classification with the interpretation reason provided. Listings of unacceptable, moderate, and low/unreactive HLA specificities can also be added in interpretation block after the SAB panel data.

This script demonstrates how antibody analysis interpretation results and the reasons behind the interpretations can be stored in this structured HAML data format.

https://github.com/lgragert/haml-interpretation

Once enough antibody analysis cases have accumulated from HLA community contributions in HAML files, we will have a benchmark for grading human analysis proficiency and automated antibody analysis algorithms (rule-based or even potentially AI-based).