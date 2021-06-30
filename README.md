# PORTA-generator

First, read [this blog post](https://farkasdilemma.wordpress.com/2017/03/22/a-brief-tutorial-on-porta/).

The python code [stable-set-generator](https://github.com/AustinLBuchanan/PORTA-generator/blob/main/stable-set-generator.ipynb) enumerates all stable sets of a wheel graph (as 0-1 vectors) to a .poi file for use with the PORTA software. 

The python code [stable-set-batch-generator](https://github.com/AustinLBuchanan/PORTA-generator/blob/main/stable-set-batch-generator.ipynb) does a similar task, but generates ninety G(n,p) random graphs: ten at each density 10%, 20%, ..., 90%. It also saves drawings of each graph to png files. Then, it creates a [batch file](https://github.com/AustinLBuchanan/PORTA-generator/blob/main/stable-set.bat) so you don't have to call PORTA ninety times manually. The resulting .poi, .ieq, and .png files are provided [here](https://github.com/AustinLBuchanan/PORTA-generator/tree/main/batch-results).

Note: unfortunately, the graph drawings label the nodes {0, 1, 2, ..., 9} but PORTA labels the variables x_1, x_2, ..., x_10. I didn't bother to fix this. So beware the "off-by-one" errors.

