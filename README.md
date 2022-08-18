# Music-Generator-RNN
Music generator based on bidirectional LSTM network
## Word about the dataset
MAESTRO (MIDI and Audio Edited for Synchronous TRacks and Organization) is a dataset composed of about 200 hours of virtuosic piano performances captured with fine alignment (~3 ms) between note labels and audio waveforms.

<p align="center">
  <img src="https://github.com/EssamMohamedAbo-ElMkarem/Music-Generator-RNN/blob/main/docs/MAESTRO_models_diagram.png" style="width:800px;"/>
</p>


The dataset contains about 200 hours of paired audio and MIDI recordings from ten years of International Piano-e-Competition. The MIDI data includes key strike velocities and sustain/sostenuto/una corda pedal positions. Audio and MIDI files are aligned with ∼3 ms accuracy and sliced to individual musical pieces, which are annotated with composer, title, and year of performance. Uncompressed audio is of CD quality or higher (44.1–48 kHz 16-bit PCM stereo).
MAESTRO is provided as a zip file containing the MIDI and WAV files as well as metadata in CSV and JSON formats. A MIDI-only archive of the dataset is also available.

## Word about RNN

A recurrent neural network (RNN) is a class of artificial neural networks where connections between nodes form a directed or undirected graph along a temporal sequence. This allows it to exhibit temporal dynamic behavior. Derived from feedforward neural networks, RNNs can use their internal state (memory) to process variable length sequences of inputs.This makes them applicable to tasks such as unsegmented, connected handwriting recognition or speech recognition.Recurrent neural networks are theoretically Turing complete and can run arbitrary programs to process arbitrary sequences of inputs.

<p align="center">
  <img src="https://github.com/EssamMohamedAbo-ElMkarem/Music-Generator-RNN/blob/main/docs/The-standard-RNN-and-unfolded-RNN.png" style="width:800px;"/>
</p>
The term "recurrent neural network" is used to refer to the class of networks with an infinite impulse response, whereas "convolutional neural network" refers to the class of finite impulse response. Both classes of networks exhibit temporal dynamic behavior.A finite impulse recurrent network is a directed acyclic graph that can be unrolled and replaced with a strictly feedforward neural network, while an infinite impulse recurrent network is a directed cyclic graph that can not be unrolled.

Both finite impulse and infinite impulse recurrent networks can have additional stored states, and the storage can be under direct control by the neural network. The storage can also be replaced by another network or graph if that incorporates time delays or has feedback loops. Such controlled states are referred to as gated state or gated memory, and are part of long short-term memory networks (LSTMs) and gated recurrent units. This is also called Feedback Neural Network (FNN). 

## BI-LSTM(Bi-directional long short term memory)

Bidirectional long-short term memory(bi-lstm) is the process of making any neural network o have the sequence information in both directions backwards (future to past) or forward(past to future). 

<p align="center">
  <img src="https://github.com/EssamMohamedAbo-ElMkarem/Music-Generator-RNN/blob/main/docs/bidlstm.jpeg" style="width:800px;"/>
</p>

In bidirectional, our input flows in two directions, making a bi-lstm different from the regular LSTM. With the regular LSTM, we can make input flow in one direction, either backwards or forward. However, in bi-directional, we can make the input flow in both directions to preserve the future and the past information.

## Loss curve and generated output

<p align="center">
  <img src="https://github.com/EssamMohamedAbo-ElMkarem/Music-Generator-RNN/blob/main/docs/loss.png" style="width:500px;"/>
</p>

<p align="center">
  <img src="https://github.com/EssamMohamedAbo-ElMkarem/Music-Generator-RNN/blob/main/docs/outdis.png" style="width:800px;"/>
</p>
