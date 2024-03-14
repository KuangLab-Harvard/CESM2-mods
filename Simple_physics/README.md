SourceMods changes for customizing simple physics models in CESM2.1.x

See https://www.cesm.ucar.edu/models/simple/held-suarez

Changes beyond those already included by CESM2:
    - Fix bug in adding topography file for CESM2.1 (it works out of the box for CESM2.2). Fixed for FV and Eulerian dry cores (included in separate folders)
    - Function and namelist additions for including a land sea mask (usually from the same file as a topography file) to allow for increased friction over land. Implemented for Eulerian dry core only. 
    - Includes function and namelist additions from https://www.cesm.ucar.edu/models/simple/tref-read, again only for Eulerian drycore. See this page for how to define topography file -- the land sea mask uses the same structure. 

SourceMods changes should be copied into SourceMods/src.cam for every new run. Namelist changes should be copied into CESM/components/cam/bld/namelist_files/ 
