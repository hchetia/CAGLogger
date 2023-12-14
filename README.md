# CAGLogger

**Broad Goal:**
Taking the HTT genotyping based on the Ciosi Assay one step further by detecting the detecting CAG repeats that are extremely long (> 113). We use an in-house alignment free detection program and tally CAG repeats from targeted MiSeq data from genomic DNA. 

**A. Define Type A Error**: 
1 base substitution per one CAG repeat (concept of mismatches or gap not applied here).  
**B. Define Type B Error:** 
Two consecutive CAG repeats with Type A Error.  
**C. Error Cut-off**:   
Maximum Type A Error allowed per CAG stretch is 3. Maximum threshold for Type B Error per CAG stretch is 1.  DONE
**D. What are the inputs?**
FastQ files (generated using the protocol in References Section).  
**E. What are the outputs?**
A frequency file of CAG repeats and their frequencies [*Adjust for 3 repeats*]. DONE (gotta minus 3)
A frequency distribution plot. DONE
A metric file with percentage of extremely long CAG repeats. DONE
**F. References:**
Targeted Miseq data from HTT exon1 CAG repeat (Strategy- [Ciosi et al 2021](https://content.iospress.com/articles/journal-of-huntingtons-disease/jhd200433), [Matlik et al 2023](https://www.biorxiv.org/content/10.1101/2023.04.24.538082v2.abstract)).
