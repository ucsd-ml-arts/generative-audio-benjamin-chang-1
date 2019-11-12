# Project 3 Generative Audio

Benjamin Chang, bmc011@ucsd.edu

## Abstract

The goal of this project is to try to use generative and interpolation audio networks to create music of the horror genre. In particular, this project aims to create music in this genre which using Performance RNN to produce music, GANSynth to interpolate between various instruments and create new sounds, soundtrap (an online webapp for audio mixing) to produce a coherent horror background track.

The idea is as follows: 1. Generate Music tracks using Performance RNN
                        2. Perform signal manipulation as needed
                        3. Generate new sound tracks modified using GANSynth
                        4. Mix together a horror background soundtrack using an audio mixer

A reasonably spooky and haunting background track was successfully created. Future directions for this work include generating a greater variety of background sounds and exploring more than just the limited sound manipulation methods used in this project. 

## Model/Data

Models
  - Performance_RNN - used to generate new music using only a neural network
  - GANSynth - used for interpolation of music transitions and for creating unique sounds

Data
-Unmodified_Data 
  - 65854__bosone__haunting-violin-fx.wav
  
- Interpolated_Data
  - We_Are_Family_WAV.wav

- Generated_Data
  - sample_output.mid

## Code

Project_2_Generative_Audio.ipynb
Link to Colab below:
  - https://drive.google.com/open?id=1RD4dr6CO9b0D3RhU4D8X7tb2Ii13u79f

## Results

Final Video Result
  - https://www.youtube.com/watch?v=f0o3SnGUmi0

Mixed Sound File (.mp3)
  - Project_2_Generative_Audio.mp3

Mixed Sound
  - https://www.soundtrap.com/studio/KcQILp-qS0u9kIEYH1DSgg/

Modified Sound Files
  - We_Are_Family_WAV.wav
  - sample_output.mid

## Technical Notes

PERFORMANCE_RNN

This code runs on Colab. Performance RNN should run out of the box. For this project, a temperature of 0.9 was used. This produced audio results with less chance of having large sections of blank spots in the audio produced, but also a higher chance of generating better sounding and more complex sounding music which is desirable.

The pitch and velocity data within the generated audio are then accessed and modified to produce a higher pitch and velocity (shorter time for each note to last). These helped generate the more unnerving and uncanny sound needed for horror background music. The result is converted into a midi file.


GANSYNTH

For the "Random Interpolation" section, make sure to first run the code section and then upload a file while the code is running before it produces an error message due to no file being detected. The pitch and velocity are adjusted once again during interpolation, but these values can be changed as needed.

The final code section was written to mix and play the resulting audio files, but is commented out due to this project ending up using a webapp mixer which was able to reverse audio files much easier. The section can be used if needed.

## Reference

Performance RNN
https://github.com/tensorflow/magenta/tree/master/magenta/models/performance_rnn

GANSynth
https://github.com/tensorflow/magenta/tree/master/magenta/models/gansynth

Audio Mixer Webapp
soundtrap.com

