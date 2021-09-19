# TBM930 de-ice panel PCB

This PCB implements a TBM930 de-ice panel for use with Microsoft Flight Simulator
2020 and [MobiFlight](http://www.mobiflight.com/).

This repo also demonstrates using KiBot for full CI/CD of KiCad projects. Every pull request gets ERC/DRC checks. Publishing a GitHub release
triggers generation of a suite of PCB documentation, interactive BOM, and submission files for JLCPCB (including pick-and-place files) and PCBWay.
The GitHub release version is inserted into the generated documentation and gerber files as well.

See the `.github/workflows` and `.kibot` folders for the scripts that do the CI/CD work.
