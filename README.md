# Music-Generation-Project

In this project, I have used few hindi songs to generate new music tunes. The songs are present in <b> MIDI </b> format. The folder <b> "midi_files"</b> contains these files.

First of all, I have extracted the notes and chords of the music files using the <b>music21</b> library in python. After preprocessing these files I have saved the training data in the <b>"notes"</b> file that contains the notes and chords of all the songs in sequential order.

The next step is building the model for the sequential data. I have used <b> LSTM model</b> from keras library for this purpose. The training data is split into input and output. The input contains first 100 notes and output contains the next note that comes after them. I have trained the model on google colab. After that I have downloaded the model.

Lastly I have used this model for creating new music tunes. The model is fed 100 notes from any input. After that it continuously predicts the next notes and this way generates new music. I have created few music tunes in midi format and saved them in <b>"Generated Music files"</b> folder.
