# pypdb

A basic wrapper for the Protein Data Bank (PDB) xml-based API. This can be used to perform searched for PDB IDs matching some criteria, as well as to look up information associated with specific PDB IDs

*Written by William Gilpin for Stanford AP315, Spring 2015.*


## Installation

   $ pip install pypdb

This code works on Python 3. It works on Python 2 if you replace the calls to **urllib.request** with calls to the **requests** libary, although I haven't tested it extensively in Python 2

+ Includes the libraries [**xmltodict**](https://github.com/martinblech/xmltodict) and [**dicttoxml**](https://github.com/quandyfactory/dicttoxml) *(Please follow the GNU license associated with those libraries)*


## Usage

This package can be used to get lists of PDB IDs associated with specific search terms, experiment types, structures, and other common criteria.

Given a list of PDBs, this package can be used to fetch any data associated with those PDBs, including their dates of deposition, lsits of authors and associated publications, their sequences or structures, their top BLAST matches, and other query-specific attributes like lists of a ligands or chemical structure.

A set of demos is included in the iPython notebook **demos.ipynb**. A static version of this notebook (for viewing) is available as **demos.html**

## Development

This package has not been refined for every use case (there are many elborate request types allowed through the PDB's xml-based API), but I believe that enough of the basic structure is present that any additional features may be easily implemented. I encourage forks and pull requests.

More information about the PDB's API and request format can be found at this page:

[The RCSB PDB RESTful Web Service interface](http://www.rcsb.org/pdb/software/rest.do)


