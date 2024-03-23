# KiloNeRF-Implementation
A basic implementation of the KiloNeRF novel view genrative model.

Some training data to get started can be [downloaded from here](https://drive.google.com/drive/folders/18bwm-RiHETRCS5yD9G00seFIcrJHIvD-)

Using that training data with the default settings in the codebase is how the small sample of example images found in the novel_views folder were generated.

The simplest way to run this codebase is with Google Colab, as the model takes a significant amount of time/horsepower to train.

By default, the batch size and resolutions selected in the code will require ~35gb of VRAM to run, so if you are using any smaller GPUs then you will have to reduce that by at least half to get it to run. 
The code is also set up by default to only run to 8 epochs so that it can be experimented and iterated with on a semi-reasonable time scale. However, this limits the resolution of the outputs significantly.
If high-res outputs are desired, then the number of epochs should be increased by at least double, though expect that the training time for that will be several hours or more.
