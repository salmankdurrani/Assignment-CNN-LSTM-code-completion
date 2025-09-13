## Assignment

In this assignment you’ll receive a partially completed notebook that implements video action recognition with a **CNN + LSTM**. Your job is to **finish the missing parts** so the pipeline runs end to end on a small dataset and produces clear evaluation outputs.

**Here you will find the GitHub link to the code you need to complete.**


## Your task

1. Load the dataset (folder per class).
    
2. Turn videos into fixed‑length frame **sequences** (same steps for train/val/test and inference).
    
3. Build the model (instruction are given in the .ipynb file)
    
4. Train with a validation split and early stopping; save training curves.
    
5. Evaluate on the **test** set and generate the required plots.
    
6. Run **inference** on at least 5 short clips and print the predicted class (and, if you like, a short timeline).
    

## What to submit (required)

Submit **the complete code**, including **data preprocessing, model training, model evaluation, and action prediction sections**. Also include:

- **Model training and loss curves**
- **Model accuracy**
- **Confusion matrix on your test set** (labels on both axes).
- **Precision and recall curves** (per‑class or macro).
- **Optional:** **t‑SNE visualization of the features** (e.g., features from the LSTM or penultimate dense layer).

Package your work as a single zip/folder named `assignment_action_recognition_<yourid>` containing:

- The completed notebook (all cells run, outputs visible).
    
- Any helper modules or scripts you created.
    
- A `results/` folder with your plots saved (confusion matrix, PR curves, optional t‑SNE).
    
- A short `README.md` with: dataset path setup, key parameters (sequence length, input size, fps), and how to run.
    

## Grading (100 pts)

- Data pipeline complete & consistent (train/val/test + inference): **25**
    
- Model builds and trains without errors; sensible settings & callbacks: **25**
    
- Evaluation quality (confusion matrix + precision/recall curves, brief interpretation): **25**
    
- Inference on a new video using the **same** preprocessing: **15**
    
- Code clarity & README (reproducible, seeds set, paths configurable): **10**
    
- **Bonus (+5):** meaningful t‑SNE of features.
    

## Notes

- Keep it lightweight (e.g., ~112×112 inputs, ~S=16–24 frames per sequence) so it runs on a laptop/GPU in minutes.
    
- Use the **same preprocessing** in training and inference.
    
- Set a random **seed** and print library versions for reproducibility.
    
- Use can use google colab to run the code without running into package issues.
    

**Deadline & submission method:** As announced on the course page. Make sure your zip opens and the notebook runs top to bottom without manual fixes.
