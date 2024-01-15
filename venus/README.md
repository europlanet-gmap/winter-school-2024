# Venus

The hands-on will be based on a pre-produced QGIS project. Data layers are described in [Venus data info](venus_data_info_2024-GMAP-winter-school.md)

## Venus hands-on short guide

### Hands-on objectives

-   Illustrate the particularities of Magellan SAR data and the basics
    of its interpretation.
-   View examples of the different primary and secondary structures of
    Venus.
-   Recognize the principal types of terrains and volcanic structures of
    Venus.
-   Learn how to work with the VIRTIS data and how to interpret them in
    the 1 μm spectral region.
-   View examples of mapping of high- and low-emissivity areas on Venus.
-   Learn how to link high- and low- emissivity anomalies to main
    mineralogical surface composition based on the comparison with
    laboratory emissivity data.

### Data required

-   Magellan SAR data. USGS Global mosaics.
-   VIRTIS retrieved emissivity map at 1.02 μm.


### Steps involved 

#### Part 1. Magellan SAR.

-   General description of the Magellan data sets.
-   Access to Magellan data through the USGS Map a planet server.
-   General view of the global SAR Venus Mosaic and the geology of the
    planet.
-   Case study: Example of tessera terrain (Alpha Regio)
-   Case study: Example of regional volcanic plains (Helen Planitia).
-   Case study: Example of young volcanic highland (Imdr Regio).

#### Part 2. Venus Express VIRTIS data.

-   General description of the VIRTIS spectrometer and data sets.
-   General view of the global VIRTIS coverage, radiance and emissivity
    maps.
-   General simplified description of VIRTIS emissivity retrieval in the
    1.02 μm spectral window
-   General guide on the interpretation of VIRTIS emissivity data at
    1.02 μm
-   Comparison of VIRTIS emissivity with laboratory emissivity data
-   Case study: Example of emissivity anomalies in young volcanic
    highland in Imdr Regio
-   Case study: Example of emissivity anomalies corresponding to tessera
    terrain in Alpha Regio

### Expected results

#### Part 1. Magellan Data.

-   Participants will be able to identify the principal types of primary
    and secondary structures on Venus and the problems that we face to
    delineate contacts due to the nature of SAR data.
-   Participants will recognize the principal types of terrains and
    volcanic structures present in the surface of Venus and the
    structures that characterize them.

#### Part 2. Venus Express VIRTIS data.

-   Participants will be able to identify and map areas of high and low
    emissivity anomalies using VIRTIS data in the 1.02 μm spectral
    window.
-   Participants will be able to link the high and low-emissivity areas
    with the main geologic units and structures mapped in the first
    Venus hands-on practical activity (geologic mapping exercise with
    Ivan).
-   Participants will be able to relate thermal emission variations from
    the Venus' surface to mineralogy.

## Venus task assignment short guide

### Task objective.

-   Simplified geologic and mineralogic mapping of the selected area and
    a geologic history of the study area.

### Data required.

-   Area selected for the exercise: Transition between Themis Regio and
    Helen Planitia (Magellan SAR data and VIRTIS emissivity data in the
    1.02 μm spectral window).

### Steps involved (quick description / screenshots, etc.)

- A general view on the mapping area: Hands-on activity with the
instructors to get familiarized with the study area (30 minutes aprox).

- Identification and mapping of the principal regional and local
structural suites of the mapping area (manually using [**Mappy
tool**](https://mappy.readthedocs.io/en/master/quick_start.html)).

- Identification and mapping of primary structures (volcanic and impact
related) of the mapping area (manually using [**Mappy
tool**](https://mappy.readthedocs.io/en/master/quick_start.html)).

- Scaling of VIRTIS emissivity value to infer the relative variation
when assuming a reference emissivity.
   - We want to scale the emissivity values adopting a global average
 emissivity of Venus plains of 0.58. This satisfies the constraint that
 the regions with the highest radiance measured on Venus have
 emissivity ≤ 1 (as used in previous studies as Smrekar et al., 2010;
 Basilevsky et al., 2012; Gilmore et al., 2015). This scales the
 emissivity of the area under investigation to a range of 0.5-0.7.
  - To scale the VIRTIS emissivity data, use the **[Raster calculator
 tool](https://docs.qgis.org/2.18/en/docs/user_manual/working_with_raster/raster_calculator.html)**
 and select the VIRTIS emissivity data@1 (which corresponds to the
 emissivity values extracted at the 1.02 µm spectral band) and proceed
 as shown in the screenshot below. The result will be a new generated
 raster with the scaled values of emissivity.


Relevant references are included below.

# References

Basilevsky, A.T. et al., 2012. Geologic interpretation of the
near-infrared images of the surface taken by the Venus Monitoring
Camera, Venus Express. Icarus 217, 434--450.

Ford, J. P., Plaut. J. J., Weitz, C. M., Farr, T. G., Senske, D. A., Stofan, E. R., Michaels, G., Parker, T. J.  (1993) Guide to Magellan Image Interpretation,  Jet Propulsion Laboratory, California Institute of Technology, JPL Publication 93-24, - available online at https://ntrs.nasa.gov/api/citations/19940013181/downloads/19940013181.pdf

Hansen, V.L. (2000). Geologic mapping of tectonic planets. Earth and
Planetary Earth Sciences. [Volume 176, Issues
3--4](https://www.sciencedirect.com/journal/earth-and-planetary-science-letters/vol/176/issue/3), 30
March 2000, Pages 527-542.

Gilmore et al., (2015) VIRTIS emissivity of Alpha Regio, Venus, with
implications for tessera composition. Icarus 254 (2015) 350--361.

López., I. and Hansen, V.L., 2008, Geologic map of the Helen Planitia
quadrangle (V--52), Venus: U.S. Geological Survey Scientific
Investigations Map 3026, 1:5,000,000 scale. (Available at
https://pubs.usgs.gov/sim/3026/)

Smrekar, et al. (2010) Recent hotspot volcanism on Venus from VIRTIS
emissivity data. Science, 328, 605-608.

Stofan, E.R., Smrekar, S.E., Mueller, N. and Helbert, J. 2016. Themis
Regio, Venus: Evidence for recent (?) volcanism from VIRTIS data.
Icarus. 271, 375-386.

Stofan, E.R., and Brian, A.W., 2012, Geologic map of the Themis Regio
quadrangle (V--53), Venus: U.S. Geological Survey Scientific
Investigations Map 3165, 1:5,000,000 scale. (Available at
<https://pubs.usgs.gov/sim/3165/>.)

Tanaka, K. L., Moore, H.J., Schaber, G. G., Chapman, M.G., Stofan, E.
R., Campbell, D. B., Davis, P. A., et al. (1994) The Venus geologic
mappers\' handbook (2d edition). US Department of the Interior, US
Geological Survey, Open-File Report 94-438 - available online
at: https://pubs.usgs.gov/of/1994/0438/report.pdf

Tanaka, K. L., Anderson, R., Dohm, J. M., Hansen, V., Pappalardo, R.,
Watters, Thomas R., and Schultz, R. A. 2010. \"[Planetary Structural
Mapping](https://repository.si.edu/handle/10088/20586).\" in *Planetary
Tectonics*, edited by Watters, Thomas R. and Schultz, R. A., 351--396.
Oxford, UK: Cambridge University Press.


