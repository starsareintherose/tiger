# tiger
Identifying rapidly-evolving characters in evolutionary data

## Usage
```
****************
TIGER Help:
****************

TIGER: Tree-Independent Generation of Evolutionary Rates

(Developed by Carla Cummins in the lab of James Mc Inerney, NUI Maynooth, Co. Kildare, Ireland)

-Options:

-in        Specify input file. File must be in FastA format and must be aligned prior.
           Datasets with uneven sequence lengths will return an error.

-v         Returns current TIGER version.

-f         Changes output formatting options.
           -f s: sorts sites depending on their agreement score
           -f r: displays rank values rather than bin numbers
           -f s,r: displays sorted ranks (*Be sure to put only a "," NO SPACE!)
           
           Default prints bin numbers unsorted.

-b         Set the number of bins to be used.
           -b <int>: Sites will be placed into <int> number of bins. <int> is a whole number.

           Default is 10

-rl       A list of the rate at each site may be optionally written to a specified
          file. 
          -rl <file.txt> : writes list of the rates at each site to file.txt.

-ptp      Specifies that a PTP test should be run. *Note: this option has a huge 
          effect on running time!

-z        Number of randomisations to be used for the PTP test. 
          -z <int>: each site will be randomised <int> times. <int> is a whole number.

	 Default is 100

-p       Specify p-value which denotes significance in PTP test.
         -p <float>: site will be denoted as significant if p-value is better than <float>.
                     <float> is a floating point number.

         Default is 0.05

-pl      Write a list of p-values to a specified file.
         -pl <file.txt>: writes list of p-values for each site to file.txt.

-u       Specify unknown characters in the alignment. Unknown characters are omitted from 
         site patterns and so are not considered in the analysis.
         -u ?,-,*: defines ?, - and * as unknown characters. (*Be sure to put only a comma
                   between characters, NO SPACE!!)
         
         Default is ? only

```

## System Requirements

- Python 3.x.

## Note

Version 1.04 is made by Guoyi Zhang instead of other original authors. So, please cite this repository.

## Citation

- Cummins, C.A. and McInerney, J.O. (2011) A method for inferring the rate of evolution of homologous characters that can potentially improve phylogenetic inference, resolve deep divergence and correct systematic biases. Systematic Biology 60 (6) 833-844. doi: 10.1093/sysbio/syr064. 

- Zhang G. (2022) TIGER version 1.04. https://github.com/starsareintherose/tiger
