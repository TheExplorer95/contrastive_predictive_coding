# Solving music genere classification with ease of a contrastive predictive coding model

**How to** use the code:

1. Acquire the following datasets: GTZAN (/data/GTZAN), fma_small (/data/fma_small_mono_wav) and youtube (/data/test_data) and place them into their respective folder
3. Set the desired model to train within run_experiment.sh [1dconv_gru/, 1dconv_transformer/, 2dconv_gru/]
4. Run the bashscript from the command line: ./run_experiment.sh

To interact with the Framework on a more low level handling of the parameters and models check out the README file inside the scripts folder.

**Folders**

1. /Data conversion: scripts to convert data
2. /models: trained model weights
3. /history: .npy of training results, call with np.load(allow_pickle=True).item()
4. /scripts: python scripts to run the model
5. /Music from Youtube.pdf: how to acquire the dataset for testing the classifier

**Files**

 - params.py: only file to change
 - train_cpc.py: train cpc and save weights
 - generate_embeddings.py: generate embeddings using trained cpc
 - train_classifiers.py: train and test classifiers using embeddings

