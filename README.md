VAE_1 is on 1 channel input with K=16 and a limited dataset to use but works to show that the vae structure works, however, it was outperformed by PCA. 
The input channel was windspeed only which probably explains why PCA performed better since there was little non-linear correlation to learn on, mostly just smoothness of the wind and land positions.

VAE_2 is on 4 channels now with K=16 and a much larger dataset. PCA uses K/num_channels to allow for fair comparison in terms of size of data reduction since the vae setup compresses all 4 channels into 1.
For K>16, PCA begins to outperform VAE which is evidence to show how power PCA is but also that again there is not much non-linear correlation.

What the VAEs have on PCA is construction of simulated data. Furthermore, PCA is normally limited to just 1 or 2 components so us giving PCA is obviously favouring PCA over the VAE.
