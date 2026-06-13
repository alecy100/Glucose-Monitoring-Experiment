# Abstract

Early detection of postprandial glucose excursions in pre-diabetic
individuals remains a significant clinical challenge, as current screening
methods require invasive blood testing and point-of-care visits. In this
work, we investigate whether non-invasive wrist-worn wearable signals ---
electrodermal activity (EDA), heart rate (HR), skin temperature, and
accelerometry --- can predict upcoming glucose spikes before they appear
in the continuous glucose monitor (CGM) record. Using the BIG IDEAs Lab
dataset of 16 pre-diabetic participants wearing simultaneous CGM and
Empatica E4 devices for 8--10 days, we propose a lag-aware classification
framework that accounts for the temporal offset between autonomic nervous
system (ANS) signals and glycemic response. We characterize the lead time
of each wearable modality via a slope-based lag estimation method, then
evaluate whether modality-specific temporal alignment improves binary spike
prediction over a naive zero-lag baseline. We further evaluate the
contribution of food-log-derived nutritional features through an ablation
study. Our zero-lag Random Forest baseline achieves a mean LOO-CV AUROC
of $0.788 \pm 0.086$, and food-log features are found to be critical
contributors. While our lag hypothesis was not confirmed by the data,
the results establish that wearable signals carry strong predictive
information about imminent glucose excursions.

#Running the notebook

This notebook was originally developed on Kaggle, where we reuploaded the BIG IDEAs Glycemic Wearables dataset, as well as cached preprocessed data. To run the pipeline locally, 
download the full dataset, change file path bases as necessary, and run the notebook. All preprocessed data will be saved to disk. The notebook will automatically check
and reuse these files, which will significantly reduce runtime for future iterations. Make sure to clear the files if any modifications to the data preprocessing pipeline are made 
so it may regenerate.
