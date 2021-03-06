# Protein aggregation molecular differential equation model  

## Full Network Model 
The goal was to create a model that could predict the size of the aggregated protein. To create the model we used a method outlined in the text *Mathematical Modelling in Systems Biology: An Introduction.* [^1] A graphic representation of our model is shown below. 

![](https://raw.githubusercontent.com/igem-waterloo/wiki2017/master/images/Full%20Network%20Model%20Graphic%20DE1.jpeg)


In our model, we have labeled one half of FYP as A and the other half as B. A and B may come together to form a dimer C. The dimer and singular half pieces A and B all aggregate into the final protein product D. 
The rate the cell creates A and B is  represented by the rate constant k1. The degradation of A and B is represented by the rate constants k7 and k8 respectively. The formation of the dimer is represented by the rate constant k4. The rate at which C, A, and B join into the final protein product D is represented by the rate constants k5, k2, and k3 respectively. Finally, the rate at which the protein aggregates degrades is represented by the rate constant k6. 
With the rate constants, we may use chemical mass actions kinetics to represent our model with a system of differential equations as follows. 

![](https://raw.githubusercontent.com/igem-waterloo/wiki2017/master/images/Full%20Network%20Model%20equations%20DE2.jpeg)

If we solve this system numerically and graph it we get the fallowing graph. 

![](https://raw.githubusercontent.com/igem-waterloo/wiki2017/master/images/Full%20Network%20Model%20Graph%20DE3%20.jpeg)

In the graph, the black curve represents the concentration of A and B with respect to time. The yellow curve represents the concentration of C with respect to time. The green curve represents the connection of D with respect to time. The concentration is in mol/L and time is in seconds. D is one protein so a “higher concentration of D” simply represents a larger protein. The numerical values shown in the graph are not important here and may not be accurate, they depend on the rate constants k1-k8 of our system, which is unknown. Rather the graph allows us to see the long-term behaviour of the different proteins in our model. Clearly, we can see that they all reach a steady state. That is to say that at a certain point the protein's contention does not change with time. 
Therefore, our model is making a prediction that makes sense when compared to reality, which gives us confidence that we are on the right track. However, the model as we have stated it thus far can only be solved numerically not analytically. Therefore let us create a simplified version of the model. 

## Simplified network model 

![](https://raw.githubusercontent.com/igem-waterloo/wiki2017/master/images/Simple%20Network%20Model%20Graphic%20DE4.jpeg)

In the simplified model rather than representing each half of FYP as A and B, we will represent it simply as one protein A. This simplification is valid because the dynamics of A and B are exactly the same. The aggregate protein is represented by B. 
The rate at which A is formed and degraded is represented by the rate constants k1 and k4 respectively. We will represent A turning into a dimer and joining the aggregate B with the rate constant k2. A can also join the aggregate as a single protein rather than a dimer which will be represented with the rate constant k5.  Finally, we will represent the degradation of B with the rate constant k3. Again we use chemical mass actions kinetics to represent the simplified model with a system of differential equations, as fallows. 

![](https://raw.githubusercontent.com/igem-waterloo/wiki2017/master/images/Simple%20Network%20model%20equations%20DE5.jpeg)

This system can be solved analytically if one assumes that at some point the concentration of A will no longer change. This assumption is valid from the graph earlier where we observed that all the protein systems reached steady state. Hence with the steady-state assumption, we can solve the system analytically as fallows. 

![](https://raw.githubusercontent.com/igem-waterloo/wiki2017/master/images/Simple%20Network%20model%20analysis%20DE6.jpeg)

Therefore it is possible that if one knows the final amount of aggregated protein [B] and if one knows the rate of degradation of that protein k3 one can find a constant L. With that constant and k3 it is possible to always know the amount of aggregate we will have in our system.  


[^1]: Ingalls, B. P. (2013). Mathematical modeling in systems biology: An introduction. Cambridge, MA: The MIT Press.

