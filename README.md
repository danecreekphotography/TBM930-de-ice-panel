# TBM930 de-ice panel PCB

This PCB implements a TBM930 de-ice panel for use with Microsoft Flight Simulator
2020 and [MobiFlight](http://www.mobiflight.com/).

## KiBot automation

This repo also demonstrates using KiBot for full CI/CD of KiCad projects. Every pull request gets ERC/DRC checks.
Publishing a GitHub release triggers generation of a suite of PCB documentation, interactive BOM, and submission
files for JLCPCB (including pick-and-place files) and PCBWay. The GitHub release version is inserted into the
generated documentation and gerber files as well. A manually triggered workflow to generate documentation is also
included.

If you just want to read through how this works [use GitHub.dev to go through the codetour](https://github.dev/neilenns/TBM930_De-ice_panel)
that walks through the KiBot and GitHub automation steps. Comments are provided in the relevant files that explain how each piece works.

If you want to try customizing the KiBot outputs the easiest way is to use
[VSCode Remote Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers).
Use the `Clone Repository in Container Volume...` command to clone this repo, then run the default build command
to trigger KiBot. Output files are put in the `KiBotOutput` folder.

Never used VSCode remote containers before on Windows? Here's how to get set up:

1. From a PowerShell install WSL2 with this command: `wsl --install`
2. Install [Visual Studio Code](https://code.visualstudio.com/Download) and Docker Desktop(https://www.docker.com/products/docker-desktop)
3. Install the [Remote Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension for VSCode

When installing Docker Desktop you may be told you have to enable virtualization in your computer's BIOS. Setting that up
is outside the scope of this readme but isn't hard. Just do a web search for your motherboard for how to enter the BIOS
and what the exact name of the setting is, then turn it on.
