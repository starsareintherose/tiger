# tiger
Identifying rapidly-evolving characters in evolutionary data

## About Tiger

TIGER is open source software for identifying rapidly evolving sites (columns in an alignment, or characters in a morphological dataset). It can deal with many kinds of data (molecular, morphological etc.). Sites like these are important to identify as they are very often removed or reweighted in order to improve phylogenetic reconstruction. When a site is changing very quickly between taxa it might not hold much phylogenetic information and therefore might simply be a source of noise. Use of TIGER can (a) allow you to see the amount of rapid evolution and noise in your alignment and (b) provide a quick and easy way to remove as many of the “noisy” sites as possible.

TIGER uses conflict between site patterns as a proxy for rapid evolution; that is, a site that does not conflict with other sites in the alignment is generally a very slowly evolving or constant site. A site with lots of conflict is considered rapidly evolving (Cummins & McInerney, Systematic Biology, 2011). TIGER rates the conflict and categorizes the sites based on the rates. In this software the categories are called bins and are user definable (see manual for further details). Bin1 will contain the constant sites and the bin with the highest number will contain the most rapidly evolving sites.

## System Requirements

TIGER is implemented in Python, so it should run on most computer platforms.

For UNIX machines, a working version of Python 3.x is required. On Windows machines, TIGER comes with everything it needs and requires no further installations.

