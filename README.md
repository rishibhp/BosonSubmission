We conducted an analysis of the embedding space of the TTS model. Our primary goal was to try to achieve voice modulation by performing manipulations in the embedding space of the model itself.

The base idea is find an "age direction" in the embedding space and then add a vector like this to a give audio embedding to make it sound older. The way we do this is we find a dataset of audio samples with ages labelled (we used the Mozilla Common Voice dataset). Then averaging the older audio samples (eighty year olds) and younger audio samples (twenty year olds) we can get vectors representing old voices and young voices. Then by taking a difference we, in principle, should have the "age direction".

In the process of doing this, we played around with interpolating between different speakers, linearly transforming the embedding vectors, conducting a PCA to find the age direction/vector, and using a dataset too find the "average old vector" and "average young vector".
