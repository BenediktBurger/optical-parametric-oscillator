# Optical Parametric Oscillator

Open source hardware for a continuous wave optical parametric oscillator (OPO) in the mid-infrared regime.

[![DOI](https://zenodo.org/badge/392327989.svg)](https://zenodo.org/badge/latestdoi/392327989)

## History

We needed a narrowband, tunable, continuous wave light source for coherent radiation at 606 nm. The result is this optical parametric oscillator with intra-cavity sum frequency generation, similar to a special version of the Aculight Argos 2400 laser system previously sold by Lockheed Martin. This is described in *Tunable, continuous-wave optical parametric oscillator with more than 1W output power in the orange visible spectrum* by S. Mieth et al. [DOI10.1364/OE.22.011182](https://www.osapublishing.org/oe/abstract.cfm?uri=oe-22-9-11182).

The design works for mid-infrared laser light as well, if the sum frequency part is left out. In fact, we use a second model with different mirror coatings and crystal for light at 2550 nm.


## Design Overview

The optical parametric oscillator consists in a bow-tie cavity (two concave mirrors with curvature radius of 100 mm and two planar mirrors) and a periodically poled lithium niobate crystal.

A pump laser at 1064 nm, focused into the center of the crystal, provides power for the difference frequency generation. The cavity is resonant (by mirror design) for one frequency (the *signal*) such that this frequency is amplified and the difference frequency (*idler*) is generated and emitted (see *singly resonant optical parametric oscillator*).

An etalon in the cavity (in the second focus) allows longitudinal mode selection for the signal wave.


## Folder Contents

- *designs* contains 3D designs.
- *drawings* contains some corresponding technical drawings.
- *images* contains some images and schematics of the design.
- *documentation* contains documentation of the setup.


## Construction

-The pump laser is a fiber laser by *IPG Photonics* (YAR-15K) with up to 15 W at 1064 nm. Its fiber tip contains a collimation unit (called *collimator*) with an additional clamp (made by Aculight) in order to mount it repeatedly with the same polarisation.
- Two highly reflective mirrors (1 inch diameter), mounted in *Thorlabs Polaris K1F* allow the pump beam to be adjusted.
- This collimator is mounted into the *OPO-Block* (see 3D file in *designs*) with a horizontal polarisation.
- A 0.5 inch lens with 62.9 mm focal length (*Newport KPX052AR.33*) focusses the pump power into the nonlinear crystal. It is mounted with the *Linsenhalter* (in designs).
- The nonlinear crystal is made of magnesium oxide doped (5%) lithium niobate with a periodic poling for *quasi phase matching*. A fanout structure of the poling period allows tuning via vertical translation. Use [SNLO](https://as-photonics.com/products/snlo/) for calculating the poling period. *HC Photonics* is capable of producing this crystal.
- The crystal is mounted in a heating oven (*HC Photonics TC038D*) for temperature controlling. For a python API controlling the oven temperature see [pymeasure](https://pymeasure.readthedocs.io).
- The oven is mounted to the OPO-Block via a translation stage (*Thorlabs XR25P_M*) and *Ofen-Adapterplatte* (in designs)
- Four specially coated 25mm mirrors (Anti-reflection for 1064 and the idler on both sides. Anti-reflection coating is for the signal on the outside and high-reflection on the inside), two mirrors with concave curvature of 100 mm (next to the oven) and two planar ones, form the cavity. Laseroptik made them in our case. Most important is the high reflectivity for the signal.
- One mirror is glued into the OPO-Block, one is mounted with a SM1 ring from Thorlabs and the other two (on the output side of the Block) are mounted with *Thorlabs Polaris K25F4_M* in order to adjust the cavity.
- Finally the Etalon is glued to a comercially available galvanometer (for Lasershows) and mounted to the lid *Deckel LwG* (in designs), which in turn is mounted on top of the OPO-Block to provide radiation blocking and reduce dust entering the cavity.
- For the setup and adjustments refer the files in *documentation*.


## Disclaimer

These files are provided by the copyright holders and contributors "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimened. In no event shall the copyright owner or contributors be liable for any direct, indicrect, insidental, special, exemplary, or consequential damages however caused and on any theory of liability, wheter in contract, strict liability, ort tort (including negligence or otherwise) arising in any way out of the use of these files, even if advised of the possibility of such damage.

This is a class IV laser system. Adhere to local regulations and apply necessary safetey measurements.
