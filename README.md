# Telecom-Frequency-Allocation-using-DSATUR
Efficient frequency allocation for telecom towers using the DSATUR graph-colouring algorithm to prevent interference and optimize spectrum usage.
Telecommunication networks contain thousands of cellular towers that must operate without interference. As tower density increases, assigning frequencies becomes challenging because nearby towers sharing the same frequency can cause co-channel interference and degrade network quality.
This project uses a graph-theoretic approach with the DSATUR (Degree of Saturation) graph colouring algorithm, where towers are modelled as nodes and interference links as edges. DSATUR assigns the minimum number of frequencies while ensuring no two interfering towers use the same one.
The implementation includes dataset processing, interference graph construction using BallTree, DSATUR-based frequency allocation, visualization, and performance evaluation.

#Problem Overview
Telecom towers operate with limited spectrum, and overlapping coverage can cause interference. To avoid this, frequencies must be assigned so that no two nearby towers share the same one. By modelling towers as graph nodes and interference as edges, graph colouring provides an efficient, scalable solution for conflict-free frequency allocation.

#Algorithm Selection — DSATUR
DSATUR (Degree of Saturation) is used for frequency allocation because it efficiently colours large, dense graphs like telecom tower networks. It prioritizes nodes with the highest saturation and assigns the smallest available colour, ensuring minimal frequencies and zero interference.
Using DSATUR, all 23,499 towers were coloured with 0 conflicts, supported by BallTree for fast neighbour detection and efficient graph construction.

#Conclusion
Graph colouring provides an efficient and scalable solution for telecom frequency allocation. By modelling towers as vertices and interference as edges, frequencies can be assigned without conflicts, reducing interference and improving network quality. The results show that heuristic algorithms like DSATUR deliver reliable, fast, and spectrum-efficient frequency planning suitable for real-world telecom networks. This approach also supports future scalability as networks expand and demand grows.
