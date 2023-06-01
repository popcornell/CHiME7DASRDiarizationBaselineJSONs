# CHiME-7 DASR Diarization Baseline Predictions 

Baseline diarization system predictions (JSONs and RTTMs) as obtained for the CHiME-7 DASR (Task 1) by me.

### Replicability Issues in the diarization baseline system of the CHiME-7 DASR Challenge
There have been replicability issues due to the fact that Ampere devices were used (more info [here](https://github.com/pyannote/pyannote-audio/issues/1370)). 
For future reference/projects it will be a good practice to disable the use of TF32 tensor cores in Pytorch as this will lead to more stable performance across different 
devices and CUDA/CUDNN versions. 


As suggested by [Cristoph Boedekker](https://github.com/boeddeker), due to replicability issues (see [this Pyannote issue](https://github.com/pyannote/pyannote-audio/issues/1370) ), 
I have decided to share, in this repository, the baseline 
predictions as produced by me on a DGXA100 machine.

You can use these "pre-packaged" diarization segmentation as follows by passing, 
as an additional argument `--download-baseline-diarization 1 `.
