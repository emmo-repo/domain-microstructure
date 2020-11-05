[![pipeline status](https://gitlab.com/sfi-physmet/platform/physmetontology/badges/master/pipeline.svg)](https://gitlab.com/sfi-physmet/platform/physmetontology/pipelines/latest)


First draft of an EMMO-based ontology for physical metallurgy
=============================================================
This is intended to be a domain ontology for physical metallurgy.  The
intension is to cover all relevant aspect of metallic microstructures,
including
  - composition
  - particles, both stable (primary) and metastable (precipitates)
  - grains
  - subgrains
  - grain boundaries & particle free zones (PFZs)
  - texture
  - dislocations

The aim is to support both microstructure modelling as well as
characterisation.

For modelling, we will distinguish between
  - evolution models (that changes the microstructure through a
    succession of states) and
  - property models (that relates a microstructure state to a property).

It should support describing same concept at different spacial
resolutions, like mean field, 1D, 2D and 3D.

For mean field descriptions (what about spatially resolved), it should
be possible describe quantities at different statistical levels, like
mean size, normalised size distribution (mean + standard deviation)
and full size distribution.

There should be a common way to connect a state to external
conditions, like temperature, volume/shape and pressure (essential for
describing a process).


Open questions
--------------
* Should industrial processes that changes the microstructure, like
    - casting (solidification)
    - homogenisation
    - extrusion/rolling
    - forming (deformation)
    - aging/heat treatment

  be included in this, or in separate sub-ontologies?



Imported ontologies
-------------------
This ontology builds on top of EMMO and the crystallography and
mechanics domain ontologies. See the following table for version
compatibilies:

| Imported Ontologies  | Version           |
| -------------------- | ----------------- |
| [EMMO][1]            | 1.0.0-alpha2      |
| [crystallography][2] | 0.0.1             |


Obtaining PhysMetOntology
-------------------------
This repository include the correct version of the crystallography and
mechanics domain ontologies as a git submodules.  Hence, use the
following command when cloning this repository:

    git clone --recurse-submodules --shallow-submodules git@gitlab.com:sfi-physmet/platform/physmetontology.git


Attributions and credits
------------------------
### Authors
- Jesper Friis, SINTEF
- Tomas Manik, NTNU
- Sylvain Gouttenbroze, SINTEF
- Astrid Marthinsen, SINTEF

### Projects
- Demystify ontologies - Internal project at [SINTEF](www.sintef.no)
- SFI PhysMet


License
-------
The physmet domain ontology is released under the [Creative Commons
Attribution 4.0
International](https://creativecommons.org/licenses/by/4.0/legalcode)
license (CC BY 4.0).


[1]: https://github.com/emmo-repo/EMMO
[2]: https://github.com/emmo-repo/domain-crystallography
