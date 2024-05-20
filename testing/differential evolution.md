After trying average weighted ensemble where each model has equal weight (therefore equal contribution) during prediction, we tried differential evolution to get optimal set of weights.

# Saving predictions of trained models on validation dataset (for each model):
First we saved the predictions for validation dataset (for each model):
https://www.kaggle.com/code/smnabilashraf/valid-all-nofinding-stage2/notebook

# Running differential evolution
We loaded the predictions saved in previous notebook and ran differential evolution where the loss function tries to maximize roc_auc. We then applied the optimal weights on the test dataset:
https://www.kaggle.com/code/smnabilashraf/valid-preds-optimal-weight-finder/notebook
