# receptor_utils

Some tools I find useful for working with Ig receptor sequences, including support for allele sequence naming and 
the creation of custom IgBlast databases. Please see the [documentation](https://williamdlees.github.io/receptor_utils/_build/html/introduction.html)
for further details.

Changes in version 0.0.46:
- fix issue with naming of D novel alleles - this could cause existing alleles to be named as novel by the utilities

Changes in version 0.0.45:
- added dependency for biopython version >=1.81

Changes in version 0.0.44:
- minor fix to novel allele naming
- fixed a bug that prevented sequence subsets being shown by identical_seqs

Changes in version 0.0.43:
- remove dependency on deprecated Bio.pairwise2
- improve naming of insertions, e.g. IGHV1-2*03_i7g_i7a would now be IGHV1-2*03_i7ga

Changes in version 0.0.42:
- better handling of long target sequences

Changes in version 0.0.41:
- annotate_j: fix issue with processing FASTA input

Changes in version 0.0.40:
- The submodule name receptor_utils.number_ighv has been changed to receptor_utils.number_v to reflect its wider scope. The old name will continue
to work for the time being but will raise a deprecation warning.
- In receptor_utils.simple_bio_seq, write_fasta(seqs, filename) has become write_fasta(filename, seqs) for consistency with write_csv. The old
calling pattern will continue to work for the time being but will raise a deprecation warning.

Changes in version 0.0.39:
- annotate_j and make_igblast_ndm will now accept a germline set in AIRR Community JSON format, as an alternative to providing the set in FASTA format.

Changes in version 0.0.38:
- Improve reporting of issues with conserved residues
- Change URL for fetching IMGT reference sets to use https





