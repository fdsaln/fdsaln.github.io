<h1> FD-SALN: Fine-grained and Disentangled Style Representation for Few-shot Speaker Adaptation in Emotional Speech Synthesis </h1>

Submitted to INTERSPEECH 2023 (Paper ID 1241)

<h3>Abstract</h3>
<img src="./assets/prop.png">

To provide speaking style information for a few-shot text-to-speech (TTS) model, conventional methods normalize the layers of text encoder and mel-spectrogram decoder using affine transformation. However, since these methods utilize a style embedding feature generated utterance-wisely, they are not relevant to provide word- or subword-level fine-scale prosodic variations. In addition, in the few-shot speaker adaptation, it is hard to model unseen speakers' full prosodic variations in the fine-tuning phase because of few target speech samples.
To solve these limitations, we propose a fine-grained style adaptive layer normalization (F-SALN) which manipulates style features on frame-level embeddings. We also propose a disentangled SALN (D-SALN), which independently generates prosody information from speaker and emotional information. From the several experimental results, we demonstrate that our F-SALN and D-SALN improve the intelligibility and fine-scale prosody of synthesized speech.

<td><audio controls="" preload="none"><source src="./assets/samples/0_f1_A_fdsalnjl.wav"></audio></td>

