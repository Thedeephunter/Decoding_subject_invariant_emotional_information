# Decoding_subject_invariant_emotional_information
There are five files in this repository:
- **SVM4PCERS:** Code for data-scaling, feature selection, model training, and subject-dependent and subject-independent cross-validation. 
  
- **subject_independent_dataset & subject_dependent_set:** These two dataset are input for subject-independent and subject-dependent cross-validation, respectively. Both sets contain **exactly the same data**, they differ in the order of arrangement. 
  
  In the **subject_independent_dataset**, data is organized according to subject identity, with samples grouped by subject. In contrast, the **subject_dependent_set** is constructed by shuffling all samples from different subjects to ensuring a subject-dependent cross-validation. Meanwhile, the distribution of emotional categories remains consistent across all folds of the cross-validation.
  
  The column order in both datasets is as follows: _emotion, subject, arousal valence and features_. Each row corresponds to the data collected from a single trial.
  
- **statistical_analysis4PCERS**: The code used for statistical analysis
  
- **Feature**: The same data and order as **subject_independent_dataset**, except that the _arousal_ and _valence_ columns are omitted. It is an Excel file with column headers, making it convenient to load as a panda DataFrame in Python.
