# quantms-utils
[![Python application](https://github.com/bigbio/quantms-utils/actions/workflows/python-app.yml/badge.svg)](https://github.com/bigbio/quantms-utils/actions/workflows/python-app.yml)
[![Python package](https://github.com/bigbio/quantms-utils/actions/workflows/python-package.yml/badge.svg)](https://github.com/bigbio/quantms-utils/actions/workflows/python-package.yml)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/ea6903630b3a4d15b674a16b8ce594a7)](https://app.codacy.com/gh/bigbio/quantms-utils/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
[![PyPI version](https://badge.fury.io/py/quantms-utils.svg)](https://badge.fury.io/py/quantms-utils)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Python package with scripts and functions for the [quantms workflow](https://github.com/bigbio/quantms) for the analysis of quantitative proteomics data.

The package is available on PyPI: [quantms-utils](https://pypi.org/project/quantms-utils/)
```
pip install quantms-utils
```

## Available Scripts 

The following functionalities are available in the package:

### Diann scripts

- `dianncfg` - Create a configuration file for Diann including enzymes, modifications, and other parameters.
- `diann2mztab` - Convert Diann output to mzTab format. In addition, convert DIA-NN output to MSstats, Triqler or mzTab.
    The output formats are used for quality control and downstream analysis in quantms.

### SDRF scripts

- `openms2sample` - Extra sample information from OpenMS experimental design file. An example of OpenMS experimental design file is available [here](https://github.com/bigbio/quantms-utils/blob/dev/tests/test_data/BSA_design_urls.tsv).
- `checksamplesheet` - Check the sample sheet for errors and inconsistencies. The experimental design coult be an OpenMS experimental design file or and SDRF file. 

### Other scripts

- `psmconvert` - The convert_psm function converts peptide spectrum matches (PSMs) from an idXML file to a CSV file, optionally filtering out decoy matches. It extracts and processes data from both the idXML and an associated spectra file, handling multiple search engines and scoring systems.
- `mzmlstats` - The `mzmlstats` processes mass spectrometry data files in either `.mzML` or `Bruker .d` formats to extract and compile statistics about the spectra. It supports generating detailed or ID-only CSV files based on the spectra data.

## Contributions and issues

Contributions and issues are welcome. Please, open an issue in the [GitHub repository](https://github.com/bigbio/quantms) or PR in the [GitHub repository](https://github.com/bigbio/quantms-utils).
