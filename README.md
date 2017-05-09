# Autoencoder-in-Julia

This reprository introduces julia implementation for PCA (principle component analysis) and some feature learning algorithms such as Autoencoders.

Some basic concepts are used from:
http://ufldl.stanford.edu/tutorial/unsupervised/Autoencoders/

-> PCA_Whitening.ipynb
is the notebook of julia code of Data whitening where all features in data become with zero mean, unit variance and uncorrelated
and then data reduced to lower dimentionality using only k features, where k is determined by a function


-> Sparse_Autoencoder_MNIST.ipynb
is the notebook of julia code of k-sparse autoencoder for feature learning of MNIST dataset. Each step of autoencoder is implemented from scratesh, either the forward or the backward path with backpropagation based on the steps in the above stanford link. Finally, a test of autoencoder is done by comparing the output and the input image (which assumed to be identical if the autoencoder learned well)
