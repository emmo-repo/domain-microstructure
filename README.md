
Microstructure Domain Ontology
==============================
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


Obtaining the Microstructure Domain Ontology
--------------------------------------------
The Microstructure Domain Ontology can be access or opened in Protege
using the following url

    https://raw.githubusercontent.com/emmo-repo/domain-microstructure/main/physmet.ttl

It can also be cloned from its [GitHub repository][3].  With [ssh
access to GitHub][github-ssh] set up, the Microstructure Domain
Ontology can be cloned with

    git clone git@github.com:emmo-repo/domain-microstructure.git



Attributions and credits
------------------------
### Authors
- Jesper Friis, SINTEF, Norway
- Tomas Manik, NTNU, Norway
- Sylvain Gouttenbroze, SINTEF, Norway
- Astrid Marthinsen, SINTEF, Norway
- Georg Schmitz, ACCESS, Germany
- Ulrike Cihak-Bayr, AC2T, Austria


### Projects
- Demystify ontologies - Internal project at [SINTEF](www.sintef.no)
- [SFI PhysMet](https://www.ntnu.edu/physmet)


License
-------
The physmet domain ontology is released under the [Creative Commons
Attribution 4.0
International](https://creativecommons.org/licenses/by/4.0/legalcode)
license (CC BY 4.0).


[1]: https://github.com/emmo-repo/EMMO
[2]: https://github.com/emmo-repo/domain-crystallography
[3]: https://github.com/emmo-repo/domain-microstructure
[github]: https://github.com/
[github-ssh]: https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
