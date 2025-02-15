# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Fixed 
- Calculation of p values of point clouds for Dispersion now works
- Updated PyVista calls to be consistent with changes in their API

## [0.7.1] - 2022-06-27

### Fixed
- Fixed type errors related to ConformerEnsemble and Python 3.8 

## [0.7.0] - 2022-06-22

### Added
- Added `SolidAngle` for solid angle calculations.

## [0.6.0] - 2022-03-28

### Added
- Add capacity to Boltzmann average 1D arrays in `ConformerEnsemble`
- `ConeAngle` now uses libconeangle as default with the internal algorithm as backup.
- Added `BiteAngle` for bite angle calculations.

### Fixed
- `XTB.get_fukui`, affecting the varieties "electrophilicity" (wrong sign), "nucleophilicity" (wrong sign), "radical" (wrong number) and "local_electrophilicty" (wrong number)
- Error when `ConformerEnsemble` was initiated with `connectivity_matrix=None`
- Interface to be compatible with version 3 of dftd4.

### Removed
- D3Grimme calculator due to removal from dftd4. The internal D3Calculator remains.

## [0.5.5] - 2021-10-07

### Fixed
- Fixed bug with `ConformerEnsemble.from_crest` with only one structure in the ensemble
- Fixed bug with `ConformerEnsemble.from_ob_ga` when generating RDKit mol 

## [0.5.4] - 2021-07-13

### Fixed
- Fixed bug with `io.write_xyz` and multiple structures

## [0.5.3] - 2021-04-29

### Fixed 
- Typing of external dependencies to allow conda-forge install

## [0.5.2] - 2021-04-28

### Added
- First public release. Changelog use starts here.

### Deprecated
- `BuriedVolume.percent_buried_volume`. Use `BuriedVolume.fraction_buried_volume` instead.`percent_buried_volume` will be reintroduced later with the proper meaning.

