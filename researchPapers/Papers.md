#Research Papers

##Bio Inspired Robots

####[Biologically Inspired Approaches to Robotics](http://pdfs.semanticscholar.org/501b/9eb3c085a66abe4bdd56043fc802c21d0526.pdf)
- Notes/Summary:
    + Varying ranges of biological inspiration from ideas (legs) to copying mechanisms, structures and strategies (3)
    + Focused on invertebrate and insects, simpler than vertebrates while still exhibiting all the useful traits of a robot
    + Gait of an insect (cockroach))
        * static stability- support polygon contains center of mass almost always
        * 2 stages, stance and swing phase - timing very important
        * metachronal wave
            - slow one leg at a time
            - fast, front and back legs step in unison with middle leg of other side
            - leg swings propogate from back to front on each side
        * distributed system for control- no master/slave
    + Distributed Neural Controller(cockroach)
        * circuitry to recreate movement
        * pacemaker neuron, sensory neurons for leg limits (forward/back), motor neurons for foot state, rate swing forward and rate swing backwards. Common command neuron with pacemaker inhibiting adjacent legs
        * command neuron takes care of pacemaker inhibition rate and leg swing speed
        * This method was robust and could survive loss of sensor
        * further development was looked at with a stick insect and shifting limits to trigger the next action
        * Genetic algorithms were also trained to use sensor data when available but not rely on it. 
    + Rough Terrain
        * passive and active compliance: springs to resist at first and force feedback to eventually 
        * search reflex
        * stepping relfex to reposition
        * elevator reflex
    + Working with K^2T Inc for a prototype robot for finding and destroying mines
- Questions:
    + What is a leaky integrator?
        * short term memory integrator also a lowpass filter far from frequency of interest
    + Do these methods extend to leg motions that are on opposite sides?
    + What if there are > or < 6 legs? 
    + Is static stability necessary?
    + How do these react to a missing leg?
- Extensions:
    + Try applying similar logic to different structures- ie quadrupeds, bipeds etc... 
    + [Website for biologically inspired Robotics] (http://biorobots.case.edu/projects/k2t-inc-walking-robot/)
####[The First Takeoff of a Biologically Inspired At-Scale Robotic Insect](http://www.micro.seas.harvard.edu/papers/TRO08_Wood.pdf)
- Notes/Summary
    + Insect Flight 
    + Single DOF flight tests- just thrust
    + great performance/thrust to weight ratio using similar flight pattern and wing control as an insect
    + Dipteran Dosoventral muscles with bidirectional force to cause acutation
    + Operate a natural frequency of aeromechanical system
- Questions
    + How far does battery technology need to come to provide power to the insect
    + How would a single actuator manage to control the flight?
    + Is this systems stability similar to insects in how it can recover from collisions?
- Extensions
    + Try different frequencies for the wing beats to determine if the resonant frequency is optimal
    + Create multiple insects and try a multirotor/wing approach... does it scale well? 

