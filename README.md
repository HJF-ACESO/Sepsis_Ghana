
# ___"Gene Expression Signatures in Blood that Predict Mortality in a West African Sepsis Cohort Define Host Response Phenotypes"___


Josh G. Chenoweth<sup>1qc</sup>, Carlo Colantuoni<sup>2q</sup>, Deborah A. Striegel<sup>1</sup>, Pavol Genzor<sup>1</sup>, Joost Brandsma<sup>1</sup>, Paul W. Blair<sup>1,3</sup>,Subramaniam Krishnan<sup>1</sup>, Elizabeth Chiyka<sup>1</sup>, Mehran Fazli<sup>1</sup>, Rittal Mehta<sup>1</sup>, Michael Considine<sup>4</sup>, Leslie Cope<sup>4</sup>, Audrey C. Knight<sup>2</sup>, Anissa Elayadi<sup>1</sup>, Anne Fox<sup>5</sup>, Ronna Hertzano<sup>6,7</sup>, Andrew G. Letizia<sup>5</sup>, Alex Owusu-Ofori<sup>8,9</sup>,Isaac Boakey<sup>10</sup>,Albert A. Aduboffour<sup>8</sup>, Daniel Ansong<sup>11,12</sup>, Eno Biney<sup>13</sup>, George Oduro<sup>13</sup>, Kevin L. Schully<sup>14</sup>, Danielle V. Clark<sup>1</sup>

<sup>1</sup> Austere environments Consortium for Enhanced Sepsis Outcomes (ACESO) at Henry M. Jackson Foundation, Bethesda

<sup>2</sup> Dept. of Neurology at Johns Hopkins School of Medicine, Baltimore

<sup>3</sup> Dept. of Pathology at Uniformed Services University, Bethesda
  
<sup>q</sup> Authors contributed equally to this work. 

<sup>c</sup> Corresponding author for additional information and with questions.  


##
Compiled by: __Pavol Genzor__ 

Date: __January 22nd, 2024__

Revision: V1
##

### Summary 

This document contains an example of the code used to analyze data associated with the manuscript. The "transfer learning" procedure consists of three main steps specific to each use where in general:  

* 1. Expression data is subjected to negative matrix factorization using __CoGAPS__
[**[link]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-020-03796-9). 

* 2. Public data of interest is acquired and prepared (*NOTE: To obtain public data please see the original study or contact the corresponding authors.*)

    + Sepsis:
      + Reyes et.al., Nature Medicine, 2020 
      + Tsalik et.al., Science Translational Medicine, 2016
      + Cazalis et.al., Intensive Care Medicine Experimental, 2014  
      
    + COVID-19:
      + Reyes et.al., Science Translational Medicine, 2021

    
* 3. Public data is projected onto the decomposed CoGAPS data using __projectR__
[**[link]**](https://www.bioconductor.org/packages/release/bioc/html/projectR.html) 

* 4. Results are plotted using preferred software.
