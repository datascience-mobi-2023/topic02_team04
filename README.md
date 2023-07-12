# team04 of topic02 
 This is the GitHub repository for team04 of the topic02.  
 To refresh your memory on how to manage GitHub, you can find commonly used commands [here](https://github.com/joshnh/Git-Commands). 

### The dataset:

Our dataset is taken from the following paper: <br>

Accurate classification of BRCA1 variants with saturation genome editing
Gregory M. Findlay1, riza M. Daza1, Beth Martin1, Melissa D. Zhang1, Anh P. leith1, Molly Gasperini1, Joseph D. Janizek1, Xingfan Huang1, lea M. Starita1,2* & Jay Shendure1,2,3*
https://www.nature.com/articles/s41586-018-0461-z <br>

The paper is about the homolgy-directed DNA repair gene BRCA1 which plays a crucial role in breast and ovarian cancer. <br>

The researchers goal was to be able to predict the risk for developing such cancer or evaluating the risk of an existant cancer based on the DNA sequence of the BRCA1 gene. <br>

To get the data for this the researchers created variations of the gene, which had single nucleotide variations (SNVs) in the genes most important domains (RING and BRCT). They then screened the proteins that where created based on these SNVs for functionality and gave them function scores. From these function scores the dms_scores in our dataset where derived. <br>

Dms values smaller than 0 mean that the protein works worse than the wildtype (>0 = better). 
The SNVs that lay under a certain dms_score get classified as bin_0 = not funtional. <br>

We chose to focus on these proteins and not on the ones that worked (some of which better than the wildtype), because the goal of this research is to evaluate cancer and cancer risk, not to figure out how humans could be genetically engineered in order to become more cancer resistant. <br>

We were interested in the correlation of the dms_score with:
- secondary structures 
- conserved regions
- and amino acid exchanges.
