# icarus
Files pertaining to the development of my personal custom keyboard Icarus.

# Ergogen
The keyboard and pcb layout were generated using Ergogen locally. The config files and corresponding outputs can be found in the `ergogen` folder. There are custom footprints that generate 3d models on the footprints of all components, and these are found in `final_pcbs/components`. **The path for these are custom to my file setup, and thus will most likely not work on your machine. Please change the corresponding file paths if you wish to locally build this model.**

# KiCad
The corresponding PCB outputs from Ergogen were traced in KiCad. The final traced PCBs, along with exported STEP files are found in the `final_pcbs` folder. Currently, **the final PCBs do not have the switch and keycap models on the footprints of the switches, and there are traces which have been shown to be on fragile board sections.** Both of these changes will be updated in the near future and this notice will be removed once that happens.

# Case files
The case files were constructed in Onshape. One can view these files [here](https://cad.onshape.com/documents/795d5125a76cdfb5a48cf88b/w/a7573c951f90309017d525a7/e/47b874ca74b5b2133d47f936). There are also STEP files in this repo, in the `case_files` folder. Note that the case files provided are for the left side of the keyboard only, and the right side is simply a mirror image of the left side.

## Travel case files

As of 01 July '26, there are travel case files in the works. Please stay tuned for their release. 

# ZMK configuration.

Icarus currently runs ZMK. The configuration repository and current firmware can be found [here](https://github.com/Hi30MC/zmk-config).

# Physical build notes

This case was designed and printed for FDM, though the battery cage is a major flaw in the design. There are supports that are best printed as "normal slim" supports on Orca, for example, as these had the cleanest release. I found that it was best to print the ports/switches/etc on the case as-is, then clean up with a file, though one may find success with adding supports and removing those manually. Additionally, I reccomend placing brim ears on all corners of the faceplate/skirt print, as well as the baseplate as they tend to warp during printing. Mounting the baseplate to the PCB was done with M2.5 self-threading screws, which need washers to secure onto the board. **Print these separately, and not attached to the baseplate.** There is also a known issue with the right PCB's battery jack hitting against the Kailh hotswap bracket, which will be fixed soon™. If any other issues arise in whoever decides to build this, please reach out!
