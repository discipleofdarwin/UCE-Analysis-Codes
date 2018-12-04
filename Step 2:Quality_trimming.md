## Trimming using illumiprocessor:

illumiprocessor --input /full/path/to/folder/containing/all/sequence/results <br/>
--output clean-fastq #can be customize with new path <br/>
--config illumiprocessor.conf <br/> 
--trimmomatic /full/path/to/trimmomatic.jar <br/> 
**This line is added to make sure program findes trimmomatic, default path might not work on your personal computer.** <br/> 
--r1-pattern .*_R1 --r2-pattern .*_R2 <br/> 
**. indicates any character while * means repeats however many times, it's a substitute for all your file name infront of R1 and R2 which indicates which foward and reverse read. No need to change! At the same time, do not change the file name of your raw sequence at this step!!!**


illumiprocessor.conf template for dual index:

[adapters] <br/>
i7:CAAGCAGAAGACGGCATACGAGAT*GTGACTGGAGTTCAGACGTGT <br/>
i5:AATGATACGGCGACCACCGAGATCTACAC*ACACTCTTTCCCTACACGACGCTCTT <br/>

[tag sequences] <br/>  
i7-B3:CAATGTGG 
i7-B4:CGGATTGA <br/>   
i5-B3:AAGTGTCG <br/>
i5-B4:TTCGCAGT <br/>
**Left hand is just shorthand abbreviations, can be set as anything, but always start with alphabet**

[tag map] <br/>
B3_S72:i7-B3,i5-B3 <br/>
B4_S73:i7-B4,i5-B4 <br/>

[names]   
B3_S72:B3 <br/>
B4_S73:B4 <br/>
**Use this area to change output file name to which ever you desire**
