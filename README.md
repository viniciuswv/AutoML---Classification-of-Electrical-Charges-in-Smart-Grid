# AutoML---Classification-of-Electrical-Charges-in-Smart-Grid
[AutoML] Hyperparameter adjustment of a classification model for high similarity electrical charges in a smart grid

This code was developed as a dissertation project by (VIANNA, 2021), for the implementation and investigation of an two stages based optimization for automatically configuring a hyperparameters set of interest in the convolutional neural network (CNN) originally developed in (FIRMES, 2020), whose objective is to classify 16 possible combinations of two types of highly similar electrical charges (lamps and PCs) on a test bench.

Highlights:

The first step is to apply the Hill Climb(down) optimization, in order to investigate how far it is possible to reduce the data (organized in "cases") while maintaining the network's test accuracy greater than or equal to 95%.

The second step is to apply the Bayesian optimization, in order to investigate whether it's possible to make the network valid accuracy close to 100%, by automatically selecting a good set of hyperparameters.

Was necessary to adjust some network learning parameters to improve the robustness and stability during training and validation, otherwise, the Hillclimb optimizer could be stuck in a local minimum.
