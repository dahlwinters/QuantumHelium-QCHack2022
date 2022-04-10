# QuantumHelium-QCHack2022

# Community Organization Over a Quantum-Optimized Helium Network
A submission to the 24-hour Amazon Braket challenge for QC Hack 2022:
Quantum Optimization of the Helium Network for the Denver Area

## Problem Description

Helium is a blockchain for low power IoT devices, allowing communication over
long distances. It is a decentralized wireless connectivity platform that could
be used for emergency communications if the electricity went out and took out
both the internet as well as cellular services. This could happen either due
to natural disasters or conflict situations (i.e. Ukraine).

The goal of this submission was to divide the HNT network into 5 communities
that were closely bound together, to offer redundancy in the network if for
example a large portion of the network were to go down. 

A Delaunay triangulation was used to form the graph connecting the hotspots, 
but in reality other measures could be used, such as how many transactions
were passed between the hotspots per day.

Below is a map of the Helium hotspots in the Denver area. This is a global network.

![Denver Area in HeliumVision](https://github.com/dahlwinters/QuantumHelium-QCHack2022/blob/main/images/Denver_HeliumVision.png)

And below is more of a closeup of the data.
![Denver Area in Helium Explorer](https://github.com/dahlwinters/QuantumHelium-QCHack2022/blob/main/images/Denver_Helium_Explorer.png)

## Results
A QUBO representation was used and deployed in hybrid fashion on the D-Wave Advantage 
QPU through Amazon Braket. It yielded an improved modularity result 
(0.44691752481705127) over the classical implementation (0.46611572091086173).

The community breakdown into 5 subcommunities is shown below.
![D-Wave Advantage QPU Hybrid Result](https://github.com/dahlwinters/QuantumHelium-QCHack2022/blob/main/output/2022-04-10%2013%2001%2033_HNTDenver_DwaveQBSolv_hybrid_5_comm_modu_0.4469.png)

## Instructions on Running the Project

Load the Jupyter Notebook and the src folder into Amazon Braket and run all
the cells. That's it! The output will go into the Output folder and will also
display in the notebook.
