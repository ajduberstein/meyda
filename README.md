meyda-docker
===========

JS-driven audio featurization using [Meyda](https://meyda.js.org/audio-features).

Keeps audio feature extraction consistent on server and client.
Made to address concerns listed [here](https://github.com/meyda/meyda/issues/277).

For example, to get the the Mel frequency cepstrum coefficients of an audio file named `mono.wav` in the current directory, run:

```
docker run --rm -v "$(pwd)":/data -w /data ajduberstein/meyda mono.wav mfcc
```
