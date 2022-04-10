# s22-team9-project
Group Members:

1. Emily Musselman
2. Evan Kubick
3. Jason Miller
4. Joseph May
5. Louis Lizzadro



Demo Section:

Implementation

We plan to use Long Short Term Memory recurrant neural network and Generative Adverserial neural networks to generate music. After tuning and standardizing hyperparameters we will compare network performance, and ensure reproducability. 

To install the required libraries open a terminal and input the following commands:

1. sudo apt install -y fluidsynth

2. pip install --upgrade pyfluidsynth

3. pip install pretty_midi

Further help and materials may be found in the reference section


Creating your own dataset & converting files to MIDI (optional):

To begin with, this tutorial assumes songs will be downloaded from youtube as MP4s, converted to MP3s and then from MP3s to MIDI files. This tutorial uses the MiniTool Video Converter Tool and the MP3 to Midi website, which can respectively be found here https://videoconvert.minitool.com/ and here https://anyconv.com/mp3-to-midi-converter/

If the process outlined here is not working, or is not feasable for you there are other ways to convert a file to MIDI type. For instance, if you have to music sheet for a song you can convert that information to MIDI filetype. These solutions are not explored in this demo, and will require research on your part should you wish to employ those options. Outside of free solutions there are a few music conversion tools you may choose from, which can take the form of downloadable software or subscription based web-services. Scan Score offers conveinant MIDI conversion and, as of writing this tutorial, a comprehensive free trial which you can use to do all your file conversions or test to see if that is a tool you would be willing to pay for. It can be found here https://scan-score.com/en/. This tutorial uses an entirely free process described below.  

If you want to get your music generating network up and running immediately there are a number of MIDI libraries out there which you may use for free to provide inputs and start training your network right away. The best libraries we were able to find were:

1. Bitmidi - https://bitmidi.com/
2. The Midi Archive - http://home.claranet.nl/users/fpieters/midipage.html
3. Partners In Rhyme - https://www.partnersinrhyme.com/midi/index.shtml
4. Instant Drum Patterns  - http://www.fivepinpress.com/drum_patterns.html
5. Free Midi Drum Loops -  https://groovemonkee.com/pages/free-midi-loops
6. Blues and Rock-n-Roll Drum Beats - https://www.prosonic-studios.com/midi-drum-beats/blues-and-rock-n-roll
7. Metal Midi - http://metal-midi.grahamdowney.com/midi.html 
8. Midiworld - https://www.midiworld.com/
9. Carlo's midi - https://www.cprato.com/en/midi/all
10. Nonstop2k - https://www.nonstop2k.com/?sid=4be521bd9370621c0c83c9204bd4dcba

Together these libraries offer a solid basis of midi files to begin training your network for music generation. If the files in those libraries do not fit your problem, or you have need for specific songs, you can follow these steps to convert files to MIDI off of youtube. 

The following steps are how we downloaded the top pop songs for 2021 off of youtube and converted them to MIDI format. 
1. Download the MiniTool Video Converter. As of writing this tutorial, it is available for free at  https://videoconvert.minitool.com/ This is the tool we will use to download videos off of YouTube. It is a very easy tool to use, but please keep in mind that version updates to the tool, or alterations to terms and services may outdate this information.

2. Open the MiniTool Video Converter 

3. Click the Video Download tab -- By default this tab will open up a YouTube window within the converter tool, if the files you wish to download are on another website, you can change the URL and navigate to that website.

4. Use the YouTube window and search for the songs you wish, just as if you were using YouTube and not the converter tool. 

5. Select the video you want. 
It is imporant to note here that video slection can affect network performance. If you select Music Videos or other video versions that are not just audio of the song, extra information will be captured in the conversion process. For example, Michael Jackson's Thriller has a runtime of 3 minutes and 22 seconds, but the music video has a runtime of 13 minutes 43 seconds. If you were to download and convert the music video there will be 10 minutes and 35 seconds of unnecessary information endoded to the MIDI file. Ensure you are downloading good quality files for your purpose if you cannot get the officia audio files, or the inputs to your network will contain junk information and lower your performance. 
        
6. Click the download button. -- You will be offered a few different options for how to download the file such as mp3, mp4, and webm. You may select the best file type for your task, for this tutorial songs were downloaded as MP4s. 

7. Once you have downloaded all the songs you want, go to the video convert tab. Upload all the files you wish to convert.

8. Make sure all files are being converted to MP3s and the quality is set to high quality conversion. Then hit the convert all button.

9. Once all files have been converted to MP3s, go to the MP3 to MIDI converter website https://anyconv.com/mp3-to-midi-converter/, which will convert files to MIDI for free. 

10. Upload all the files you wish to convert, and select to convert to MIDI filetype, and hit the convert button. -- It might take some time to convert multiple files to MDID, and occasionally the website has trouble handling large batches of file conversions. We found that batches of 20 files at a time worked best. 

11. At this point you should have MIDI files of your choosing and can use those as inputs for your music generation network. 







References

Jupyterlab - where we developed and tested out code
1. overview - https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html
2. Instillation & setup guide - https://www.tutorialspoint.com/jupyter/jupyterlab_installation_and_getting_started.htm
3. General documentaion - https://jupyterlab.readthedocs.io/en/stable/index.html


Core libraries for the project
1. Tensorflow
        install - https://www.tensorflow.org/install
        introduction - https://www.tensorflow.org/learn
2. Numpy
        install - https://numpy.org/install/
        homepage - https://numpy.org/
3. Pandas
        install - https://pandas.pydata.org/pandas-docs/version/0.23/install.html
        homepage - https://pandas.pydata.org/
6. Fluidsynth
        install - https://github.com/FluidSynth/fluidsynth/releases
        homepage - https://www.fluidsynth.org/ 
8. Pretty_midi
        install - https://pypi.org/project/pretty_midi/
        homepage - http://craffel.github.io/pretty-midi/
             

Tools to download songs and convert to MIDI filetype
1. Minitool Video Converter - https://videoconvert.minitool.com/
2. Anyconv.com - https://anyconv.com/mp3-to-midi-converter/

