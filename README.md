# Tarry's Traversal Algorithm OMNeT++ Implementation

### Description

This is a student project made for "Distributed Systems" course of department of Informatics - Ionian University. The main purpose of the project is to implement Tarry's Traversal Algorithm, run it on various networks with random topologies and compare algorithm's complexity-theory (message passes) with the results of the simulations.

##### [Report (greek)](https://github.com/p17griv/tarrys-traversal-algorithm-implementation/blob/master/report%20-%20greek.pdf)

### About Tarry's Algorithm

Tarry's algorithm is a random graph traversal algorithm defined in 1895. Algorithm's functionality is based on two rules:
* A node does not forward the token twice through the same channel and
* A node (not defined as initiator) forwards the token to his parent node* only if there isn't other available channel through which he hasn't sent.

The algorithm does <b>2*E</b> (E = number of network edges) message forwards because the token is sent only once through each direction of each channel - network edge.

###### *parent node: the node who sent the token for the first time for each node.

### How to run - Instructions

1. Download and install [OMNet++](https://omnetpp.org/download/) (tested on 5.6.2 version)
2. Run ```git clone (git url of the repository)``` into a directory in order to download the project.
3. Open OMNeT++ IDE
4. Go to ```File > Open Project from File System...``` and define the project directory as the "Import source"
5. Open the "omnetpp.ini" file and run the simulation.
