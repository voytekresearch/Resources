# Standard Operating Procedures

Standards and guidelines for writing code in the Voytek lab.

## Python

New python code should be written in Python3 (current version 3.6) unless there is specific reason to use an older version.

The guidelines mentioned below are also covered in more depth in the [shablona](https://github.com/uwescience/shablona) template, which also provides a standardized template to organizing code. 

### Style Guides

Code should be written to abide by [PEP8](https://www.python.org/dev/peps/pep-0008/). Use of a lintr is recommended to ensure PEP8 compliance. 

### Documentation

Code must be documented! Use [numpy docs](https://github.com/numpy/numpy/blob/master/doc/HOWTO_DOCUMENT.rst.txt). 

### Testing

As a first pass, code should include ['smoke tests'](http://softwaretestingfundamentals.com/smoke-testing/) - that is, simple test that ensure the code at least run, but does not necessarily extensively test all features nor the validity of all outputs.

More mature code should include ['unit tests'](http://softwaretestingfundamentals.com/unit-testing/), in which each separable unit of code is tested, both for execution, and for the validity of the outputs. This will likely include using synthetic data, on which the appropriate results can be known. 

Tests in Python should use [pytest](https://docs.pytest.org/en/latest/). 

### API Standards

Before releasing a module or update, run through the API checklist, and check for compliance: http://python.apichecklist.com

### Releasing Code

To avoid package bloat, new features should preferentially be integrated with existing modules, rather than as separate entities. For example, code operating on time-series neural data should be merged with [neurodsp](https://github.com/voytekresearch/neurodsp), unless there is a clear reason to instead have a stand-alone tool.

New features to existing packages, or new packages, should include tutorials, in the form of Jupyter notebooks, demonstrating the use of the tool.

If code is to be more formally released, it should be indexed on [PYPI](https://pypi.python.org/pypi) -  a guide on how to do so is available [here](http://peterdowns.com/posts/first-time-with-pypi.html).

### Github Standards

Keep the README up to date, it should always specify:
- continuous integration coverage and module status
- install instructions
- dependencies (including python version)
- examples of code use and outputs

## Data Standards

If and when relevant / possible, choose to use standardized data formats. For EEG/MEG/ECoG, this means the [BIDS](http://bids.neuroimaging.io), and relevant extensions, and for other electrophys / local field potential data, consider [neurodata without borders](http://www.nwb.org). Wherever possible / relevant, tools developed should have I/O orientied to these formats in particular.
