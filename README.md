# Music-Generator-RNN
Music generator based on bidirectional LSTM network
## Word about the dataset
MAESTRO (MIDI and Audio Edited for Synchronous TRacks and Organization) is a dataset composed of about 200 hours of virtuosic piano performances captured with fine alignment (~3 ms) between note labels and audio waveforms.

<p align="center">
  <img src="https://github.com/EssamMohamedAbo-ElMkarem/Music-Generator-RNN/blob/main/docs/MAESTRO_models_diagram.png" style="width:800px;"/>
</p>


The dataset contains about 200 hours of paired audio and MIDI recordings from ten years of International Piano-e-Competition. The MIDI data includes key strike velocities and sustain/sostenuto/una corda pedal positions. Audio and MIDI files are aligned with ∼3 ms accuracy and sliced to individual musical pieces, which are annotated with composer, title, and year of performance. Uncompressed audio is of CD quality or higher (44.1–48 kHz 16-bit PCM stereo).
MAESTRO is provided as a zip file containing the MIDI and WAV files as well as metadata in CSV and JSON formats. A MIDI-only archive of the dataset is also available.

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
