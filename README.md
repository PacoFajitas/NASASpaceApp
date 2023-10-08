# NASASpaceApp

Slide 1:
Title: Utilizing Artificial Neural Networks to Predict Geomagnetic Storms
Content:
Introduce the DSCOVR dataset and its significance in space weather forecasting.
Highlight the challenge: Predicting geomagnetic storms, quantified by the Kp index, based on various particle measurements.
Mention the problems with the DSCOVR instrument, such as electrical anomalies and noise in the data, which necessitates a robust predictive model.

Slide 2: Initial Data Exploration and Challenges
Title: Navigating Through the Noisy Spectra
Unraveling Frequencies: Share that the team initiated the analysis by exploring the frequency domain of the data via Fourier analysis, aiming to identify any dominant frequencies or patterns in the magnetic field disruptions.
Challenges Encountered: Describe how the data presented itself as notably wild and noisy, making it challenging to discern clear patterns or cyclic behaviors through Fourier analysis.
Shifting Focus: Explain the pivot to delve into the particle parameters (such as speed, density, and temperature) from the DSCOVR data, seeking to find more direct predictors for geomagnetic disturbances.
Linking Space to Earth: Highlight that while DSCOVR provided rich data, the objective was to understand and predict the magnetic field disruptions observed on Earth, emphasizing the importance of accurate prediction models for space weather forecasting.
So we chose to try and model extreme events with classifier Models
Visual:


Then the challenge was to match the frequencies of DISCOVR With earth kp 


Slide 2: Why Artificial Neural Networks (ANN)?
Title: The Power of ANN in Time-Series Prediction
Content:
Complexity Handling: ANNs can handle complex, non-linear relationships in the data, crucial for space weather prediction.
Adaptability: ANNs learn and adapt to patterns in the input data, potentially handling noisy signals from DSCOVR effectively.
Versatility: They can be tuned and adjusted (e.g., depth, neuron count, activation functions) to optimize for various predictive challenges.
We compared it to binary classifier and RNNs, and it showed a very more significant prediction capabilites
We used after using many other classifier (binary, RNNs)

Slide 3: Initial Model Architecture
Title: Crafting the Initial ANN Model
Content:
Model Structure: Discuss the architecture of the initial ANN model (input layer, hidden layers, output layer) and the activation functions employed.
Challenge Identification: Mention the challenges faced, such as overfitting or inadequate predictive performance, that motivated further optimization.
Visual: initial ANN architecture.

Slide 5: Fine-tuning and Experiments
Title: Experimental Approach to Model Improvement
Content:
Hyperparameter Tuning: Highlight experimentation with different neuron counts, and dropout rates to optimize the model.
Model Variations: Describe additional experiments (like varying model depth) and the rationale behind them for continual model enhancement.
Used Random Forest for feature importance because good for noise tolerance and Non-linear relationship

Slide 7: Conclusion

Highlight the potential impact of accurate predictions in the realm of space weather forecasting and related domains.
Achievements: mprovements observed through model optimization and what it means in the context of magnetic storm prediction.
Future Directions: Discuss potential future work, such as trying different neural network architectures (e.g., RNN, LSTM) or incorporating additional data.
Test more with different learning rates
