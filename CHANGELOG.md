# Changelog

## [2.2.0](https://github.com/strongsdcom/github-actions/compare/v2.1.0...v2.2.0) (2026-02-19)


### Features

* add run-on input to linode-lke-deploy workflow ([#65](https://github.com/strongsdcom/github-actions/issues/65)) ([ab3da57](https://github.com/strongsdcom/github-actions/commit/ab3da57ddca91e52d22582d4cab12425c67b789c))


### Bug Fixes

* refactor token retrieval in release-please workflow ([#62](https://github.com/strongsdcom/github-actions/issues/62)) ([15ec8d8](https://github.com/strongsdcom/github-actions/commit/15ec8d876953f723621afa4c21c6783e16c70202))
* remove existing gh-token remote before adding new one ([67c1289](https://github.com/strongsdcom/github-actions/commit/67c1289de39e8ac7e1a32b371d411c681a1fcd2f))

## [2.1.0](https://github.com/strongsdcom/github-actions/compare/v2.0.4...v2.1.0) (2026-01-14)


### Features

* add run-on parameter to release-please ([#59](https://github.com/strongsdcom/github-actions/issues/59)) ([7bd168e](https://github.com/strongsdcom/github-actions/commit/7bd168e79f187b82d77776fa04ec362193d3250b))

## [2.0.4](https://github.com/strongsdcom/github-actions/compare/v2.0.3...v2.0.4) (2026-01-12)


### Reverts

* **ci:** change release-please runner back to ubuntu-latest ([#57](https://github.com/strongsdcom/github-actions/issues/57)) ([e9fcc99](https://github.com/strongsdcom/github-actions/commit/e9fcc99b4e4fc8fb7797e96d0c66059c6e5b4edc))

## [2.0.3](https://github.com/strongsdcom/github-actions/compare/v2.0.2...v2.0.3) (2025-09-05)


### Bug Fixes

* change cache action path ([#42](https://github.com/strongsdcom/github-actions/issues/42)) ([8792bd1](https://github.com/strongsdcom/github-actions/commit/8792bd154f1c6d2d2134c4ff88155b1543d4e1da))
* remove not needed separate caching action ([#44](https://github.com/strongsdcom/github-actions/issues/44)) ([b5c9be6](https://github.com/strongsdcom/github-actions/commit/b5c9be65b7c42371458c1f1784002d8d5826dc3b))
* resolve issue with docker layer caching ([#40](https://github.com/strongsdcom/github-actions/issues/40)) ([4a1f354](https://github.com/strongsdcom/github-actions/commit/4a1f354255cee5fa0bc89feaf1e6db13d90bcb2d))

## [2.0.2](https://github.com/strongsdcom/github-actions/compare/v2.0.1...v2.0.2) (2025-04-14)


### Bug Fixes

* rename version to release ([#38](https://github.com/strongsdcom/github-actions/issues/38)) ([2d5657e](https://github.com/strongsdcom/github-actions/commit/2d5657ebc8c441407a4381b38d2c9d8b76b2a2ba))

## [2.0.1](https://github.com/strongsdcom/github-actions/compare/v2.0.0...v2.0.1) (2024-09-16)


### Bug Fixes

* remove default release-type ([293782f](https://github.com/strongsdcom/github-actions/commit/293782fff7f33d0500f90963bc820b8bbea67a0b))

## [2.0.0](https://github.com/strongsdcom/github-actions/compare/v1.0.0...v2.0.0) (2024-09-16)


### ⚠ BREAKING CHANGES

* **release-please:** upgrade to v4

### Features

* **release-please:** upgrade to v4 ([65ff2d0](https://github.com/strongsdcom/github-actions/commit/65ff2d0ea052c55b11f419b149da673710289ab9))

## 1.0.0 (2024-09-16)


### Features

* add ARM support ([#13](https://github.com/strongsdcom/github-actions/issues/13)) ([1d19dac](https://github.com/strongsdcom/github-actions/commit/1d19dac2d0ac341f8790be26514b402663074838))
* add secrets support pass as helm set value argument for deployment step ([ec8e4c9](https://github.com/strongsdcom/github-actions/commit/ec8e4c984135edede1d78ce501d06d82da2bae48))
* add support for custom platform to the docker build workflow ([#16](https://github.com/strongsdcom/github-actions/issues/16)) ([4a75c61](https://github.com/strongsdcom/github-actions/commit/4a75c61790b5497cd440f75152a6d4e283b2515e))
* build-args for inputs ([#7](https://github.com/strongsdcom/github-actions/issues/7)) ([1c19f90](https://github.com/strongsdcom/github-actions/commit/1c19f905c6179a84ab9139f8d4c4ab80cec3eac7))
* Github actions for Linode Cloud ([#10](https://github.com/strongsdcom/github-actions/issues/10)) ([9d387ea](https://github.com/strongsdcom/github-actions/commit/9d387ea57982622a18e29491b674640580702687))
* release-please-action upgrade to v4 ([#15](https://github.com/strongsdcom/github-actions/issues/15)) ([9053dc5](https://github.com/strongsdcom/github-actions/commit/9053dc5fe07116568fc71723f96190611a297392))
* Self hosted runner ([#14](https://github.com/strongsdcom/github-actions/issues/14)) ([04d6c1b](https://github.com/strongsdcom/github-actions/commit/04d6c1b8effdb9b20c47d54d2d717af9b08637e8))


### Bug Fixes

* helm multiline secrets ([#11](https://github.com/strongsdcom/github-actions/issues/11)) ([b00228c](https://github.com/strongsdcom/github-actions/commit/b00228cb5b4acc5c8c114063d6ebe21b5939323e))
* incorrect run-on input format ([150e594](https://github.com/strongsdcom/github-actions/commit/150e594665a26c5233a9cc2516cb56b0ff1663fb))
* remove default aws region to reduce potential issues ([6954c77](https://github.com/strongsdcom/github-actions/commit/6954c7717fa3f5c2cb3c901d546e67cc0821274f))
