# The ACTS (A Common Tracking Sofware) Project

The ACTS project was launched in 2016 as a feasibility study aiming to encapsulate the common and re-usable components of the ATLAS Common Tracking Software for broader use in the community. From the very beginning it was targetting at high quality, generic, modernly designed components that can be used to assemble track and vertex reconstruction applications for high energy, nuclear and heay ion physics experiments.

The ACTS core project implements event data model, geometry, and tracking and vertexing tools in C++, following the C++20 standard, and aims at minimal dependecies for the core software stack. However, customizable extensions and interface layers to community libraries are available and can be augmented to the core package.

## Project organization

ACTS is organizes in a core project `acts-project/acts` which holds the software components and a simple example/demonstration framework that showcases typical track reconstruction applications using the OpenDataDetector.

Furthermore, it hosts an umbrella project, called `traccc` that aims to re-implement the standard `Acts` chain for massively parralel hardware. `traccc` relies on the sub libraries:
 - vecmem: a library for the memory management of containers
 - covfie: a covariant vector field library, e.g. for the description of the magnetic field
 - detray: a GPU friendly geometry library for describing the reconstruction geometry
 - algebra-plugins: an abstraction layer for linear algebra and float precision
