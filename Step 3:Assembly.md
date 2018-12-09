# Assemble your UCE reads using ABySS 

phyluce_assembly_assemblo_abyss \\<br/>
    --config path/to/your/config/file/Abyss.conf \\<br/>
    --output where/you/want/to/store/the/data/folder_name \\<br/>
    --kmer 35 \  <-between 55~65 recommanded by creator of phyluce<br/>
    --subfolder split-adapter-quality-trimmed \\<br/>
    --cores 2 \\<br/>
    --clean \\<br/>
    --log-path path/to/where/you/want/the/log/files/log_folder

## Sample config file
    
\[samples]
sample_name1:/folder/path/to/trimmed/sample
sample_name2:/folder/path/to/trimmed/sample
sample_name3:/folder/path/to/trimmed/sample
