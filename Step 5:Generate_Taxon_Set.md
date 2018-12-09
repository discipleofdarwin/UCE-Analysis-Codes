# These codes will make taxon set meaning they will generate file with sample name and UCE loci that will be pulled out for later steps

## include unique loci

phyluce_assembly_get_match_counts \\<br/>
    --locus-db /path/to/probe.matches.sqlite \\<br/>
    --taxon-list-config /path/to/dataset.conf \\<br/>
    --taxon-group 'dataset1' \\<br/>
    --output /path/to/an/output/location/of/your/choosing \\<br/>
    --incomplete-matrix<br/>


## only loci shared by "ALL" 
phyluce_assembly_get_match_counts \\<br/>
    --locus-db /path/to/probe.matches.sqlite \\<br/>
    --taxon-list-config /path/to/datasets.conf \\<br/>
    --taxon-group 'dataset1' \\<br/>
    --output /path/to/uce/taxon-set1/dataset1.conf<br/>


## example dataset.conf format

[dataset1]<br/>
list of your sample names
