<h2> FD-SALN: Fine-grained and Disentangled Style Representation for Few-shot Speaker Adaptation in Emotional Speech Synthesis </h2>

Submitted to INTERSPEECH 2023 (Paper ID: 1241)


<h3>Abstract</h3>
<img src="./assets/prop.png">

To provide speaking style information for a few-shot text-to-speech (TTS) model, conventional methods normalize the layers of text encoder and mel-spectrogram decoder using affine transformation. However, since these methods utilize a style embedding feature generated utterance-wisely, they are not relevant to provide word- or subword-level fine-scale prosodic variations. In addition, in the few-shot speaker adaptation, it is hard to model unseen speakers' full prosodic variations in the fine-tuning phase because of few target speech samples.
To solve these limitations, we propose a fine-grained style adaptive layer normalization (F-SALN) which manipulates style features on frame-level embeddings. We also propose a disentangled SALN (D-SALN), which independently generates prosody information from speaker and emotional information. From the several experimental results, we demonstrate that our F-SALN and D-SALN improve the intelligibility and fine-scale prosody of synthesized speech.


<h3>Samples - Texts in the JL-Corpus</h3>

<h4>"They should start to talk."</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Emotion
        </td>
        <td class="text">
            <center>Angry</center>
        </td>
        <td class="text">
            <center>Happy</center>
        </td>
        <td class="text">
            <center>Sad</center>
        </td>
        <td class="text">
            <center>Neutral</center>
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_gt/3_m1_A_gt.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_gt/3_f2_H_gt.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_gt/3_m1_S_gt.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_gt/3_f1_N_gt.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Stylespeech</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_sty/3_m1_A_salnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_sty/3_f2_H_salnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_sty/3_m1_S_salnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_sty/3_f1_N_salnjl.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Adaspeech</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_ada/3_m1_A_acmjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_ada/3_f2_H_acmjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_ada/3_m1_S_acmjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_ada/3_f1_N_acmjl.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">FD-SALN (Proposed)</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_fd/3_m1_A_fdsalnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_fd/3_f2_H_fdsalnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_fd/3_m1_S_fdsalnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/they_fd/3_f1_N_fdsalnjl.wav"></audio></td>
    </tr>
</table>


<h4>"Jim saw the port."</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Emotion
        </td>
        <td class="text">
            <center>Angry</center>
        </td>
        <td class="text">
            <center>Happy</center>
        </td>
        <td class="text">
            <center>Sad</center>
        </td>
        <td class="text">
            <center>Neutral</center>
        </td>
    </tr>
    <tr>
        <td class="first-col">Ground Truth</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_gt/2_m1_A_gt.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_gt/2_f1_H_gt.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_gt/2_m1_S_gt.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_gt/2_f1_N_gt.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Stylespeech</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_sty/2_m1_A_salnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_sty/2_f1_H_salnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_sty/2_m1_S_salnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_sty/2_f1_N_salnjl.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Adaspeech</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_ada/2_m1_A_acmjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_ada/2_f1_H_acmjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_ada/2_m1_S_acmjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_ada/2_f1_N_acmjl.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">FD-SALN (Proposed)</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_fd/2_m1_A_fdsalnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_fd/2_f1_H_fdsalnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_fd/2_m1_S_fdsalnjl.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/jim_fd/2_f1_N_fdsalnjl.wav"></audio></td>
    </tr>
</table>


<h3>Samples - Texts in the ESD</h3>

Our proposed model outperforms baselines in terms of intelligibility (pronunciation) proved by experiments. Therefore, the difference in intelligibility between models is noticeable in long sentences. Since all the sentences in JL-Corpus are relatively short, we introduce samples using the sentences in ESD.


<h4>"In which fox loses a tail and its elder sister finds one."</h4>

<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td>
        	Emotion
        </td>
        <td class="text">
            <center>Angry</center>
        </td>
        <td class="text">
            <center>Happy</center>
        </td>
        <td class="text">
            <center>Sad</center>
        </td>
        <td class="text">
            <center>Neutral</center>
        </td>
    </tr>
    <tr>
        <td class="first-col">Stylespeech</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_sty/19_f2_A_saln.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_sty/19_f1_H_saln.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_sty/19_m2_S_saln.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_sty/19_m2_N_saln.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">Adaspeech</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_ada/19_f2_A_acm.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_ada/19_f1_H_acm.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_ada/19_m2_S_acm.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_ada/19_m2_N_acm.wav"></audio></td>
    </tr>
    <tr>
        <td class="first-col">FD-SALN (Proposed)</td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_fd/19_f2_A_fdsaln.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_fd/19_f1_H_fdsaln.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_fd/19_m2_S_fdsaln.wav"></audio></td>
        <td><audio controls="" preload="none"><source src="./assets/samples/in_fd/19_m2_N_fdsaln.wav"></audio></td>
    </tr>
</table>
