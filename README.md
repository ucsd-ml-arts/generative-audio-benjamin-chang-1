# Project 3 Generative Audio

Benjamin Chang, bmc011@ucsd.edu

## Abstract

The goal of this project is to try to prove that it is possible to use generative and interpolation audio networks to replicate particular music genres. In particular, this project aims to create new music in the future funk genre using GANSynth to interpolate between various instruments and Performance RNN to produce different tracks. This will be done by manipulating parameters in the The Future Funk lyrics will likely be added later to the generated music.

The idea is as follows: 1. Generate Music tracks using Performance RNN
                        2. Perform signal manipulation as needed
                        3. Combine tracks using GANSynth

"Include your abstract here. This should be one paragraph clearly describing your concept, method, and results. This should tell us what architecture/approach you used. Also describe your creative goals, and whether you were successful in achieving them. Also could describe future directions."

## Model/Data

Briefly describe the files that are included with your repository:
- trained models
- training data (or link to training data)

## Code

Your code for generating your project:
- Python: generative_code.py
- Jupyter notebooks: generative_code.ipynb

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

