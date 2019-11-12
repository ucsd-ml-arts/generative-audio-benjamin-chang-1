# Project 3 Generative Audio

Benjamin Chang, bmc011@ucsd.edu

## Abstract

The goal of this project is to try to use generative and interpolation audio networks to create music of a new genre. In particular, this project aims to create music in this new genre named steamfunk disco using GANSynth to interpolate between various instruments and Performance RNN to produce a coherent track. This will be done by manipulating parameters in the The Steamfunk Disco's lyrics will likely be added later to the generated music.

The idea is as follows: 1. Generate Music tracks using Performance RNN
                        2. Perform signal manipulation as needed
                        3. Combine tracks using GANSynth

"Include your abstract here. This should be one paragraph clearly describing your concept, method, and results. This should tell us what architecture/approach you used. Also describe your creative goals, and whether you were successful in achieving them. Also could describe future directions."

## Model/Data

Models
- Performance_RNN - used to generate new music using only a neural network
- GANSynth - used for interpolation of music transitions and for creating unique sounds

Data
- Unmodified_Data
  - Hoedown_WAV.wav
  - Achy-Breaky-Heart_WAV.wav
  - We_Are_Family_WAV.wav

- Generated_Data
  - sample_output.mid

## Code

Project_2_Generative_Audio.ipynb
Link to Colab below:
https://drive.google.com/open?id=1RD4dr6CO9b0D3RhU4D8X7tb2Ii13u79f

## Results

Documentation of your results in an appropriate format, both links to files and a brief description of their contents:
- `.wav` files or `.mp4`
- `.midi` files
- musical scores
- ... some other form

## Technical Notes

Any implementation details or notes we need to repeat your work. 
- Does this code require other pip packages, software, etc?
- Does it run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

References to any papers, techniques, repositories you used:
- Papers
- Repositories
- Blog posts

https://github.com/tensorflow/magenta/tree/master/magenta/models/performance_rnn
https://towardsdatascience.com/generate-piano-instrumental-music-by-using-deep-learning-80ac35cdbd2e
http://rosemck1.tripod.com/jukebox-country.html

