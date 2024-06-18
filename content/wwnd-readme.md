FOCAL POINTS - Working with network data
========================================

Working with network data
James Bagrow and Yong-Yeol Ahn
2024

https://cambridge.org/network-data

Our book uses six *focal points*, real-world networks, as examples to
illustrate common issues and practices. Here we provide these networks for you
to download and use. Some networks come in multiple forms, such as both static
and dynamic representations and many have attributes associated with the nodes
or edges. Each network provided in GraphML and GML files; most libraries
such as NetworkX and igraph support these formats.

Below we discuss some specifics for each network. Please see our book for more
information.



Zachary Karate Club
-------------------

The famous Zachary Karate Club. This network represent members of a university
martial arts club who interacted heavily outside the club, according to surveys
gathered by Wayne Zachary during the early 1970s. This club had a disagreement
and split into two groups, one following the club president and the other the
club's karate instructor. This group information is available in the `group`
node attribute. 

Original data `karate.mtx` (retrieved 22 August 2022) available at:  
https://www.cise.ufl.edu/research/sparse/matrices/Newman/karate

Reference:
W. W. Zachary, An information flow model for conflict and fission in small
groups, Journal of Anthropological Research 33, 452-473 (1977).
https://doi.org/10.1086/jar.33.4.3629752



Plant-pollinator network
------------------------

A network where nodes are either plant or pollinator species and links exist
only from plant to pollinator when field observations were made of that
pollinator acting to pollinate that plant. Nodes are identified by species
names. This network was collected from field observations conducted in Spain.

Original data (network ID `M_PL_058`) (retrieved 22 August 2022) available at:
https://www.web-of-life.es/

Reference:  
Bartomeus, I., Vilà, M. & Santamaría, L. Contrasting effects of invasive plants
in plant–pollinator networks. Oecologia 155, 761–770 (2008).
https://doi.org/10.1007/s00442-007-0946-1



Developer collaboration network
-------------------------------

A network representing software developers contributing to open source projects
hosted by IBM on the GitHub online development platform. Nodes represent
developers (identified by their GitHub usernames) and links connect developers
who have edited one or more source code files in common, a simple measure of
collaboration. We treat the network as weighted by associating with each link a
weight counting the number of files commonly edited by the two developers.

The `dynamic` directory contains yearly snapshots of the network from 2013--2017.


Original data (deposited 26 March 2019) available at:  
https://doi.org/10.6084/m9.figshare.7893002.v1

Reference:  
Bagrow, J., Bollt, E. An information-theoretic, all-scales approach to
comparing networks. Appl Netw Sci 4, 45 (2019).
https://doi.org/10.1007/s41109-019-0156-x



Flavor network
--------------

A network representing recipe ingredients and the flavor molecules they
contain, extracted from food science reference texts. Nodes are identified with
integers prepended with "i" if the node is an ingredient or "c" if it is a
flavor chemical. Associated with each ingredient is its name and category.
Associated with each chemical is its name and CAS number.

The `backbone` directory contains the multiscale backbone (Ch. 10) visualized
in the original reference and in Ch. 1.

_Note_: 
It was discovered by Augustine Koh (ak.augustine.koh@gmail.com) and Lav
Varshney (varshney@illinois.edu) that "Farnesol", a flavor compound, is present
both as an ingredient (ID i339) and compound (ID c951). Thus, you may want to
remove farnesol from the ingredient list and from the ingredient-compound
network.

Original data `ingr_comp.zip` and `flavor_network_backbone.zip` (retrieved 20
October 2022) available at:
https://yongyeol.com/2011/12/15/paper-flavor-network.html

Reference:  
Ahn, YY., Ahnert, S., Bagrow, J. et al. Flavor network and the principles of
food pairing. Sci Rep 1, 196 (2011).
https://doi.org/10.1038/srep00196



Human Reference Interactome
---------------------------

A protein-protein interaction network derived from high-throughput assays.
Nodes are represented by standardized IDs that can be connected to GENCODE gene
annotation metadata.

Original data `HuRI.tsv` (retrieved 22 August 2022) available at:  
http://www.interactome-atlas.org/download

Reference:  
Luck, K., Kim, DK., Lambourne, L. et al. A reference map of the human binary
protein interactome. Nature 580, 402–408 (2020).
https://doi.org/10.1038/s41586-020-2188-x



Malawi Sociometer Network
-------------------------

A face-to-face contact network between 86 individuals living in a rural village
in Malawi.  Edge weights denote the number of contacts between individuals
during the study.

The `dynamic` directory contains the dynamic network stored as a multigraph.
Note that the contact day has been renumbered compared to the original release
to match the contact time.

Original data `tnet_malawi_pilot.csv` (retrieved 22 August 2022) available at:  
http://www.sociopatterns.org/datasets/contact-patterns-in-a-village-in-rural-malawi/

Reference:  
Ozella, L. et al., Using wearable proximity sensors to characterize social
contact patterns in a village of rural Malawi, EPJ Data Science 10, 46 (2021).
https://doi.org/10.1140/epjds/s13688-021-00302-w

