## Using AI-Camera for People Tracking

**Roland Unger**

### Executive summary
**Project overview and goals:** <br>The goal of this project is to analyze the people moving and forecasting the movement for further action in an alarm control system.<br>
**Findings:**<br> The current best model is an `ARIMA` forecast model with an well performed forecast of 5 seconds.<br>
**Results and conclusion:**<br> The evaluation of the best model returned a comparsion with fitting time and forecast plots of the given dataset.<br>

### Rationale
In a common CCTV surveillance system an operator is watching abnormal behavior and reacting manually.
If the system is big, lets say 200 cameras, it is hard or unpossible to recognize the attacker.
Therefore a AI-model should filter and select the interesting cameras to the operator monitor.
Furthermore the model could start automatic actions on an alarm control system like:<br>
- Switch the selected cameras to an alarm monitor (multiple camera view on one monitor). 
- Predict the people moving from the last movement and see if the person will go over a specific virtual line (trip wire) in the near future. If so, an action could be released similar to point 1. The prediction gives the operator more time to react on the attacker´s behavior.  
- The predicting function of the model should find the person after covering from an other person in the picture or some other    object in the scene.
- The model should find abnormal behavior of people movement: Change of moving speed (slow to run), abnormal moving

### Research Question
The question this project aims to answer is what is the best forecast model with the fastest fitting and longest forecast time.

### Data Sources
The data source come from an AI-camera output meta data stream. The meta data contain <br>
- Timestamp of the detection
- Location of the detected object (x and y coordinates)
- Size of the object (bounding box)
- Classification (person, car, bike etc.)

### Methodology
First data cleaning and peparations was done. Furthermore the important features was selected and a base line ARIMA model was set up.<br>
Next, with a cross validation function the best hyperparameter was selected. The results was stored in a comparsion dictionary and plotted for better understanding.

### Results
What did your research find?

### Next steps
What suggestions do you have for next steps?

### Outline of project

- [Link to notebook 1](https://github.com/te8titan/Capstone_project_II)


#### Contact and Further Information

Roland Unger
Email: te8@titan-electronic.com