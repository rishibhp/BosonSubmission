We conducted an analysis of the embedding space of the TTS odel. Our primary goal was to find an "age" direction for produced audio. Once we had that direction, the expectation was that we could modify quantized audio samples to sound older.

In the process of doing this, we played around with interpolating between different speakers, linearly transforming the embedding vectors, conducting a PCA to find the age direction/vector, and using a dataset too find the "average old vector" and "average young vector".
