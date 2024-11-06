Parkinson's Disease Prediction using Voice Measurements
Overview
This project leverages machine learning to predict Parkinson's disease status using vocal measurements. Parkinson's Disease (PD) is a progressive neurological disorder often diagnosed through clinical observations of motor skills and neurological history. However, early detection is challenging due to the lack of definitive lab tests and the subtlety of initial symptoms. This project demonstrates a non-invasive, data-driven approach to screen for PD using vocal characteristics.

Dataset
The dataset, available from the UCI Machine Learning Repository, includes vocal features from individuals with and without Parkinson's Disease. The vocal attributes capture frequency and amplitude variations, noise ratios, and non-linear dynamical complexity, which are characteristic in PD-afflicted speech.

Context: PD leads to speech impairments, such as difficulty in articulating sounds (dysarthria), reduced volume (hypophonia), and limited pitch variation (monotone speech). These changes make voice recordings an effective screening tool, potentially reducing clinic visits and aiding early intervention.
Attribute Information
Key attributes:

MDVP
(Hz), MDVP
(Hz), MDVP
(Hz): Measures of vocal fundamental frequency.
MDVP
(%) and MDVP
: Indicators of frequency and amplitude variations.
NHR, HNR: Noise-to-harmonic ratio measures.
status: Indicates PD status (1 for Parkinson's, 0 for healthy).
Additional non-linear measures include RPDE, DFA, and PPE for fundamental frequency variation.
Full Dataset Information

Citation
If using this dataset, please cite:

'Exploiting Nonlinear Recurrence and Fractal Scaling Properties for Voice Disorder Detection',
Little MA, McSharry PE, Roberts SJ, Costello DAE, Moroz IM.
BioMedical Engineering Online, 2007, 6:23 (26 June 2007)

Project Approach
Data Preprocessing: Applied standardization and split the data into training and test sets.
Modeling: Used a RandomForestClassifier to classify individuals as having Parkinson’s or not, followed by hyperparameter tuning.
Evaluation: Assessed the model with accuracy, precision, recall, F1-score, and confusion matrix.
Results
The model achieved a 77% accuracy on the test set, demonstrating strong predictive performance for identifying Parkinson's cases.

Tools
Python: pandas, numpy, matplotlib, seaborn, scikit-learn
Jupyter Notebook: Complete analysis and code documentation.
Future Work
The results and feature importance analysis will be visualized in Tableau for deeper insights, potentially aiding clinical understanding.

