# ModelAgnosticMLProject
GUI for Model-Agnostic Machine Learning model explanations for Rupture status Classification
******************************************************************************************
*                                                                                        *
*   G-MARC: GUI for Model-Agnostic model explanations for Rupture status Classification  *
*                                                                                        *
******************************************************************************************

This is a prototypical GUI which comprises of the following 4 model-agnostic 
model explanation techniques for rupture status classification:

    1.  Model Reliance technique for determining Global Feature Importance visualized 
        using Bar Plots     
    2.  Individual Conditional Expectation (ICE) Plots for determining relationship 
        between features
    3.  Determining counterfactuals of any feature of an instance visualized using
        Density Plots 
    4.  Determining value(s) and combination of features that is representative of 
        each class label by means of a Ruleset Model (RIPPER algorithm) visualized
        using Box Plots 
    
    Classes:    1. Ruptured(Aneurysm)
                2. Unruptured(Aneurysm)

------------------------------------------------------------------------------------------

->  All tabs in the GUI have a dropdown to select the model on which the dataset were
    pretrained. The details such as the performance of model, best hyperparameters and
    the hyperparameter grid values are mentioned right down the dropdown.

->  Toolbar: A widget which allows you to reposition/adjust, zoom, change layout, modify
             and save the plot. Additionally offers home, forward and backword buttons   

------------------------------------------------------------------------------------------

                    GUI Details

1.  . Shows the most important features per model.
    . Toolbar option available.

2.  . Shows ICE plots for each model.
    . The features are made available in the dropdown.
        . Features are sorted based on Model Reliance Technique.
    . Two types of ICE plots are made available: Normal ICE and Centered ICE.
    . Toolbar option available.

3.  . Shows density plots(Counterfactual) of feature(s) of instances.
    . A textbox to enter the instance number.
        . The number of instances ranges from [0-100)
    . If counterfactuals for the features of the selected instance are available,
      the features will be listed in the dropdown.
    . There is a very small error rate of the plot not loading up in the GUI. 
        . Please refresh(Refresh Button provided) or check the dropdown if it 
          has values in it.
        . If above step not satisfied then it means, no counterfactual for any 
          features was found for that particular instance    

4.  . Shows the range of values for the features that represents each class label using 
      Box plot.
        . Each class label represented using radio buttons
    . Toolbar option available
