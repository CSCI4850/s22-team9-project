Readme- s22-team9-project Alcove  
 
This is a project utilizing two different Neural Networks architectures, Long-Short-Term-Memory (LSTM) and Generative Adversarial (GAN), to create music. After building and training each model, the results of both models were compared primarily through loss and accuracy ratings, but also in number of parameters (neural units), and overal song quality to be able to compare which architecture LSTM or GAN is better at generating music. 

Motivation:
We have made two different neural network architectures, a Long-Short-Term-Memoery (LSTM) network and a generative adverserial (GAN) network.
We will have each model process musical instrument digital interface (MIDI) files and generate music snippets 30 seconds in length. After tweaking 
and optimizing the models to the best of our abilities, we will compare the results of each model and observe which model performs better at generating music. 

Datasets:
The data used for each model can either be found in the Datasets folder in the github, or pulled from other web sources using some code snippets which are 
included in the pretinent files. 

Core tools and dependencies:

Jupyterlab – web based user interface
1. Homepage - https://jupyter.org/
2. Installation -https://jupyter.org/install
3. Documentation - https://docs.jupyter.org/en/latest/

Tensorflow – build and train neural networks​
1. Homepage - https://www.tensorflow.org/
2. Installation - https://www.tensorflow.org/install
3. Documentation - https://www.tensorflow.org/api_docs/

Numpy – Array/Vector/Matrices handling and operations​
1. Homepage - https://numpy.org/
2. Installation - https://numpy.org/install/
3. Documentation - https://numpy.org/doc/

Pandas – data analysis and manipulation​
1. Homepage - https://pandas.pydata.org/
2. Installation - https://pandas.pydata.org/pandas-docs/version/0.23/install.html
3. Documentation - https://pandas.pydata.org/docs/

Fluidsynth – music synthesizer for midi files​
1. Homepage - https://www.fluidsynth.org/
2. Installation - https://github.com/FluidSynth/fluidsynth/releases
3. Documentation -  https://www.fluidsynth.org/documentation/

Pretty_midi – various utilities for handling midi files for formatting & modification
1. Homepage - http://craffel.github.io/pretty-midi/#
2. Installation - https://pypi.org/project/pretty_midi/
3. Documentation - http://craffel.github.io/pretty-midi/

Image to Midi conversion

1. Code that inspired out GAN network approach for music generation - https://github.com/mathigatti/midi2img
2. Contains helper functions and othe information to turn midi files to images for processing

LSTM Architecture Inspiration 
1. Keras Tutrotial - https://www.tensorflow.org/tutorials/audio/music_generation



Special installation requirements (LSTM Network):


 To install the required libraries for the LSTM network open a terminal and input the following commands:

  1. sudo apt install -y fluidsynth

  2. pip install --upgrade pyfluidsynth

  3. pip install pretty_midi


Special installation requirements (GAN Network):

 To install the required libraries for the GAN network open a terminal and input the following commands:

  1. pip install music21
