# GLIDE-Linux

GLIDE is learning software. It uses calculations that the Forgetting Curve depend on, for the spacing of study rehearsals. GLIDE prevents the decay of the ability to retrieve information, from dropping too far below 95%. This means that everything a person studies through GLIDE, will be remembered if it is used regularly.



# Programming Language

Development of GLIDE-Linux will primarily be in the C programming language. The documentation for the API’s are much more thorough, and up-to-date, than anything in MonoDevelop. I’ve already built a lot of GUI pieces quicker than I could in MonoDevelop, due to their poor documentation maintenance.

The UWP version will probably remain in C#. C is just easier to work with on Linux right now.




# Calculation Problems

The only problem that may exist with the calculations, is the determination of difficulty, and the length of the interval between the first, and the second, study of new information. 

The length of the very first interval between study repetitions, is not given in the research that I used. This value is needed, for the calculation of difficulty, to calculate against after every repetition. I used 24 hours, (1440 minutes), because a lot of research supports this time frame.

There was no formula available, from any of the research that I have found yet, that was used to calculate the difficulty of an engram. The formula I use does work perfectly, (the Slope-Intercept formula), but the two values that I use, may be slightly off.  Difficulty is used to determine the length of an interval between repetitions. I chose the values of 1.3, and 2.5, for the maximum, and minimum, levels of difficulty, respectively. The maximum difficulty at 1.3, yields a shorter interval between repetitions, for a particular engram, the minimum value of 2.5, increases the length of an interval between repetitions for a particular engram. Therefore; difficult information is studied more often, than easier information.
