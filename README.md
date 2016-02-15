# StringTheoryTools

## What is going on in this repo?

This repository is a collection of various tools (written in Mathematica) used in String theory/Supergravity such as [T duality](https://en.wikipedia.org/wiki/T-duality), [S duality](https://en.wikipedia.org/wiki/S-duality), rotations, boosts, some differential geometry, etc. So far all the functions are collected in two packages **DiffGeometry.m** and **TransformationRules.m**. Usage of every function is shown in various examples, e.g. *Example...*.


## Some details. Structure of the repository

Package **TransformationRules.m** implements boosts, rotations, S duality and T duality for NS-NS fields.

A great example of utilizing boosts and T/S dualities is a beautiful solution-generating technique (here by solutions we mean that they solve the equations of motion, such as Einstein and Maxwell equations), in which you start with a simple solution and by performing a series of tranformations obtain something new. This solution-generating technique was used to [construct](http://arxiv.org/abs/hep-th/0105136) [fuzzballs](https://en.wikipedia.org/wiki/Fuzzball_(string_theory)).

An example of using the package is presented in *Example.KerrToD1.nb*, in which you start with a rotating black hole in 4 dimensions (Kerr black hole) and perform the series of tranformations, namely: "add flat direction"->"boost"-"T duality"->"S duality", to obtain the D1 brane. At the end we take the extremal non-rotating limit to check that the result is the well-known supersymmetric D1 brane.

Package **DiffGemetry.m** implements computation of connections (Christoffel symbols), Riemann and Ricci tensors, Ricci scalar and spin connections.

One simple example of using the package is presented *Example.AdS2xS2.nb*, in which the Einstein equations are checked for AdS2, S2 and AdS2xS2.

Another example is *Example.SUSY.IIB.nb*, in which we solve SUSY (Killing spinor) equations of type IIB supergravity in the NS-NS sector for one particular background - the near horizon NS5 brane.

## FAQ:

1. Why bother writing this code and not just use other available libs/frameworks?

I am not sure if there are any open source libs implemeting what I needed, but even if there are, it is better to write my own code to get a better understanding and eliminate errors due to other people :)


## TODO: 

1. Add more detailed description in README file.
2. Add Sen-Hassan-Cvetic method using large matrices to perform a series of dualities in one rotation [arxiv:hep-th/9512127](http://arxiv.org/abs/hep-th/9512127)
2. Implement duality rules for RR-fields
