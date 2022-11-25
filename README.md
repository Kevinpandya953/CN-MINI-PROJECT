# CN-MINI-PROJECT

ABSTRACT


Open Shortest Path First (OSPF) is a link-state routing protocol that was developed for IP networks and is based on the Shortest Path First (SPF) algorithm. OSPF is an Interior Gateway Protocol (IGP).
In an OSPF network, routers or systems within the same area maintain an identical link-state database that describes the topology of the area. Each router or system in the area generates its link-state database from the link-state advertisements (LSAs) that it receives from all the other routers or systems in the same area and the LSAs that itself generates. An LSA is a packet that contains information about neighbors and path costs. Based on the link-state database, each router or system calculates a shortest-path spanning tree, with itself as the root, using the SPF algorithm.
OSPF has the following key advantages:
•	Compared with distance-vector routing protocols such as the Routing Information Protocol (RIP), OSPF is more suitable for serving large, heterogeneous internetworks. OSPF can recalculate the routes in a short amount of time when the network topology changes.
•	With OSPF, you can divide an Autonomous System (AS) into areas and keep area topologies separate to decrease the OSPF routing traffic and the size of the link-state database of each area.
•	OSPF provides equal-cost multipath routing. You can add duplicate routes to the TCP stack using different next hops.
We are building a software for simulation using Python(VS code) and Py game(visuals) in which user can add some nodes (Here node is a router) and make a topology or can use existing topologies like mesh or ring and then can ping a node from any other node and find the shortest path between them using dijkstra algorithm which is also called as Open Shortest Path First (OSPF).



INTRODUCTION



This program demonstrates the work of the OSPF protocol. Python is used and for visualization this program uses pygame library. Routers are imitated by separate processes. ( by multiprocessing python library)


In the beginning there are two processes:
•	main process with thread for input
•	display process

Then for each router adds the process.

In this program there are 2 built-in constants:
•	Max count of existing routers (15 by default)
•	Max router signal range (0.25 by default)

They could be changed in ospf_net.py file.

 


PROBLEM STATEMENT


In the new age of computing, a lot of devices are rolled out in public 
Which are connected to internet and as the density of devices increases there comes complications in connecting those devices to internet in an efficient manner. 


To overcome that issue we are implementing a routing protocol called as Open Shortest Path First (OSPF) which connects the network devices in most efficient manner by taking the least number of passing nodes to reduce latency in network.




IMPLEMENTATION


Our expected end product will have capacity to arrange the nodes in      some topology or users on choice and find the shortest path between 2 nodes.

	Method:
•	Add router to the window with (x, y) router coordinates; (x, y) must be in range [0;1]
•	Ping from one (existing) router to another to see the path; each router has it ones id’s (it represents on the window)
•	Run one of three pat scenarios: circle, polygon or mill; it adds a couple of routers by one command
•	Command help for full report
•	Command exit for correct program terminate



REFERENCES

https://www.linkedin.com/pulse/ospf-protocol-implementing-dijkstras-algorithm-ayush-ganatra/
https://medium.com/@kp-the-great/how-ospf-protocol-implements-dijkstra-algorithm-53c390199ee8
https://www.pygame.org/docs/
http://web.mit.edu/modiano/www/6.263/lec18.pdf

