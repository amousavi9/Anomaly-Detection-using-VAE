# [Anomaly Detection using Variational autoencoder](https://github.com/amousavi9/Anomaly-Detection-using-VAE)
VAEs are data driven, unsupervised models that can learn meaningful latent spaces in many contexts. The VAE is based on an autoencoding framework, which can discover nonlinear explanatory features through data compression and nonlinear activation functions. A traditional autoencoder consists of an encoding phase and a decoding phase where input data is projected into lower dimensions and then reconstructed.18 An autoencoder is deterministic, and is trained by minimizing reconstruction error. In contrast, VAEs are stochastic and learn the distribution of explanatory features over samples.    
VAEs achieve these properties by learning two distinct latent representations: a mean and standard deviation vector encoding. The model adds a Kullback-Leibler (KL) divergence term to the reconstruction loss, which also regularizes weights through constraining the latent vectors to match a Gaussian distribution. VAEs mostly shine as generative models, but the advantages of generating a smooth and continuous latent space can also be of value for anomaly detection tasks. The idea behind Anomaly Detection is to detect samples that are far from what is usually seen, in some sense or other.         
In this work, we use the Chest X-Ray dataset to construct an anomaly detection problem. For an anomaly detection problem, we have normal data as well as anomalies (Pneumonia). We train the VAE model on normal data, then test the model on anomalies to observe the reconstruction error. This technique is called semi-supervised because the model has only seen normal data during training. In real-world scenarios, we don’t necessarily have labeled anomalies; under such circumstances the semi-supervised method is especially useful. We can train the model to learn the distribution of normal data, so when anomalies happened, the model can identify the data that doesn’t fall into the distribution.


# Result
<p align="left" width="100%">
    <img width="50%" src="https://github.com/amousavi9/Anomaly-Detection-using-VAE/blob/main/figs/latent_space.jpg">
</p>

# Evaluation
<p align="left" width="100%">
    <img width="50%" src="https://github.com/amousavi9/Anomaly-Detection-using-VAE/blob/main/figs/loss.jpg">
</p>
