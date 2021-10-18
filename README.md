# Ion Traps and Accessories

## Background

Ion traps are one of the leading platforms in several quantum technologies pillars: from atomic clocks to quantum communication, via quantum simulations to quantum computing. These efforts have, to a very large degree, been performed in the academic domain, with more and more commercial entities showing interest in the ion-trap platform. However, most of the information and documentation regarding ion traps and the used accessories such as mounts, resonators, filters, etc. is distributed over research articles and theses.

## Challenge

* Bring the ion trap platform to the next technical readiness level,
* addressing the possibility of a bottom-up approach for standardization,
* and leveraging the existing know-how such that motivated new entities can join this interesting field of research and engineering

is highly challenging when the available data in solutions that have worked and, potentially more important, that have **not** worked.

## Goal

An informal group of ion trap researchers and developers have joined forces to collect information to facilitate the coordination, documentation and general improvement of the ion-trap platform. As such, the documentation spans from ion traps (surface traps, 3D traps, ...), trap mounts (with all the necessary information such as suitable temperature ranges they may be exposed to), filter boards and resonators, DACs and RF drives (both room temperature and cryo, for in-vacuum and air-based operation), to optical integration.

Seeing that research and engineering regarding ion trap technologies is rapidly evolving, the content, offered detail, and structure is up for discussion.

## Confidentiality and Publication

For the moment this repository is private. However, the goal of this work is to serve as go-to documentation regarding ion traps and all accessories that enable high-performance control of charged particles. As such, none of contributions to this repository shall be confidential.

Publication has not been clarified yet. However, Gitlab Pages and similar services would allow us to create visually appealing pages without the necessity to disclose the entire repository.

## Approach

The documentation is split into:
* [Ion traps](ion_traps/README_ion_traps.md)
* [Electronics](electronics/README_electronics.md)

Each of these folders come with their own guidelines and templates to address the respective documentation requirements.

## Contributors

The content presented here has been gathered and reviewed and is maintained by representatives from (in alphabetic order):
* [University of Innsbruck, team of Prof. Rainer Blatt](https://quantumoptics.at/en/)
Regarding details on the contribution and review process, please have a look [here](CONTRIBUTING.md).

## File formats

The design files should be provided in file formats that are readable without the need for commercial licenses. As a minimum requirement, proprietary design files should be complemented by human readable version in the portable document format (`PDF`). Images should be proved in `PNG` or `JPG` format.

We suggest to use these file formats for the following component types.

| Component type | Preferred format | Alternative formats |
| ------ | ------ | ------ |
| Electronic schematic | [KiCad](https://www.kicad.org/) Schematic | [Altium](https://www.altium.com/altium-designer/) |
| Electronic Printed circuit board | [KiCad](https://www.kicad.org/) PCB                | [Gerber](https://en.wikipedia.org/wiki/Gerber_format), [Altium](https://www.altium.com/altium-designer/) |
| Mechanical component | [STEP](https://en.wikipedia.org/wiki/ISO_10303-21) | [DWG](https://en.wikipedia.org/wiki/.dwg), [Solidworks](https://www.solidworks.com/), [Inventor](https://www.autodesk.com/products/inventor/) |
| Mask layout | [GDSII](https://en.wikipedia.org/wiki/GDSII) | [DXF](https://en.wikipedia.org/wiki/AutoCAD_DXF) |
