# Souffle Dominators Demo

This example demonstrates how [dominators](https://en.wikipedia.org/wiki/Dominator_(graph_theory)) can be computed using Souffle Datalog. The script `dominators.dl` defines `dominate(D,N)` relation that states that the node `D` dominates the node `N`. The CFG is represented using relations stored in the `example` directory.

The example can be executed using Docker:

    docker build . -t dominators-demo
    docker run dominators-demo

It should print dominators as follows:

    l1	l2
    l1	l3
    l1	l4
    l1	l5
    l1	l6
    l2	l3
    l5	l6
