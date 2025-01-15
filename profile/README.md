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

## Supported by

<table border=0>
 <tr>
 <td width=200><img src="https://github.com/user-attachments/assets/07a45daa-fbe7-4f3e-ab22-04f0e573279a" height="100"></td>
 <td><a href="https://ep-dep.web.cern.ch/node/7537">CERN EP R&D</a></td>
  <td>The CERN EP department has launched a strategic R&D programme on technologies for future experiments. This initiative covers detector hardware, electronics, software and detector magnets for new experiments and detector upgrades beyond LHC phase II.</td>
</tr>
<tr>
 <td width=200><img src="https://github.com/user-attachments/assets/e489d4d3-3772-411c-a34b-86cf121bd542" height="100"></td>
 <td><a href="https://iris-hep.org">IRIS-HEP</a></td>
 <td>IRIS-HEP is a software institute funded by the National Science Foundation. It is developing state-of-the-art software cyberinfrastructure required for the challenges of data intensive scientific research at the High Luminosity Large Hadron Collider (HL-LHC) at CERN, and other planned HEP experiments of the 2020’s.</td>
</tr>
<tr>
 <td width=200><img src="https://github.com/user-attachments/assets/a8ac4283-7cee-4622-b281-fa01dfd1619a" height="100"></td>
 <td><a href="https://aidainnova.web.cern.ch">AIDAInnova</a></td>
 <td>Discoveries in particle physics are technology-driven; AIDAinnova will provide state-of-the-art upgrades to research infrastructures, such as test beams, in order to unfold the scientific potential of detector technologies. The project will run for a duration of four years from April 2021 to March 2025 and is co-funded by the European Commission under its Horizon 2020 programme.</td>
</tr>
</table>
