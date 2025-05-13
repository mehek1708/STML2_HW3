# *Seattle Bird Call Classification Using Neural Networks*

This project uses Convolutional Neural Networks (CNNs) to classify bird species from sound recordings. Audio clips were preprocessed into mel spectrograms and used to train both binary and multi-class classification models.

## Project Contents

- `HW3_Birds.ipynb` – Final Jupyter Notebook with all code and results
- `test_birds/` – Raw test audio clips in `.mp3` format  
- `test_audio/` – Converted `.wav` versions of the test audio files 
- `test_plots/` – Accuracy/loss plots, spectrograms, and confusion matrices used in the final report  
- `train_extended.txt` – Metadata file for training samples (from Xeno-Canto)  
- `bird_spectrograms.hdf5` – Preprocessed spectrograms for 12 bird species

## Models

### Binary Classification
- **Target Species:** selected random 2 species
- **Training Accuracy:** ~63.8%  
- **Validation Accuracy:** ~67.3%  
- **Loss:** ~0.66  
- **Comments:** Model successfully learned species differences from audio spectrograms.

### Multi-Class Classification
- **Species Count:** 12  
- **Training Accuracy:** ~6.78%  
- **Validation Accuracy:** ~7.06%  
- **Loss:** ~2.61
- **Comments:** Model faced many issues and performed poorly.
- **Challenges:** Class imbalance, similar call patterns, and low inter-class variation affected performance.

## Results
3 unknown bird call clips were processed and passed through the trained multi-class CNN.  
Predictions were logged and compared visually using spectrograms. All related visualizations are in the `test_plots/` folder.

Submitted by: *Mahek Patel*
