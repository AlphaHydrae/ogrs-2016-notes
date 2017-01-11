# OGRS 2016 - SpatiaLite Workshop

## ISO Topology

https://www.gaia-gis.it/fossil/libspatialite/wiki?name=topo-intro

* Types: nodes, edges, faces.
* Nodes and edges can be *dangling* (or *isolated*).
* Every node must have a unique id.
* Nodes cannot share the same spatial coordinates.
* Edges are linestrings.
* Two edges can never cross (a node must be used).
* Nodes with edges cannot be removed before removing the edges.
* Edges start at a starting node and end at an ending node.
* Faces are defined by nodes and edges.
* Polygons are represented by one or multiple faces.

> ISO topology is a very nice mathematical gadget, but it requires a lot of intelligence to use in production. It’s like a very nice gun. You can do anything with it, including shoot yourself in the foot.

## Databases implementing ISO Toplogy

* Oracle spatial
* PostGIS
* SpatiaLite

## Networks

* Examples: roads, eletrical network, water pipes, etc.
* Edges are called links.
* There are no faces.
* Crossings with no intersections are allowed.
* Two nodes can overlap.
* Can have no geographical representation (e.g. graph theory applied to genetics).

## Issues

* Floating point geo computations are not precise enough.
  Sometimes the calculated intersection of two edges do not overlap either of them due to lack of precision.
* Use snap functions to mitigate the issue.
