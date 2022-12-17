# The Infofile format

Recording metadata during data acquisition is both, an essential aspect of and as old as science itself. The Infofile format is a simple textual file format developed to document research data. It allows researchers in the lab to record all relevant metadata during data acquisition in a user-friendly and obvious way while minimising any external dependencies. The resulting machine-actionable metadata in turn allow processing and analysis software to access relevant information, besides making the research data more reproducible and FAIRer.

## Features

* Simple text format
* Storing structured, machine-actionable metadata
* Minimum formatting
* Focussing on human-writability
* No external (software) dependencies


## Requirements

Nothing more than a (plain) text editor.


## Format specification

The specification of the Infofile format can be found in the supporting information to the publication provided in the "How to cite" section below.


## Organisation

Examples of templates for different (spectroscopic) methods are provided in the `examples` directory, with older versions of these templates residing in the `examples/archive` subdirectory. 

The current reference implementation of the Infofile parser is part of the [ASpecD framework](https://github.com/tillbiskup/aspecd). Development of the templates for specific methods will always be closely connected to the respective data model, e.g. in context of the [trepr](https://github.com/tillbiskup/trepr) and [cwepr](https://github.com/tillbiskup/cwepr) Python packages.



## Contributing

Due to its permissive BSD license, you are free to use and further develop the Infofile format for your own purposes. However, any feedback will be greatly appreciated. To coordinate development, cloning the repository and providing pull requests is strongly encouraged. For details, see the file `CONTRIBUTING`.


## How to cite

The Infofile format is licensed under a BSD license. However, if you use it for your own research, you may cite the following paper:

  * Bernd Paulus, Till Biskup (2022) Towards more reproducible and FAIRer research data: documenting provenance during data acquisition using the Infofile format. *ChemRxiv*. [doi:10.26434/chemrxiv-2022-jsjnd](https://doi.org/10.26434/chemrxiv-2022-jsjnd)


## License

The Infofile format is distributed under the BSD license. For details, see the file `LICENSE`.


## Authors

* Bernd Paulus (2011-14)

    Motivated and co-developed the format and was key to its practial adoption, as he made its use obligatory for all students he supervised.

* Till Biskup (2011-2022)

    Developed the format, formalised its specification, implemented the importers, maintains the format.


## Related projects

The Infofile format has originally been developed for use with MATLAB(r) based toolboxes for data processing and analysis. Nowadays, these MATLAB(r) toolboxes have largely been superseded by Python software, namely the ASpecD framework and derived packages. The current reference implementation of the Infofile parser is part of the ASpecD framework, support for special formats (and mappings) is contained in derived packages, namely the trepr and cwepr Python packages.

* [ASpecD framework](https://docs.aspecd.de/)

    A Python framework for the analysis of spectroscopic data focussing on reproducibility and good scientific practice, developed by T. Biskup.

* [cwepr package](https://docs.cwepr.de/)

    Python package for processing and analysing continuous-wave electron paramagnetic resonance (cw-EPR) data, originally implemented by P. Kirchner, developed and maintained by M. Schröder and T. Biskup.

* [trepr package](https://docs.trepr.de/)

    Python package for processing and analysing time-resolved electron paramagnetic resonance (trEPR) data, developed by J. Popp, currently developed and maintained by M. Schröder and T. Biskup.

