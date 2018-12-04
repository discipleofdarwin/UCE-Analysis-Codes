## Trimming using illumiprocessor:

illumiprocessor --input /full/path/to/folder/containing/all/sequence/results\
--output clean-fastq #can be customize with new path\
--config illumiprocessor.conf\ 
--trimmomatic /full/path/to/trimmomatic.jar\ 
**This line is added to make sure program findes trimmomatic, default path might not work on your personal computer.**\ 
--r1-pattern .*_R1 --r2-pattern .*_R2\  
**. indicates any character while * means repeats however many times, it's a substitute for all your file name infront of R1 and R2 which indicates which foward and reverse read. No need to change! At the same time, do not change the file name of your raw sequence at this step!!!**


illumiprocessor.conf template for dual index:

[adapters]
i7:CAAGCAGAAGACGGCATACGAGAT*GTGACTGGAGTTCAGACGTGT
i5:AATGATACGGCGACCACCGAGATCTACAC*ACACTCTTTCCCTACACGACGCTCTT

[tag sequences]  
i7-B3:CAATGTGG    
i7-B4:CGGATTGA   
i5-B3:AAGTGTCG
i5-B4:TTCGCAGT
**Left hand is just shorthand abbreviations, can be set as anything, but always start with alphabet**

[tag map]
B3_S72:i7-B3,i5-B3
B4_S73:i7-B4,i5-B4

[names]   
B3_S72:B3
B4_S73:B4
**Use this area to change output file name to which ever you desire**
