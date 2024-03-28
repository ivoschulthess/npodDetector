# LUXE ECAL-E / NPOD Detector

Simulation tools for the LUXE ECAL-E and NPOD detector. 

Works with the DESY key4hep LUXE setup:

source /cvmfs/ilc.desy.de/key4hep/luxe_setup.sh



## Usage

On the DESY-NAF do ```$ source setup.sh``` to setup the environment. To display the geometry of a single module do ```$ geoDisplay generation/geometry/npodDetector_singleModule.xml```. To display some events with the module do ```$ ddsim --compactFile=./generation/geometry/npodDetector_singleModule.xml --runType=vis -G -N=1  --steeringFile steering.py --outputFile=tmp.root --gun.position "0.0 0.0 -10.0*cm" --gun.direction "0.0 0.0 1.0" --gun.energy "0.5*GeV" --part.userParticleHandler="" --gun.particle "pi0"```. This shoots a 500 MeV pi0 onto the detector. The pi0 has very similar properties as an ALP. In the interactive simulation, the viewer settings can be loaded with ```Idle> /control/execute/vis.mac``` and the particle gun can be triggered with ```Idle> /run/beamOn 1```. 




## Contact persons

I. Schulthess: ivo.schulthess at desy.de
