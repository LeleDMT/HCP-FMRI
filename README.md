# Is thinking about myself important to understand what others are thinking? 
Social cognition (SC) is a fundamental human skill which enables individuals to perceive, interpret, and respond to their social environment. During social cognitive tasks, increased BOLD activation is reported in brain regions within the Default Mode Network (DMN), a key network implicated in mentalizing and theory of mind. Whether pro-social personality traits, such as Agreeableness, modulate DMN activity during social cognition remain uncharted territory).

### However, does this relates to personnality trait?
 Can this also be related to personality traits? Does people that are more agreable tend to mentalize more people's emotion, through ther overlapping brain regions of the DNM and social cognition?

### Hypothesis
In our study, we hypothesized that individuals with higher Agreeableness scores would exhibit greater changes in activation within core DMN regions that are activated during a Theory of the Mind task (ToM)

## Method

We used the fMRI data and personality trait data X from the Human Connectome Project (n=100) acquired during a ToM task. We defined regions of interest (ROIs) using the Glasser parcellation, focusing on the Temporoparietal Junction, Medial Prefrontal Cortex, and Superior Temporal Sulcus activated during the ToM task. General Linear Model was employed to investigate the linear relationship between Agreeableness scores and BOLD activation contrasts (mental > random) at each of these DMN regions of interest.

## Results
No significant (p<0.05 Bonferroni-corrected) correlation between Agreebleness (and other traits) and Mental>Random fMRI contrast. Confounds included: Age, Gender

### Exploratory analysis : Machine learning


## Discussion
Agreeableness may not robustly modulate DMN activity during Theory of Mind tasks. 



# Files of the code
- fMRI.ipynb : Computing the contrasts between the Theory of the Mind task (ToM) and a random condition. Run this first to give a csv file with the average contrast of 100 subjects for the Temporoparietal Junction (TPJ), the Medial Prefrontal Cortex (mPFC) and the Superior Temporal Sulcus (TCC)
- HCP_personnality.ipynb : Concatenate the personnality data from hcp_behavior_unfiltered.csv with the average fMRI contrast to do GLM analysis
- HCP_personnality_ML.ipynb : Exploratory analysis, using machine learning, to attempt predicting personnality traits of the Big Five (Agreableness, Openness, Neuroticism, Extraversion, and Conscientiousness) using our average contrast
  - BONUS FILE (Thanks Abri) : voxelwise_task.ipynb uses the actual fMRI data (and not the timeseries that we had provided) to run the GLM analysis. It uses 100 participant of the HCP dataset. If you wanna download it on your machine, it's 200gb. Good luck!
