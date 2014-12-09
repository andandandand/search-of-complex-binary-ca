# **Search of Complex Binary Cellular Automata Using Behavioral Metrics**#

![self-rep3.PNG](https://bitbucket.org/repo/dodynj/images/4082026190-self-rep3.PNG)

Preprint, *Mathematica* demos of complex CA found, and search algorithm implementation in Java.

##Instructions to run the Discoverer search app##

*Java 6+ required. 

After downloading the discoverer_1_0.zip file, decompress it and run from a command line


```
#!bash

 java -jar discoverer_5_2.jar
```

Hitting the **RUN** button in the UI will start the genetic search of CA whose behavioral measures are close to the Game of the Life in the non-totalistic Moore neighborhood with radius = 1.

The cellular automaton in the population with behavior closer to the GoL will evolve on the right panel. 

**View Data** shows the log of all CA selected from the population. The app automatically saves all cellular automata with behavioral measures with less than 0.01 difference with the Game of Life and stores them using HSQL. This *"full completion"* may take several hours on a powerful computer (more RAM = faster completion). 

**Export to Mathematica** creates a notebook with the found automata with rule number specified in Wolfram code.