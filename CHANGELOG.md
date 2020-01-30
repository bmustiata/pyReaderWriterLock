# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## Added

- Code coverage badge to README.md using [codecov](https://codecov.io)
- Download count related badges to README.md
 - [🎉Wow readerwriterlock is popular🥳](https://blog.pepy.tech/python/packages/stats/2019/12/14/most-popular-python-packages-in-november-2019.html)
- Added time source in the __init__ of every RWLockable

### Changed

- use by default 'time.perf_counter' instead of 'time.time'
- Updated support files
- Source tar file is now reproducible

### Removed

- Removed README.rst since pypi now supports markdown

## [Released] - 1.0.6 2020-01-14

## Fixed
- Add missing runtime dependency 'typing_extensions' to setup.py

## [Released] - 1.0.5 2020-01-14

## Fixed
- README.rst is now included in source tar

### Changed
- Fix mypy lint error '"bool" is invalid as return type for "__exit__" that always returns False'
- Use mypy Prototype to define "Lockable"

## [Released] - 1.0.4 2019-06-29


### Removed
- Python 3.4 from the list of supported python version

### Added
- Implement PEP561

## [Released] - 1.0.3 2019-02-13

### Added
- Allow alternate lock implementations to be used
- Python 3.7 to the list of supported python version

## [Released] - 1.0.2 2018-09-28

### Added
- More folders/files to be deleted by the "clean" target of the makefile to prevent previous build to pollute next build whl file
  - (fix: https://github.com/elarivie/pyReaderWriterLock/issues/1)

### Changed
- Fix lint warning R0205 (useless-object-inheritance)

## [Released] - 1.0.1 2018-03-31

### Changed
- Improve badges on README.md
- Create README.rst to present the pypi package (since pypi does not support Markdown)

## [Released] - 1.0.0 2018-03-30
**Note:** Version number was left at 1.0.0 since it is the first release on Pypi.

### Changed
- The license GPLV3 -> MIT
- Adjusted the project structure for PyPI release
- make pep8 happy
  - Rename module:
    - RWLock ➡ rwlock
  - Rename methods:
    - genRlock ➡ gen_rlock
    - genWlock ➡ gen_wlock
- make pep257 happy
- Add lint steps
- Setup CI with TravisCI
- Publish as a python package on pypi: [readerwriterlock](https://pypi.python.org/pypi/readerwriterlock)

## [Released] - 1.0.0 2015-07-08

### Added
- RWLockRead
- RWLockWrite
- RWLockFair
