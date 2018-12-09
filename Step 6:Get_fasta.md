# This code will help you pull out the UCE loci in .fasta format 

## Complete matrix(Loci shared by all)

phyluce_assembly_get_fastas_from_match_counts \\<br/>
    --contigs /path/to/contig/file \\<br/>
    --locus-db /path/to/probe.matches.sqlite \\<br/>
    --match-count-output /path/to/edited/.conf/file \\<br/>
    --output /path/to/where/you/want/the/output/dataset1.fasta<br/>


## Incomplete matrix(include unique UCE loci)

phyluce_assembly_get_fastas_from_match_counts \\<br/>
    --contigs /path/to/contig/file \\<br/>
    --locus-db /path/to/probe.matches.sqlite \\<br/>
    --match-count-output /path/to/edited/.conf/file \\<br/>
    --incomplete-matrix /path/to/incomplete/data/generated/in/last/section/dataset1.incomplete \\<br/>
    --output /path/to/where/you/want/the/output/dataset1.fasta<br/>
