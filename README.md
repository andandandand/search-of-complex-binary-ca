# **Search of Complex Binary Cellular Automata Using Behavioral Metrics**#

![self-rep3.PNG](https://bitbucket.org/repo/dodynj/images/4082026190-self-rep3.PNG)

Preprint, *Mathematica* demos of complex CA found, and search algorithm implementation in Java.

##Instructions to run the Discoverer search app##

![ca-discoverer.png](https://bitbucket.org/repo/dodynj/images/244061540-ca-discoverer.png)

***Java 6+ required.** 

After downloading the discoverer_1_0.zip file, decompress it and run from a command line


```
#!bash

 java -jar ca-discoverer.jar
```

Hitting the **RUN** button in the UI will start the genetic search of CA whose behavioral measures are close to the Game of the Life in the non-totalistic Moore neighborhood with radius = 1.

The cellular automaton in the population with behavior closer to the GoL will evolve on the right panel. 

**Examine Fittest** shows the log of all CA selected from the population. The app automatically saves all cellular automata with behavioral measures with less than 0.01 difference with the Game of Life and stores them using HSQL. This automatic  *"full completion"* may take several hours on a powerful computer (more RAM = faster completion). 

**Configuration** allows the definition of the grid size, the number of chromosomes in the search population, and the interval between samples used to estimate the behavior of the automata in the population. 

**Export to Mathematica** creates a notebook with the found automata, their rule numbers are specified in Wolfram code. The file must be saved with an .nb extension. After opening, go to *Evaluation -> Evaluate Notebook*. 