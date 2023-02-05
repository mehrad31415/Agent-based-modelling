# Agent-based-modelling
This is an agent based model in NetLogo. 

## WHAT IS IT?

This is a simple virus spreading model. The model consists of only of breed of *turtles*.

## HOW IT WORKS

Each turtle has three specific attributes: 1 - whether they have a virus or not denoted by the *virus?* variable. 2 - whether they are immune or not denoted by the *immune?* variable. 3 - Lastly a *period* variable which keeps track of how long - i.e., how many ticks - they have been immune/infected. The *normal* turtles are indicated by *green*, the *infected* by *red*, and finally, the *immune* by *blue*. In short, the infected turtles can spread the virus to the normal ones, however, the immune ones do not get infected. The turtles will only be infected if they pass through a neighbouring *patch* of an infected turtle. The infected turtles have a chance of being cured, if so, they will become immune to the disease; but if not cured after a certain amount of time, then they will die due to illness. The immune turtles, will not stay immune forever and after a certain period of time will lose immunity (become normal). Also, these turtles, reproduce in a way that normal turtles produce normal ones, the infected ones produce infected ones, and the immune ones produce immune ones. Overall, the cycle is:
```
Immune -> Normal -> Infected -> Immune -> Normal ....
```
## HOW TO USE IT

There are many parameters the user can control using the interface tab. The number of turtles, the step-size of the movement of the turtles, the number of infected turtles in the initialization, the number of immune turtles in the initialization, the percentage of which an infected turtle will be cured (and thus immune), the number of reproduction per ticks, the direction/angle of movement of the agents, the duration for which an infected turtle has time before dying, the duration for which the turtle will stay immune before becoming normal (and thus prone to the disease again) are all controlled. Three monitors show the number of people, the number of infected people, and the number of immune people continuously through the simulation. A plot is drawn continuously for the respective numbers. Ultimately, there is a switch that when turned on can show the connections between the turtles, in other words, we can see which turtles have infected whom.

## THINGS TO NOTICE

Given the high number of parameters to control, I suggest keeping them at a standard logical rate and changing them only one by one to prevent further confusion. Also, given the experiment one wants to carry out not all the parameters are important for testing.

## THINGS TO TRY

I highly suggest playing with the immunity-duration, dying-duration, production, and immunity percentage sliders. These variable respectively indicate, the duration which an immune turtle remains immune, the duration which an infected turtle - if not cured - has before dying, the number of offsprings each turtle can produce, and the percentage of chance which an infected turtle has to be cured (become immune). 

## EXTENDING THE MODEL

For accuracy, I suppose dividing the turtles into three breeds (immune, infected, and normal) would help divide them. However, I do not know whether *NetLogo* allows conversion between breeds. Also finding the root of the networks in the connections of the turtles will be a nice project. This will lead to finding the initial turtles which caused infection out of a popultion. 

## RELATED MODELS

I have noticed that there is a model called *virus* in the model library. There might be similarities between my created model and this model. However, this model was inspired and created from the frame *Communication T-T Example*. 
