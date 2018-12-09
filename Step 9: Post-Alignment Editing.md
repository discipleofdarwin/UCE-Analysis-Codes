# Post-Alignment Editing

## Remove loci name from each alignment sequences

phyluce_align_remove_locus_name_from_nexus_lines \\<br/>
    --alignments /path/to/folder/with/all/alignments \\<br/>
    --output /specify/path/for/output/ \\<br/>
    --cores 2 <-specify number of cores<br/>


## Selecting alignments that include at least certain percentages of taxa 

phyluce_align_get_only_loci_with_min_taxa \\<br/>
    --alignments /path/to/alignment/folder \\<br/>
    --taxa 46 \\ <-total number of taxa<br/>
    --percent 0.75 \\ <-percentage cutoff<br/>
    --output /specify/output/file/path \\<br/>
    --cores 2 <-specify number of cores<br/>
    
## Selecting alignment with specific length cutoff

phyluce_align_filter_alignments \\<br/>
    --alignments /path/to/alignment/folder \\<br/>
    --output /specify/output/path \\<br/>
    --input-format nexus \\ <-specify input file format <br/>
    --containing-data-for genus_species genus_species2 \\ <-list of all your specimen name here<br/>
    --min-length 400 \\ <-set minimum sequence length cutoff<br/> 
    --log-path /path/to/log/folder<br/>



