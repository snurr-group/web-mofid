# MOFid website

The MOFid code has many utilities, two of which can be run in your web browser:

1. **Generate a MOFid/MOFkey**: The [ID tool](sbu.html) allows you to deconstruct a MOF into its building blocks for the purposes of generating a MOFid/MOFkey, requiring only a CIF as the input.
2. **Run queries on the CoRE MOF database**: The [Search Tool](searchdb.html) runs queries against the CoRE MOF 2019-ASR [database](https://zenodo.org/record/3677685) of ~15,000 MOFs.

## Tips for Generating MOFids/MOFkeys

To generate an accurate MOFid/MOFkey, disorder should not be present in the structure. The ID tool will attempt to automatically remove solvent from the framework, if present. Molecules or ions that are not part of the framework should be manually removed from the CIF before generating the MOFid/MOFkey. For newly reported MOFs, we recommend reporting the shorter MOFkey alongside the common name and, optionally, reporting the longer MOFid in the Supporting Information. Several visualization options are provided for the uploaded CIF as well.

Please note that the tools may require a few minutes to run the analysis after you click "submit." All analysis is performed locally on your own machine. If the analysis stalls and does not complete after a few minutes for some reason, please refresh the page and try again.

If you receive an error message of "Exception thrown, see JavaScript console," it is often because the CIF parser is having trouble reading the formatting of your CIF. Try reading in your CIF in a program like [VESTA](https://jp-minerals.org/vesta/en/download.html) and re-exporting it as a CIF to see if that resolves the issue.

## Further Information

The main project [GitHub repository](https://github.com/snurr-group/mofid) includes a downloadable C++/Python code, [example CIFs for analysis](https://github.com/snurr-group/mofid/tree/master/Resources/TestCIFs), and credits for third-party software.

This work is supported by the U.S. Department of Energy, Office of Basic 
Energy Sciences, Division of Chemical Sciences, Geosciences and 
Biosciences through the Nanoporous Materials Genome Center under award 
DE-FG02-17ER16362.
