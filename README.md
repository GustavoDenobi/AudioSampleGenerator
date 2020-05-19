# Creating a dataset generator from TTS and noise
The idea consists on creating a generator that mixes voices from a multiple-speaker TTS engine with ambient noises, generating audio samples to be used for training the MOTH architectures. The results of such artificial dataset is yet to be validated.

One issue here is that the output samples can only be generated in the same language as the TTS engine.

Each generated sample is going to be saved as a WAV file, with a name consisting of an id number and it's label, according to the following:

AAAAAA-BCD.wav
AAAAAA: id number with zero padding

B: bool for the presence of speech

C: bool for the presence of multiple speakers

D: bool for the presence of the activation commmand
