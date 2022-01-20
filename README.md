# TBM930 de-ice panel PCB

This PCB implements a TBM930 de-ice panel for use with Microsoft Flight Simulator
2020 and [MobiFlight](http://www.mobiflight.com/).

![image](https://user-images.githubusercontent.com/9524118/136433703-f8cf90e0-04c0-4a58-af3a-8a8c053edf4a.png)

## KiBot automation

This repo also demonstrates using KiBot for full CI/CD of KiCad projects. Every pull request gets ERC/DRC checks.
Publishing a GitHub release triggers generation of a suite of PCB documentation, interactive BOM, and submission
files for JLCPCB (including pick-and-place files) and PCBWay. The GitHub release version is inserted into the
generated documentation and gerber files as well. A manually triggered workflow to generate documentation is also
included.

Want to use KiBot GitHub automation with your own project? Check out my [GitHub repository template](https://github.com/neilenns/KiBot-CICD-Template/) for KiCad CI/CD to get started!
