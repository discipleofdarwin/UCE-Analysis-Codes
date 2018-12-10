# This code will tell you the number of reads in each of your files

for i in files_which_you_store_all_your_sequence_results/*_R1.fastq.gz; do echo $i; gunzip -c $i | wc -l; done

## Divide the output number by 4 to get number of R1 reads

## R2 uses the same code, just change *_R1 to *_R2
