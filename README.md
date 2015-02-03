# SongPredict

This is for a data science competition to predict whether a 1/2 second clip of one of eight Taylor Swift songs is popular.

The first thing I tried is to use Random Forest algorithm on just the time data, just the Fourier transformed data,
or the combination of the two.

Surprisingly to me, the time data gave much better performance than the FT.  (This is in script-time-and-ft.ipynb)

I'm currently working on getting STFT to work, and then integrating over the frequency dimension of each time slice to 
determine which snippets within the 1/2 second clip are "interesting features".  Taking the FT spectrum from each of
of these slices might prove to give better identifiable features - this is adapted from the approach in the paper
that I've added to this repo, and the most current version is script3.ipynb

