# Assemble your UCE reads using ABySS 

phyluce_assembly_assemblo_abyss \
    --config path/to/your/config/file/Abyss.conf \
    --output where/you/want/to/store/the/data/folder_name \
    --kmer 35 \  <-between 55~65 recommanded by creator of phyluce 
    --subfolder split-adapter-quality-trimmed \
    --cores 2 \
    --clean \
    --log-path path/to/where/you/want/the/log/files/log_folder
    
    ## Sample config file
    
    [samples]
sample_name1:/folder/path/to/trimmed/sample
sample_name2:/folder/path/to/trimmed/sample
sample_name3:/folder/path/to/trimmed/sample
