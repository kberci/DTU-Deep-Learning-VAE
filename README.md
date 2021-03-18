# VAE
Variational auto-encoders project for DTU course 02456.

## Colab
Test out the model in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DTU-VAE/VAE/blob/master/vae_train.ipynb)

## Description
This project is the implementation of a variational auto-encoder used to generate midi music data. 
The dataset used to train the model is the MAESTRO set, which contains a couple hunder hours of piano music stored in the MIDI format. 
The VAE model’s encoder and decoder are implemented as LSTM modules which are able to remember past information as they train on the songs. 
A custom dataloader is implemented which randomly batches the songs to train on, but sequentially samples the time sequence from these selected songs.

<script>
var audio = new Audio("https://github.com/kberci/DTU-Deep-Learning-VAE/blob/master/generated_sample.mp3")
audio.play()
</script>

[Generated piano music-example](/generated_sample.mp3 "Example of generated piano music by the VAE model")
