# GSOC Work Report

Worked on following 3 projects – 
## HDF Data Storage Capabilities
•	Implemented a `HDFWriterMixin` class , which have these functions - 
	  

 1. Method to aggregate selected properties of class
 2. Write these selected properties to a HDF file
 3. A `to_hdf` method that combines both of these methods.

•	It determines, how these properties will be uniformly stored, such as scalars , 1D or 2D objects.        
•	Implemented unit tests for the same using Mock setups.
•	It can easily be extended and inherited, eliminating the need of implementing HDF functionalities in separate classes.
•	Wrote Documentation for the same.

### Related PRs
[PR#744](https://github.com/tardis-sn/tardis/pull/744) -  HDFWriter class + Unit Tests  
[PR#747](https://github.com/tardis-sn/tardis/pull/747) - Update Model and Density classes to use HDFWriter + Unit Tests   
[PR#748](https://github.com/tardis-sn/tardis/pull/748) - Update Runner and Spectrum classes to use HDFWriter + Unit Tests  
[PR#749](https://github.com/tardis-sn/tardis/pull/749) - Change name of HDFWriter to HDFWriterMixin  
[PR#752](https://github.com/tardis-sn/tardis/pull/752) - PlasmaWriterMixin + Unit Tests  
[PR#753](https://github.com/tardis-sn/tardis/pull/753) - HDFWriter Documentation  
[PR#768](https://github.com/tardis-sn/tardis/pull/768) - Simulation HDF and deprecated to_hdf cleanup  
[PR#769](https://github.com/tardis-sn/tardis/pull/769) - [DOC] Updated to_hdf notebook  


## Isotope handling within TARDIS
•	Extended current Tardis Configuration System to support parsing of Isotopic Elements.
•	Using Pyne library , decayed isotopic elements , and then merge it into normal elemental elements abundance dataframe. 
•	Wrote a console script to convert CMFGEN files into TARDIS format. 
•	Unit tests and Documentation for the same.

### Related PRs
[PR#756](https://github.com/tardis-sn/tardis/pull/756) - Isotope Abundances class  
[PR#757](https://github.com/tardis-sn/tardis/pull/757) - Decay and merge isotopic abundance dataframe  
[PR#762](https://github.com/tardis-sn/tardis/pull/762) - Isotope uniform config option  
[PR#764](https://github.com/tardis-sn/tardis/pull/764) - Isotope stratified file support  
[PR#767](https://github.com/tardis-sn/tardis/pull/767) - Docs for Isotope config  
[PR#771](https://github.com/tardis-sn/tardis/pull/771) -  Add cmfgen2tardis script   
[PR#772](https://github.com/tardis-sn/tardis/pull/772) - CMFGEN density parser  


## Testing Framework for multiple reference data 
•	Working on adding ability to test and generate reference data for Plasma module of TARDIS.
•	It will allow to test Plasma module and easily expand it to add new references. 

### Related PRs

[PR#775](https://github.com/tardis-sn/tardis/pull/775) - Transition from atomic-dataset config option to tardis-refdata  
[PR#779](https://github.com/tardis-sn/tardis/pull/779) - Save coverage report when tests use tardis-refdata  
[PR#774](https://github.com/tardis-sn/tardis/pull/774) - Replace Comparison values in Plasma Unit Tests with reference HDF file  
