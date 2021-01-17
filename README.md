## PCMProcessing.py  
### Truncate, Elongate data
- TruncateToMinLength,  ElongateToMaxLength  
  These methods takes multiple .tsv files in and cuts or attaches tail to the .tsv file to match the length of the data. The attachment is just a linear approach towards the average of the data.
### Match Frequency
From [last project](https://github.com/Mins0o/PCMLabeler) data of different sampling frequency was created. While facing small-data-problem in the ML experiment, I tried to find a way to combine the two data. Resampling data from a different sampling rate is not a good approach to solve the data shortage problem, but I was able to learn how to use a rather uniform distribution of pseudo-random occurences to make the sampling/interpolating less distorting to the original data.  

## PCMFeature.py
### Fourier Transform
Fourier transform is a rather simple but extremely powerful mathematical tool to analyze audio data. Fourier transform decomposes the sound signal into frequency domain. A detailed method of how I performed the Fourier transform can be seen inside the code's comment.

___
Fourier transform, random sampling with uniform distribution, interpolating with pseudo-random distribution, truncating and elongating PCM data
