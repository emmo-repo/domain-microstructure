[![DOI](https://zenodo.org/badge/348298817.svg)](https://zenodo.org/badge/latestdoi/348298817)


Microstructure Domain Ontology (MDO)
====================================
This is work in progress.

The Microstructure Domain Ontology is intended to be a domain ontology
for physical metallurgy.  The intension is to cover all relevant
aspect of metallic microstructures, including:
  - composition
  - particles, both stable (primary) and metastable (precipitates)
  - grains
  - subgrains
  - grain boundaries & particle free zones (PFZs)
  - texture
  - dislocations
  - alloy systems

The aim is to support both microstructure modelling as well as
characterisation.

For modelling, we will distinguish between
  - evolution models (that changes the microstructure through a
    succession of states) and
  - property models (that relates a microstructure state to a property).

It should support describing same concept at different spatial
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
Version dependencies on imported ontologies:

| Version | [EMMO] | [CHAMEO] |
|---------|--------|----------|
| 0.3.1   | 1.0.0  | 1.0.0    |



Obtaining the Microstructure Domain Ontology
--------------------------------------------
The Microstructure Domain Ontology can be access or opened in Protege
using the following url

    https://w3id.org/emmo/domain/microstructure/source

It can also be cloned from its [GitHub repository] using the `git`
command:

    git clone https://github.com/emmo-repo/domain-microstructure.git



Attributions and credits
------------------------
### Authors
- Jesper Friis, SINTEF, Norway
- Tomas Manik, NTNU, Norway
- Sylvain Gouttenbroze, SINTEF, Norway
- Astrid Marthinsen, SINTEF, Norway
- Georg Schmitz, ACCESS, Germany
- Ulrike Cihak-Bayr, AC2T, Austria


### Supporting projects
- Demystify ontologies - Internal project at [SINTEF](http://www.sintef.no)
- [SFI PhysMet](https://www.ntnu.edu/physmet/) (2020-2028) that receives funding from the Research Council of Norway, project no. 309584.


License
-------
The physmet domain ontology is released under the [Creative Commons
Attribution 4.0
International](https://creativecommons.org/licenses/by/4.0/legalcode)
license (CC BY 4.0).


[EMMO]: https://github.com/emmo-repo/EMMO
[CHAMEO]: https://github.com/emmo-repo/domain-characterisation-methodology
[Crystallography]: https://github.com/emmo-repo/domain-crystallography
[GitHub repository]: https://github.com/emmo-repo/domain-microstructure
