# TBM930 de-ice panel PCB

This PCB implements a TBM930 de-ice panel for use with Microsoft Flight Simulator
2020 and [MobiFlight](http://www.mobiflight.com/).

## KiBot automation

This repo also demonstrates using KiBot for full CI/CD of KiCad projects. Every pull request gets ERC/DRC checks.
Publishing a GitHub release triggers generation of a suite of PCB documentation, interactive BOM, and submission
files for JLCPCB (including pick-and-place files) and PCBWay. The GitHub release version is inserted into the
generated documentation and gerber files as well. A manually triggered workflow to generate documentation is also
included.

A CodeTour is provided that walks through the KiBot and GitHub automation steps. Comments are provided in the relevant
files that explain how each piece works.

The easiest way to play with KiBot in this repo is to use
[VSCode Remote Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers).
Use the `Clone Repository in Container Volume...` command to clone this repo, then run the default build command
to trigger KiBot. Output files are put in the `KiBotOutput` folder.
