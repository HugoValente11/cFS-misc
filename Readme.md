# Prerequisites
This tool is part of the cFS modified TASTE toolchain (cFS Creator). Before we can work with cFS Creator we need tools to be available on the computer and some libraries to compile against.

1. Install the TASTE VM following the instructions in https://gitrepos.estec.esa.int/taste/taste-setup. <strong>All the following instructions assume you are using the TASTE VM.</strong>
2. Replace the misc folder with our modified one following the instructions in [cFS misc](https://github.com/HugoValente11/cFS-misc).
3. Replace kazoo with our modified Kazoo following the instructions in [cFS Kazoo](https://github.com/HugoValente11/cFS-Kazoo).
4. Setup our modified QtCreator environment, cFS Creator, following the instructions in [cFS Creator](https://gitlab.com/aurora-software/cFS-Creator).
5. Add the cFS runtime following the instructions in [TASTE cFS Runtime](https://github.com/HugoValente11/TASTE-cFS-Runtime).
6. Replace the local configuration files for Qt with our modified ones following the instructions in [cFS Local Config](https://gitlab.com/aurora-software/cFS-local-config).

# How to use the toolchain
It works exactly the same way as the original TASTE version. You can use the `taste` command to create a new project and it should load the modified QtCreator environment, cFS Creator.

# Build misc
To update the misc to our modified version that allows to generate code for cFS applications execute the following commands

`$ mv ~/tool-src/misc ~/tool-src/misc-bu`

`$ git clone https://github.com/HugoValente11/cFS-misc ~/tool-src/misc`

`$ ~/tool-src/install/90_misc.sh`

# Description
This repository contains necessary files involved in different parts of the toolchain.
The helper-scripts folder is used to generate the initial project files for cFS applications.
The aadl-library contains the cFS AADL property set with the properties supported in our code generation toolset.
The space-creator folder contains the mapping rules to ensure that the XML properties are correctly mapped to AADL properties specified in the cFS AADL property set