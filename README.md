{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "68773717-1983-4c8c-a933-afad924835cb",
   "metadata": {},
   "source": [
    "# Readme- s22-team9-project - Alcove -- Music Generation comparison between LSTM and GAN architectures"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ba1d63ce-7e6f-461e-80aa-b0fc3b25e7b7",
   "metadata": {},
   "source": [
    "   "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "d8ffaae3-66ce-4e49-835d-34527112f1f2",
   "metadata": {},
   "source": [
    "## Motivation \n",
    "\n",
    "We have made two different neural network architectures, a Long-Short-Term-Memoery (LSTM) network and a generative adverserial (GAN) network. We will have each model process musical instrument digital interface (MIDI) files and generate music snippets 30 seconds in length. After tweaking and optimizing the models to the best of our abilities, we will compare the results of each model and observe which model performs better at generating music. \n",
    "\n",
    "___"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a29a2bec-42e6-46cf-aeed-ed13e75c5761",
   "metadata": {},
   "source": [
    "### Datasets\n",
    "\n",
    "The data used for each model can either be found in the Datasets folder in the github, or pulled from other web sources using some code snippets which are included in the pretinent files. The GAN network "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f539e5ff-dac5-4fb7-af65-044d4421966f",
   "metadata": {},
   "source": [
    "_______"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "b5435e9b-1fe2-43db-93a0-314417c6c1b0",
   "metadata": {},
   "source": [
    "### Core tools and dependencies"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "fa65a7ea-44df-4830-9c66-b7efbbfd981d",
   "metadata": {},
   "source": [
    "Jupyterlab – web based user interface\n",
    "1. Homepage - https://jupyter.org/\n",
    "2. Installation -https://jupyter.org/install\n",
    "3. Documentation - https://docs.jupyter.org/en/latest/\n",
    "\n",
    "Tensorflow – build and train neural networks​\n",
    "1. Homepage - https://www.tensorflow.org/\n",
    "2. Installation - https://www.tensorflow.org/install\n",
    "3. Documentation - https://www.tensorflow.org/api_docs/\n",
    "\n",
    "Numpy – Array/Vector/Matrices handling and operations​\n",
    "1. Homepage - https://numpy.org/\n",
    "2. Installation - https://numpy.org/install/\n",
    "3. Documentation - https://numpy.org/doc/\n",
    "\n",
    "Pandas – data analysis and manipulation​\n",
    "1. Homepage - https://pandas.pydata.org/\n",
    "2. Installation - https://pandas.pydata.org/pandas-docs/version/0.23/install.html\n",
    "3. Documentation - https://pandas.pydata.org/docs/\n",
    "\n",
    "Fluidsynth – music synthesizer for midi files​\n",
    "1. Homepage - https://www.fluidsynth.org/\n",
    "2. Installation - https://github.com/FluidSynth/fluidsynth/releases\n",
    "3. Documentation -  https://www.fluidsynth.org/documentation/\n",
    "\n",
    "Pretty_midi – various utilities for handling midi files for formatting & modification\n",
    "1. Homepage - http://craffel.github.io/pretty-midi/#\n",
    "2. Installation - https://pypi.org/project/pretty_midi/\n",
    "3. Documentation - http://craffel.github.io/pretty-midi/\n",
    "\n",
    "Image to Midi conversion\n",
    "\n",
    "1. Code that inspired out GAN network approach for music generation - https://github.com/mathigatti/midi2img\n",
    "2. Contains helper functions and othe information to turn midi files to images for processing\n",
    "\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "11b46afa-14e8-45ca-a311-6eb90056bc41",
   "metadata": {},
   "source": [
    "### Special installation requirements (LSTM Network)\n",
    "\n",
    "To install the required libraries for the LSTM network open a terminal and input the following commands:\n",
    "\n",
    "sudo apt install -y fluidsynth\n",
    "\n",
    "pip install --upgrade pyfluidsynth\n",
    "\n",
    "pip install pretty_midi"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a0b3d353-8dfe-49c3-af61-c5e46539ce28",
   "metadata": {},
   "source": [
    "# Demo "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "5dea3399-4d0c-414b-a137-1171882aff83",
   "metadata": {},
   "source": [
    "## LSTM Network"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "284ba6f2-fbed-4cda-9322-03f4609f44e6",
   "metadata": {},
   "source": [
    "### Preprocessing Data"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "32fadf52-8d82-42da-bd0c-bde08a5bf78e",
   "metadata": {},
   "source": [
    "### Making the model"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "ec191c3a-192b-4787-852d-f82ce745a4a9",
   "metadata": {},
   "source": [
    "## GAN Network"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "3f86302c-34b2-47e1-9779-2c4568fd5a02",
   "metadata": {},
   "source": [
    "### Preprocessing Data"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9c96c45a-54d8-4ae4-a478-0739d098ef1e",
   "metadata": {},
   "source": [
    "### Making the model"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "8bde4d52-fa3f-4a23-b6c1-d78994b69983",
   "metadata": {},
   "source": [
    "### Results Comparison"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "a9601b7e-5c7a-4a25-9241-799c82377bd7",
   "metadata": {},
   "source": [
    "## Sample outputs"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
